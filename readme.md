# Unity for ReSharper

This plugin adds basic support for [Unity](http://unity3d.com/) to ReSharper.

Current features:

* ReSharper knows about classes that derive from `UnityEngine.MonoBehaviour` and the classes, public fields and methods are no longer marked as unused when Solution Wide Analysis is enabled.
* <kbd>Alt</kbd>+<kbd>Insert</kbd> on `MonoBehaviour` classes to generate event handlers, with method parameters. Invoke the shortcut on the class declaration.
* Suppresses the naming consistency warnings on `MonoBehaviour` event handlers. E.g. ReSharper no longer suggests that `AnimatorIK` be renamed to `AnimatorIk`.
* Disables the `Assets` and `Assets\Scripts` from being considered as "namespace providers". This means ReSharper will no longer suggest to include `Assets` or `Scripts` in the namespace of your code.
* Automatically sets Unity projects to be C# 5 only. The Unity compiler is only C# 5, so no more incompatible C# 6 suggestions!

That's it! If you want anything else, [suggest it](https://github.com/JetBrains/resharper-unity/issues)!

## Installing

Use ReSharper's Extension Manager (ReSharper &rarr; Extension Manager), search for "Unity" and install. Restart, and it'll just start working.

Please watch the repo or follow [@citizenmatt](https://twitter.com/citizenmatt) and [@slavikt](https://twitter.com/slavikt) on twitter for updates.

## Roadmap

There is no roadmap as such. I am not a Unity developer, so do not know what the common pain points are. If you'd like to suggest a feature, please [raise an issue](https://github.com/JetBrains/resharper-unity/issues).

Some ideas:
 
 * Convert void method into CoRoutine (and updating usages)
