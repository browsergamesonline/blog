---
layout: default
---

<section class="hero">

  <div class="container hero-content">

    <span class="hero-label">
      Browser Gaming
    </span>

    <h1>
      Discover Fun Browser Games
    </h1>

    <p>
      Discover fun online games across racing, action, puzzle, sports,
      multiplayer, adventure, and platform categories.
    </p>

    <a href="#articles" class="hero-button">
      Explore Articles
    </a>

  </div>

</section>


<section class="latest-articles" id="articles">

  <div class="container">

    <div class="section-title">

      <h2>
        Latest Articles
      </h2>

      <p>
        Explore our latest browser gaming guides and recommendations.
      </p>

    </div>


    <div class="article-grid">

      {% for post in site.posts %}

      <article class="article-card">

        <div class="article-date">
          {{ post.date | date: "%B %d, %Y" }}
        </div>

        <h3>
          <a href="{{ post.url | relative_url }}">
            {{ post.title }}
          </a>
        </h3>

        <p>
          {{ post.description }}
        </p>

        <a href="{{ post.url | relative_url }}" class="read-more">
          Read Article
        </a>

      </article>

      {% else %}

      <article class="article-card">

        <h3>
          Articles Coming Soon
        </h3>

        <p>
          New browser game articles will appear here soon.
        </p>

      </article>

      {% endfor %}

    </div>

  </div>

</section>
