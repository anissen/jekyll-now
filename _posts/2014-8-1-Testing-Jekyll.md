---
layout: post
title: Testing 1, 2, 3...
---

This is a simple post to try out blog handling with _Jekyll_.

Here is another paragraph.

And a list!

* Here
* It
* Goes

Some _Haxe_ source code that may or may not be syntax highlighted:

{% highlight haxe %}
private function setupGame():Void
{
	var stageWidth :Int = Lib.current.stage.stageWidth;
	var stageHeight :Int = Lib.current.stage.stageHeight;

	if (zoom == -1)
	{
		var ratioX :Float = stageWidth / gameWidth;
		var ratioY :Float = stageHeight / gameHeight;
		zoom = Math.min(ratioX, ratioY);
		gameWidth = Math.ceil(stageWidth / zoom);
		gameHeight = Math.ceil(stageHeight / zoom);
	}

      Reg.gameManager = new GameManager();
      Reg.networkManager = new NetworkManager();
      Reg.networkManager.connect();
	addChild(new FlxGame(gameWidth, gameHeight, initialState, zoom, framerate, framerate, skipSplash, startFullscreen));
}
{% endhighlight %}
