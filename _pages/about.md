---
permalink: /
title: "👋 Hello Everyone I am Parthiv! Great to see ya 😀"
excerpt: "About me"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<link rel="stylesheet" href="/assets/css/ml-intro-card.css">

<div class="ml-intro-card">
  <h1 class="ml-intro-title">
    <span class="title-part1">Trust me, I'm a</span>
    <span class="title-part2">machine learning engineer.</span>
  </h1>
  
  <p class="ml-intro-description">
    I'm a CSE undergraduate from IIIT-Delhi who believes that if you can't explain your model to a five-year-old, you probably don't understand it yourself. I specialize in ML, DL, NLP and computer vision, but I'm also that person who likes overfitting beacuse it is just the model being too eager to please. I've dabbled in everything from Gaussian Mixture Models to neural networks, and I'm convinced that the best algorithms are the ones that work when you're not looking.  
  </p>
  
  <p class="ml-intro-attribution">~ I believe a decreasing loss curve is more pleasing then Sydney Sweeny.</p>
  
  <p class="ml-intro-tagline">Turning data into decisions, one epoch at a time 🧠 (ChatGPT)</p>
</div>

# My achievements

<link rel="stylesheet" href="/assets/css/achievement-cards.css">

<script>
function toggleCard(button) {
  const card = button.parentElement;
  const isExpanded = card.classList.contains('expanded');
  
  // Close all other expanded cards
  document.querySelectorAll('.achievement-card.expanded').forEach(expandedCard => {
    if (expandedCard !== card) {
      expandedCard.classList.remove('expanded');
      const btn = expandedCard.querySelector('.view-more-btn');
      if (btn) {
        btn.textContent = 'View More';
        btn.classList.remove('expanded');
      }
    }
  });
  
  // Toggle current card
  if (isExpanded) {
    card.classList.remove('expanded');
    button.textContent = 'View More';
    button.classList.remove('expanded');
  } else {
    card.classList.add('expanded');
    button.textContent = 'View Less';
    button.classList.add('expanded');
  }
}
</script>

<div class="achievement-cards-container">
  <div class="achievement-card">
    <div class="achievement-number">1</div>
    <p class="achievement-text">My biggest ever achievement was that, I was the highest scorer in 12th CBSE boards exams(94.2%) in my school and was 4th in 10th CBSE exams. This lay the foundation of never ending hardwork. This was like a foundation stone from where I never stopped working hard and took my academics very seriously.</p>
    <button class="view-more-btn" onclick="toggleCard(this)">View More</button>
  </div>
  
  <div class="achievement-card">
    <div class="achievement-number">2</div>
    <p class="achievement-text">In my college, We had many assignments but the Kaggle Challenges in our machine learning course were the most challenging. It was class about 170 students including B.TECH, M.TECH and PHDs. We were given a dataset[Google Speech Command Dataset] in which we had to predict the words said in the audio clips accurately. I ranked 11th in the entire batch with an accuracy of 89.78% on unseen testing data. You can see the leaderboard yourself <a href="https://www.kaggle.com/competitions/gaussian-mixture-models/leaderboard">here</a>. My id is Parthiv A Dholaria. We were told to only use Gaussian Mixture model for classification and No deep learning models/techniques which made it very challenging.</p>
    <button class="view-more-btn" onclick="toggleCard(this)">View More</button>
  </div>
  
  <div class="achievement-card">
    <div class="achievement-number">3</div>
    <p class="achievement-text">In another kaggle challenge on Human Activity Recognition from UCL. I ranked 17th in the entire batch with an accuracy of 59.798%. I had used KNN to get this accuracy. You can see the leaderboard rankings <a href="https://www.kaggle.com/competitions/unsupervised-learning-m2023/leaderboard">here</a>. My ID is Parthiv A Dholaria.</p>
    <button class="view-more-btn" onclick="toggleCard(this)">View More</button>
  </div>
  
  <div class="achievement-card">
    <div class="achievement-number">4</div>
    <p class="achievement-text">I am also privileged to be a part of two excellent clubs of my college. Firstly, GDSC i.e Google Developers student club. I developed interests in Web Development in the first and second years of my B.Tech and I was able to crack the interview by showcasing some of my projects in WebD. Secondly, Salt N' Pepper which is a food club of our college. The thing I like about this club is the ability to be creative from a very simple thing like food and make our audience feel happy and entertain them. I learned a lot from the events we conducted at Salt N' Pepper.</p>
    <button class="view-more-btn" onclick="toggleCard(this)">View More</button>
  </div>
</div>

<!-- # A data-driven personal website

Like many other Jekyll-based GitHub Pages templates, academicpages makes you separate the website's content from its form. The content & metadata of your website are in structured markdown files, while various other files constitute the theme, specifying how to transform that content & metadata into HTML pages. You keep these various markdown (.md), YAML (.yml), HTML, and CSS files in a public GitHub repository. Each time you commit and push an update to the repository, the [GitHub pages](https://pages.github.com/) service creates static HTML pages based on these files, which are hosted on GitHub's servers free of charge.

Many of the features of dynamic content management systems (like Wordpress) can be achieved in this fashion, using a fraction of the computational resources and with far less vulnerability to hacking and DDoSing. You can also modify the theme to your heart's content without touching the content of your site. If you get to a point where you've broken something in Jekyll/HTML/CSS beyond repair, your markdown files describing your talks, publications, etc. are safe. You can rollback the changes or even delete the repository and start over -- just be sure to save the markdown files! Finally, you can also write scripts that process the structured data on the site, such as [this one](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb) that analyzes metadata in pages about talks to display [a map of every location you've given a talk](https://academicpages.github.io/talkmap.html).

# Getting started

1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right.
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.
1. Check status by going to the repository settings, in the "GitHub pages" section

## Site-wide configuration

The main configuration file for the site is in the base directory in [\_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [\_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header.

## Create content & metadata

For site content, there is one markdown file for each type of content, which are stored in directories like \_publications, \_talks, \_posts, \_teaching, or \_pages. For example, each talk is a markdown file in the [\_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the \_talks directory).

**Markdown generator**

I have also created [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the academicpages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

## How to edit your site's GitHub repository

Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons.

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

## For more info

More info about configuring academicpages can be found in [the guide](https://academicpages.github.io/markdown/). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful. -->
