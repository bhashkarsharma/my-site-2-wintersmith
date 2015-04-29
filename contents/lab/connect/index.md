---
title: Connect
template: page.hbs
description: In-browser chat application
style: true
script: true
---
A simple peer-to-peer chat application that allows people to watch YouTube videos in sync.

<link rel="stylesheet" href="/css/mediaelementplayer.min.css"/>
<script src="http://cdn.peerjs.com/0.3/peer.min.js"></script>
<script src="/js/mediaelement-and-player.min.js"></script>
<div class="login 6u">
    <form>
        <label>Your id is: <input id="username" value="being fetched"></label>
    </form>
</div>

<div class="video-box" id="video">
    <video width="640" height="360" id="player" preload="none">
        <source type="video/youtube" src="http://www.youtube.com/watch?v=Wch3gJG2GJ4" />
    </video>
</div>

<div id="chats">
</div>
<a href="javascript:void(0);" id="clearChats">Clear history</a>

<div class="row">
    <div class="3u">
        <input type="text" name="peername" id="peername" placeholder="Peer name">
    </div>
    <div class="8u">
        <input type="text" name="msg" id="msg" placeholder="Message">
    </div>
    <div class="1u">
        <input type="submit" id="send" value="&gt;">
    </div>
</div>