Description
===========

A [Dashing](https://github.com/Shopify/dashing) widget for displaying data from Stripe

![](http://imgur.com/CdpGkHX.png)

Dependencies
============

You need an account with [Stripe](http://www.stripe.com) to use this.

Add to dashing's gemfile:
```
gem 'stripe'
```
and run`bundle install.

Usage
============

Add the widget HTML to your dashboard
```
    <li data-row="1" data-col="1" data-sizex="1" data-sizey="1">
      <div data-id="stripe_stats" data-view="StripeStats" data-title="Business Name"></div>
    </li>
```
Create a directory titled "stripe_stats" under your widgets directory and move stripe_stats.coffee, stripe_stats.html, and stripe_stats.scss into that directory.

Get your api key from Stripe by logging into stripe.com, clicking on your business name in the top right, and selecting account settings. Click on API Keys and use your secret key.

Modify the api key in the stripe_stats.rb file.

Move stripe_stats.rb into your jobs folder.
