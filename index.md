---
layout: 'page'
---
<div class="header">
  <div class="container">
    <div class="grid-row padding-vertical">
      <div class="grid-col--1">
        <img src="/assets/fastly_logo_white.svg" class="fastly-logo">
      </div>
      <div class="grid-col--1 text-xs-right">
        <a href="https://www.fastly.com/signup" class="button action button-lg">Try Fastly for Free</a>
      </div>
    </div>
    <div class="grid-row">
      <div class="grid-col--1 header-text">
        <h1>Fastly Real-time Analytics</h1>
        <p>
          As a CDN, we’re in a unique position to view traffic patterns on
          the web. Fastly powers tens of thousands of websites, including
          top publishers and social media platforms like BuzzFeed, Vox&nbsp;Media,
          Twitter, Wenner&nbsp;Media, and Condé&nbsp;Nast, giving us key insights into
          how users react to the debate online – and this year’s election is
          clearly driving record levels of online engagement.
        </p>
      </div>
    </div>
  </div>
</div>
<div class="container">
  <div class="grid-row">
    <div class="grid-col--1 navigation padding-vertical">
      <div class="unit"><a href="#" data-link="ferns">Between Two Ferns</a></div>
      <div class="unit"><a href="#" data-link="debate1">First Debate</a></div>
      <div class="unit"><a href="#" data-link="debate2">Second Debate</a></div>
      <div class="unit"><a href="#" data-link="debate3">Third Debate</a></div>
      <div class="unit"><a href="#" data-link="election">Election Day</a></div>
    </div>
  </div>
  <div class="grid-row">
    <div class="grid-col--1 padding-vertical">
      <div class="timeline" data-content="ferns">
        <h1>Ferns</h1>
        <div data-timeline="ferns" class="endcap">Start</div>
        <div class="unit">Timeline 1</div>
        <div class="unit">Timeline 2</div>
        <div class="unit">Timeline 3</div>
        <div class="unit">Timeline 4</div>
        <div data-timeline="debate1" class="endcap">end</div>
      </div>
      <div class="timeline hidden" data-content="debate1">
        <h1>Debate 1</h1>
        <div data-timeline="ferns" class="endcap">Start</div>
        <div class="unit">Timeline 1</div>
        <div class="unit">Timeline 2</div>
        <div class="unit">Timeline 3</div>
        <div class="unit">Timeline 4</div>
        <div data-timeline="debate2" class="endcap">end</div>
      </div>
      <div class="timeline hidden" data-content="debate2">
        <h1>Debate 2</h1>
        <div data-timeline="ferns" class="endcap">Start</div>
        <div class="unit">Timeline 1</div>
        <div class="unit">Timeline 2</div>
        <div class="unit">Timeline 3</div>
        <div class="unit">Timeline 4</div>
        <div data-timeline="debate2" class="endcap">end</div>
      </div>
      <div class="timeline hidden" data-content="debate3">
        <h1>Debate 3</h1>
        <div data-timeline="ferns" class="endcap">Start</div>
        <div class="unit">Timeline 1</div>
        <div class="unit">Timeline 2</div>
        <div class="unit">Timeline 3</div>
        <div class="unit">Timeline 4</div>
        <div data-timeline="debate2" class="endcap">end</div>
      </div>
      <div class="timeline hidden" data-content="election">
        <h1>Election Day</h1>
        <div data-timeline="ferns" class="endcap">Start</div>
        <div class="unit">Timeline 1</div>
        <div class="unit">Timeline 2</div>
        <div class="unit">Timeline 3</div>
        <div class="unit">Timeline 4</div>
        <div data-timeline="debate2" class="endcap">end</div>
      </div>
    </div>
  </div>
</div>
<script>
$("a[data-link]").click(function(){
  $('.timeline').addClass('hidden');
  value = $(this).attr('data-link');
  $("div[data-content='"+value+"']").removeClass('hidden');
});
</script>
