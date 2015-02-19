---
title: Segment Clock
template: page.hbs
---
<style type="text/css">
.container.box.style3 {
    padding: 0;
    text-align: center;
}

#post section {
    background: black;
    padding: 1em;
    text-align: center;
}

.cover {
    position: relative;
    background: black;
    opacity: 0.85;
    z-index: 1;
}

.top, .bottom {
    height: 60px;
}

.before, .middle, .after {
    height: 157px;
    width: 50px;
    float: left;
}

.marker {
    width: 70px;
}

.marker .knob {
    left: 25px;
}

.marker .knob:nth-child(1) {
    top: 35px;
}

.marker .knob:nth-child(2) {
    top: 100px;
}

.marker.blink .knob {
    visibility: hidden;
}

.clear {
    clear: both;
}

.digit {
    position: relative;
    width: 90px;
    height: 155px;
    float: left;
}

.node {
    position: absolute;
}

.edge {
    width: 20px;
    height: 65px;
    border: 1px solid #aaa;
    border-radius: 12px;
    position: absolute;
    transform-origin: 11px 11px;
    transition-duration: 0.5s;
    background: #e6e6e6;
    box-shadow: 1px 1px 1px #666;
}

.knob {
    width: 20px;
    height: 20px;
    border: 1px solid #aaa;
    background-color: #e6e6e6;
    border-radius: 12px;
    z-index: 1;
    position: absolute;
    box-shadow: 2px 2px 4px #666;
}

.inner {
    width: 10px;
    height: 10px;
    border: 1px solid #aaa;
    border-radius: 10px;
    left: 4px;
    top: 4px;
    position: absolute;
}

.node:nth-child(1) {
    left: 0;
    top: 0;
}
.node:nth-child(2) {
    right: 22px;
    top: 0;
}
.node:nth-child(3) {
    left: 0;
    top: 67px;
}
.node:nth-child(4) {
    right: 22px;
    top: 67px;
}
.node:nth-child(5) {
    left: 0;
    bottom: 22px;
}
.node:nth-child(6) {
    right: 22px;
    bottom: 22px;
}

</style>

<div class="cover top"></div>

<div class="maincontent">
<div class="cover before"></div>

<div class="digit" id="hour1">
    <div class="node 00">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 01">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 10">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 11">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 20">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 21">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
</div>

<div class="cover middle"></div>

<div class="digit" id="hour0">
    <div class="node 00">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 01">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 10">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 11">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 20">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 21">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
</div>

<div class="cover middle marker">
    <div class="knob">
        <div class="inner"></div>
    </div>
    <div class="knob">
        <div class="inner"></div>
    </div>
</div>

<div class="digit" id="min1">
    <div class="node 00">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 01">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 10">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 11">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 20">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 21">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
</div>

<div class="cover middle"></div>

<div class="digit" id="min0">
    <div class="node 00">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 01">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 10">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 11">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 20">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 21">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
</div>

<div class="cover middle marker">
    <div class="knob">
        <div class="inner"></div>
    </div>
    <div class="knob">
        <div class="inner"></div>
    </div>
</div>

<div class="digit" id="sec1">
    <div class="node 00">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 01">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 10">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 11">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 20">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 21">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
</div>

<div class="cover middle"></div>

<div class="digit" id="sec0">
    <div class="node 00">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 01">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 10">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 11">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 20">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
    <div class="node 21">
        <div class="edge first"></div>
        <div class="edge second"></div>
        <div class="knob">
            <div class="inner"></div>
        </div>
    </div>
</div>

<div class="cover after"></div>
<div class="clear"></div>
</div>

<div class="cover bottom"></div>

<div class="center">Inspired by <a href="http://www.artlebedev.com/everything/segmentus/">Segmentus</a>.</div>

<script type="text/javascript">
$(document).ready(function() {
    var map = {
        "0" : [4, 2, 0, 2, 4, 2, 0, 6, 4, 6, 6, 0],
        "1" : [4, 2, 0, 1, 2, 5, 0, 6, 0, 2, 6, 0],
        "2" : [4, 2, 0, 2, 2, 2, 1, 6, 5, 6, 6, 0],
        "3" : [4, 2, 2, 1, 5, 6, 1, 6, 5, 0, 6, 0],
        "4" : [4, 2, 0, 1, 5, 6, 0, 6, 0, 2, 6, 0],
        "5" : [4, 2, 2, 6, 4, 6, 0, 2, 0, 2, 2, 6],
        "6" : [4, 2, 1, 6, 5, 6, 0, 2, 4, 6, 2, 6],
        "7" : [4, 2, 1, 2, 5, 0, 6, 6, 0, 2, 6, 0],
        "8" : [0, 6, 0, 2, 6, 0, 0, 6, 2, 6, 6, 0],
        "9" : [0, 6, 0, 2, 2, 6, 1, 2, 2, 5, 6, 0]
    };

    var setDigit = function(digitId, val) {
        var dirs = map[val];
        $(digitId).find('.edge').each(function(index, el) {
            $(el).css('transform', 'rotateZ(' + (dirs[index] * 45) + 'deg)');
        });
    }

    var func = function() {
        var date = new Date();
        var hour = ("0" + date.getHours()).slice(-2);

        setDigit("#hour1", hour.slice(0,1));
        setDigit("#hour0", hour.slice(1,2));

        var min = ("0" + date.getMinutes()).slice(-2);

        setDigit("#min1", min.slice(0,1));
        setDigit("#min0", min.slice(1,2));

        var sec = ("0" + date.getSeconds()).slice(-2);

        setDigit("#sec1", sec.slice(0,1));
        setDigit("#sec0", sec.slice(1,2));

        $('.marker').toggleClass('blink');
    }

    setInterval(func, 1000);
});
</script>