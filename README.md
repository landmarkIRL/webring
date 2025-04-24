# LMU Webring

A community of personal sites from developers, designers, and digital creatives affiliated with Landmark University, past or present.

## What is a webring?

A [webring](https://en.wikipedia.org/wiki/Webring) is a group of websites linked together in a loop, centered around a shared interest or community. Each member site links to the next and previous ones, allowing visitors to browse through the network.

## How to Join

[Open a pull request](https://github.com/landmarkIRL/webring/compare) with your site’s name and URL. If you have an RSS feed, feel free to include that too.

Or You can sign up through the form on [our site](https://webring.landmarkirl.xyz/). Webring admins will review and process your request.

## This webring accepts

f you think you belong here, chances are you do. Developers, designers, and digital creatives from Landmark University, whether current students or alumni, are welcome. Being listed requires:

- A connection to Landmark University
- A personal website
- Using our webring code somewhere on your website

## Listing the webring on your site

Once accepted, add this snippet to your site:

```html
<webring-banner>
    <p>Member of <a href="{{ meta.url }}">{{ meta.title }}</p>
    <a href="{{ meta.url }}/prev">Previous</a>
    <a href="{{ meta.url }}/random">Random</a>
    <a href="{{ meta.url }}/next">Next</a>
</webring-banner>
<script async src="{{ meta.url }}/embed.js" charset="utf-8"></script>
```

This displays a banner that links to other webring members.
If you prefer to roll your own design, use the simpler HTML snippet below instead and style it however you'd like (as long as it’s accessible):

```html
<nav class="webring" aria-labelledby="webring">
  <h2 id="webring">LMU Webring</h2>
  <p>This site is part of <a rel="external" href="https://webring.landmarkirl.xyz/">LMU Webring</a>.</p>
  <ul>
    <li><a rel="external" href="https://webring.landmarkirl.xyz/prev">Previous website</a></li>
    <li><a rel="external" href="https://webring.landmarkirl.xyz/random">Random website</a></li>
    <li><a rel="external" href="https://webring.landmarkirl.xyz/next">Next website</a></li>
  </ul>
</nav>
```

## Webring Link Placement

You can place the webring banner or links on a subpage rather than the homepage, as long as it's accessible within **one click** from your landing page.

## Who made this?

Created by [David Umoru](https://davidumoru.me/), inspired by [Max Böck's webring project](https://github.com/maxboeck/webring).

## License

MIT
