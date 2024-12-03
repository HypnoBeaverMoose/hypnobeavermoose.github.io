---
layout: post
title:  "Game Architecture Using Scriptable Objects Part 1"
---

It's been over seven years since Unite 2017 at Austin, but there is a certain video from that conference, that I constantly find myself going back to. If you've worked with Unity 3D in any kind of professional capacity in the time since, you've probably seen it too. 
I am of course talking about Ryan Hipple's seminal lecture on building game architecture using scriptable objects.

[![IMAGE ALT TEXT HERE](http://img.youtube.com/vi/raQ3iHhE_Kk/0.jpg)](https://www.youtube.com/watch?v=raQ3iHhE_Kk) 

It is the most watched Unite conference video in Unity's youtube channel - and by a lot. Coincidentally, the video [in second place](https://www.youtube.com/watch?v=6vmRwLYWNRo), which has almost half the views is on the same subject matter. Apparently 2016/2017 were great years for scriptable objects!

### ControllerManager.cs

There is a very good reason why this lecture is so popular. It came out right around the time where all of us (Unity devs) were up to our neck in `Managers`, `Controllers` and `ControllerManagers` and it had become very apparent to everyone and their grandma, that the "primary" way of making games in Unity was not cutting it. Especially for large projects. There were the usual problems with initialization race conditions (which "Awake" get's called first), unwieldy swiss army knife classes, and the complete inability to test any of this mess efficiently, because for the simplest test you needed to run the whole thing. Not to mention the fact, that the simplest change you needed a developer around, and not just any developer - one that new their way around this mess. The code was technically "modular" - it had "modules", but because everything had to be kept "in the scene", it was very easy to jumble everything together into one big incoherent mess. You could do a lot with `static` classes in C#, but then you ran into the problem of domain reload, and the fact that those static values keep persisting even when you don't want them to.

### Overthrowing the MonoBehaviour Tyranny in a Glorious Scriptable Object Revolution

Enter `ScriptableObject`. At the time it was a fairly obscure piece of the engine, that most people ignored, and some used to fill with all kinds of configuration data. Basically, you would have one `ScriptableObject` called `GameData`, fill that with an ungodly combination of data, and then pass it to anything that might need to be "configured" somehow.

```cs
public class GameData : ScriptableObject
{
    public float playerHealth;
    public int enemyCount;
    public bool isDemo;
    public string copyrightMessage;
}
```
Few of us realized, that you can actually fill those things with logic - and use that code as... you know - data! So you can imagine what a game changer Ryan's lecture was to a lot of us. Here was a completely new way to organize your game, which was in essence very simple and easy to follow. It forced you to separate your data, and work in concepts that were easily accessible to designers and an other not-necessarily-technical people in the team. It was testable - it allowed you do drag a single prefab in the scene and see it work. But most of all it opened our eyes to the idea that the editor wasn't that chunky UI thing, that you constantly needed to wrestle with to get your job done. It was essentially a [dependency injector](https://en.wikipedia.org/wiki/Dependency_injection).


## Game Architecture Using Scriptable Objects

As you can tell from, that lecture has had a big impact on me. Over the last several years I end up implementing different variations of these ideas time and again. Which is why I decided to build a small library, that can easily be imported into Unity as a package. This library can then serve as basis for developing prototypes or even full fledged games. I myself plan to use it in a number of projects, which I'll hope to share in the future.

Those who watched the video will no doubt point out that, there is actually code in there, and there is a repo in github with it. So why do you need to write it again? Well, the code in the video is not actually "production" code, it's more of an illustration of an approach, and as soon as you start to use it in practice a bunch of stuff jump out at you. Problems, which I have solved, so you don't have to!

The library is modeled on a number of abstract generic classes, that can be inherited to create concrete representations for concept in your project.
```cs
    [CreateAssetMenu]
    public class StringVariable : Variable<string> { }
```
You can use these to create scriptable objects in the project. Most of these work in tandem with a corresponding editor script, that enables certain neat functionalities, such as displaying the current value of a variable, or invoking an event manually. Adding that is also straightforward: 

```cs
    [CustomEditor(typeof(BoolEvent))]
    public class BoolEventEditor : EventEditorBase<bool> { }
```

Event better, I've gone ahead and covered most of the basic cases of C# primitives as well as vectors. They also provide a nice blueprint, in case you get stuck. In the [second part](/2024-12-07-game-architecture-using-scriptable-objects-part-2.md) I take deep dive into the actual implementation and highlight some of the more interesting aspects and reasoning behind various decisions I've made.

[THE LINK](https://github.com/HypnoBeaverMoose/ScriptableLibrary)