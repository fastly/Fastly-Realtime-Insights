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
<div class="main-content container">
  <div class="grid-row">
    <div class="grid-col--1 navigation padding-vertical">
      <div class="unit"><a href="#ferns" data-link="ferns">Between Two Ferns</a></div>
      <div class="unit"><a href="#debate1" data-link="debate1">First Debate</a></div>
      <div class="unit"><a href="#debate2" data-link="debate2">Second Debate</a></div>
      <div class="unit"><a href="#debate3" data-link="debate3">Third Debate</a></div>
      <div class="unit"><a href="#election" data-link="election">Election Day</a></div>
    </div>
  </div>
  <div class="grid-row">
    <div class="grid-col--1 padding-vertical">
      <div class="timeline" data-content="ferns">
        <h1>Between Two Ferns with HRC</h1>
        <div class="unit">
          <p>
            When Emmy Award-winning comedy website Funny Or Die aired their
            popular “Between Two Ferns” interview with Hillary Clinton on
            September 22, 2016, the video was retweeted over 28,000 times,
            their site saw an increase in online traffic of over 1,000% —
            double the amount of requests they saw after airing the 2014
            interview with Barack Obama.
          </p>
        </div>
        <div class="unit">
          <p>
            The video was viewed more than 30 million times during the first
            24 hours (breaking their previous viewership records as the highest
            first-day viewership in Funny Or Die history).
          </p>
        </div>
        <a href="#" data-link="debate1" class="endcap">The First Presidential Debate</a>
      </div>
      <div class="timeline hidden" data-content="debate1">
        <h1>
          Spikes of up to 3,000% to sites with fact checkers during the first
          debate
        </h1>
        <ul>
          <li>On average, traffic to media sites increased 63% between 8:40 and 10:50 PM ET</li>
          <li>An hour before the debate began, traffic to hillaryclinton.com was up by almost 140% versus the same time last week, and spiked by 6,500% after the debate started.</li>
          <li>Traffic to hillaryclinton.com surged during the debate as viewers reacted to both candidates, spiking most notably when viewers were first directed to Clinton’s website, with an increase of 4,600%.</li>
        </ul>
        <a data-link="ferns" class="endcap">Between Two Ferns with HRC</a>
        <div class="unit">
          9:16 PM EDT 22% increase in media traffic when Trump claimed he “did not say” climate change is a Chinese hoax
        </div>
        <div class="unit">
          9:49 PM EDT 20% increase in media traffic when Lester Holt interrupted the debate to clarify that courts declared stop-and-frisk illegal
        </div>
        <div class="unit">
          9:44 PM EDT Traffic to hillaryclinton.com went up again when the race segment of the debate began, going up about three times normal traffic.
        </div>
        <div class="unit">
          9:58 PM EDT Traffic to hillaryclinton.com went up by 3x again when Trump mentioned that Clinton “chose to stay home” and she responded that she prepared for the debate, and “to be president.”
        </div>
        <div class="unit">
          After the debate ended, traffic to hillaryclinton.com remained high, with requests at 2,000% above normal.
        </div>
        <a data-link="debate2" class="endcap">The Second Presidential Debate</a>
      </div>
      <div class="timeline hidden" data-content="debate2">
        <h1>Sustained traffic to media sites during second debate</h1>
        <a data-link="debate1" class="endcap">The First Presidential Debate</a>
        <div class="unit">
          9:08 PM EDT: a 250% spike when Clinton answered the very first question about education funding and reform
        </div>
        <div class="unit">
          9:27 PM EDT: a 100% spike when Trump said he would get a special prosecutor to investigate Clinton
        </div>
        <div class="unit">
          10:07 PM EDT: a 256% spike when Trump discussed Clinton's tax reform efforts in the Senate, saying he understood the tax code better than anyone
        </div>
        <div class="unit">
          10:07 PM EDT: a 256% spike when Trump discussed Clinton's tax reform efforts in the Senate, saying he understood the tax code better than anyone
        </div>
        <a data-link="debate3" class="endcap">The Final Presidential Debate</a>
      </div>
      <div class="timeline hidden" data-content="debate3">
        <h1>Major moments of engagement dropped by 83% during third and final debate</h1>
        <a data-link="debate2" class="endcap">The Second Presidential Debate</a>
        <div class="unit">
          9:38 PM EDT: a 500% spike when Trump claimed that Clinton “wanted the wall.”
        </div>
        <div class="unit">
          10:12 PM EDT: a steady, 350% increase while Clinton discussed her foreign policy
        </div>
        <div class="unit">
          10:35 PM EDT: a 67% increase as compared to normal as viewers checked out media sites post debate
        </div>
        <a data-link="election" class="endcap">Election Day</a>
      </div>
      <div class="timeline hidden" data-content="election">
        <h1>Election Day</h1>
        <a data-link="debate3" class="endcap">The Final Presidential Debate</a>
        <div class="unit">
        </div>
        <div class="unit">
        </div>
        <div class="unit">
        </div>
        <div class="unit">
        </div>
        <a href="/signup" class="endcap">Add Fastly to your timeline.</a>
      </div>
    </div>
  </div>
</div>
<script>
$(document).ready(function(){
  if(window.location.hash) {
    setTimeline(window.location.hash.split('#')[1]);
  }
});
$("a[data-link]").click(function(e){
  e.preventDefault();
  setTimeline($(this).attr('data-link'));
  scrollToTop();
});
function setTimeline(value){
  $('.timeline').addClass('hidden');
  $("div[data-content='"+ value +"']").removeClass('hidden');
}
function scrollToTop(){
  $("html, body").animate({
    scrollTop: $('.main-content').offset().top
  });
}
</script>
