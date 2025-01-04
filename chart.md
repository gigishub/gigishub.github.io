---
layout: default
title: TradingView Chart
---

## Live TradingView Chart

<div class="tradingview-widget-container">
  <div id="tradingview_12345"></div>
  <script type="text/javascript" src="https://s3.tradingview.com/tv.js"></script>
  <script type="text/javascript">
    new TradingView.widget(
    {
      "width": 980,
      "height": 610,
      "symbol": "NASDAQ:AAPL",
      "interval": "D",
      "timezone": "Etc/UTC",
      "theme": "light",
      "style": "1",
      "locale": "en",
      "toolbar_bg": "#f1f3f6",
      "enable_publishing": false,
      "allow_symbol_change": true,
      "container_id": "tradingview_12345"
    }
    );
  </script>
</div>

## Latest Posts

{% for post in site.posts limit:3 %}
  - [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}