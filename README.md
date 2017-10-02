# DT Overview
A list of open-source Unity tools / modules made by @darrentsung. The goal is to make it easier to discover which repositories might be helpful for an external user.

Sorted by star rating (recommendation level for external users).

## ★★★★★ - Highly Recommended
#### [DTCommandPalette](https://github.com/DarrenTsung/DTCommandPalette)
Inspired by similar command palettes from sublime text + atom. Quickly run methods, find GameObjects in the scene, etc. Easy to extend and add new commands. Great for power users.

I integrate DTCommandPalette into a lot of my other packages and use it heavily.

```csharp
public static class ExampleClass {
	[DTCommandPalette.MethodCommand]
	public static void DeletePlayerPrefs() {
		PlayerPrefs.DeleteAll();
	}
}
```

#### [DTValidator](https://github.com/DarrenTsung/DTValidator)
Runs prefab / scene validation to quickly check that all outlets that are required (required by default) are filled out. Any errors are displayed in the validation window.

#### [DTLocalization](https://github.com/DarrenTsung/DTLocalization)
Localization framework that has support for GDocs database backend through GDataDB, easy to extend for other backends. Built-in offline caching that's easy to integrate in your CI pipeline.

#### [DTFPSView](https://github.com/DarrenTsung/DTFPSView)
Simple API for an FPS tracker along with built-in UI including graph for DEBUG builds.

#### [DTCompileTimeTracker](https://github.com/DarrenTsung/DTCompileTimeTracker)
Simple editor extension for tracking compile time, use this in conjunction with my article: TK add article to make sure you have the fastest iteration (code -> compile -> code) loop possible.

#### [DTDebugMenu](https://github.com/DarrenTsung/DTDebugMenu)
Easily extended UI for debug functionality - turn off 20+ keybindings and use this instead! Easy to define new UI through code.

## ★★★★ - Recommended, But Not Super Special
#### [DTPrefabSandbox](https://github.com/DarrenTsung/DTPrefabSandbox)
Tired of dragging out prefabs into the scene to modify them? Use DTPrefabSandbox!

Open up prefabs into a separate scene to be modified and then return back to the scene you were in. Integrates DTValidator for real-time validation while editing.

#### [DTMediaCapture](https://github.com/DarrenTsung/DTMediaCapture)
API / keybindings for taking screenshots and recording video. Some alternatives that are more feature complete on the App Store, but this is really easy to setup and use.

TK Also check out keijros videocapture repository - didn't see this when I first built this thing!

#### [DTTimeScaleScrubber](https://github.com/DarrenTsung/DTTimeScaleScrubber)
Use keybindings or touch to scrub time from speeding up + slowing down using Time.timeScale. Comes with UI that overlays on top of the game.

#### [DTBuildManifest](https://github.com/DarrenTsung/DTBuildManifest)
Has built-in extensions to be used with DTDebugMenu.

Reads UnityCloudBuildManifest and adds it as a tab to the DTDebugMenu. Can easily extend and add a different type of manifest for listing additional build information.

#### [DTUIRebuildVisualizer](https://github.com/DarrenTsung/DTUIRebuildVisualizer)

## ★★★ - Useful, But Requires Willingness To Use
#### [DTObjectPoolManager](https://github.com/DarrenTsung/DTObjectPoolManager)
Useful API for creating / recycling prefabs that allows MonoBehaviours to hook into the recycle / cleanup lifecycle. Has some specific frame delay logic for handling recycling animators correctly that makes it more complex than might be needed for most cases.

#### [DTEasings](https://github.com/DarrenTsung/DTEasings)
Simple easing API that I'm used to. Adds easing Coroutine extensions to MonoBehaviours / GameObjects like `this.DoEaseFor(float delay, EaseType easeType, Action<float> callback)`.

#### [DTAnimatorStateMachine](https://github.com/DarrenTsung/DTAnimatorStateMachine)

#### [DTViewManager](https://github.com/DarrenTsung/DTViewManager)

#### [DTCoreModule](https://github.com/DarrenTsung/DTCoreModule)

