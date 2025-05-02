---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a Ph.D. candidate in Electrical and Computer Engineering at the [University of Maryland, College Park](https://ece.umd.edu/), working with [Prof. Shuvra S. Bhattacharyya](https://user.eng.umd.edu/~ssb/) in the [Maryland DSPCAD Research Group](https://code.umd.edu/dspcad-pub/dspcadwiki/-/wikis/Maryland-DSPCAD-Research-Group). I received my M.S. degree from the [Graduate Institute of Electronics Engineering](https://giee.ntu.edu.tw/en/home/) at National Taiwan University, where I was advised by [Prof. Liang-Gee Chen](https://www.ee.ntu.edu.tw/profile1.php?id=26) in the [DSPIC Lab](https://homepage.ntu.edu.tw/~lgchen/index.html). I earned my B.S. degree in Electrical Engineering from [National Taiwan University](https://web.ee.ntu.edu.tw/eng/index.php).

Research
======
Like many other Jekyll-based GitHub Pages templates, Academic Pages makes you separate the website's content from its form. The content & metadata of your website are in structured markdown files, while various other files constitute the theme, specifying how to transform that content & metadata into HTML pages. You keep these various markdown (.md), YAML (.yml), HTML, and CSS files in a public GitHub repository. Each time you commit and push an update to the repository, the [GitHub pages](https://pages.github.com/) service creates static HTML pages based on these files, which are hosted on GitHub's servers free of charge.

Many of the features of dynamic content management systems (like Wordpress) can be achieved in this fashion, using a fraction of the computational resources and with far less vulnerability to hacking and DDoSing. You can also modify the theme to your heart's content without touching the content of your site. If you get to a point where you've broken something in Jekyll/HTML/CSS beyond repair, your markdown files describing your talks, publications, etc. are safe. You can rollback the changes or even delete the repository and start over - just be sure to save the markdown files! Finally, you can also write scripts that process the structured data on the site, such as [this one](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb) that analyzes metadata in pages about talks to display [a map of every location you've given a talk](https://academicpages.github.io/talkmap.html).

Preprints
======
<div style="display: flex; align-items: flex-start; margin-bottom: 20px; position: relative;">
  <img src="/images/autocompose.jpg" alt="AutoComPose" style="width: 150px; height: auto; margin-right: 20px; border-radius: 4px;" class="original-image">
  <div>
    <h3 style="margin: 0; font-size: 0.8em;">
      AutoComPose: Automatic Generation of Pose Transition Descriptions for Composed Pose Retrieval Using Multimodal LLMs
    </h3>
    <p style="margin: 5px 0; font-size: 0.8em;">
      <strong>Yi-Ting Shen*</strong>, Sungmin Eum*, Doheon Lee, Rohit Shete, Chiao-Yi Wang, Heesung Kwon, and Shuvra S. Bhattacharyya (* equal contribution)
      <br>
      <a href="https://arxiv.org/abs/2503.22884">[arXiv]</a>
    </p>
    <p style="margin: 0; font-size: 0.8em;">
      We introduce AutoComPose, the first framework to automatically generate pose transition annotations using multimodal large language models, significantly improving composed pose retrieval performance while reducing reliance on costly human labeling.
    </p>
  </div>
  <img src="/images/autocompose.jpg" alt="AutoComPose Enlarged" class="hover-enlarge">
</div>

<style>
/* Add this CSS to your page or a linked stylesheet */
.original-image {
  z-index: 1;
}

.hover-enlarge {
  display: none;
  position: absolute;
  top: 0;
  left: 160px; /* Adjust to position beside the original image */
  width: 300px; /* Adjust size for enlargement */
  height: auto;
  border: 2px solid #ccc; /* Optional: Add a border for better visibility */
  background: white; /* Optional: Add a background to avoid overlap issues */
  z-index: 10; /* Ensure it appears above other elements */
  transition: transform 0.3s ease;
}

div:hover .hover-enlarge {
  display: block;
  transform: scale(1); /* No additional scaling needed */
}
</style>

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

The repository includes [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the Academic Pages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring Academic Pages can be found in [the guide](https://academicpages.github.io/markdown/), the [growing wiki](https://github.com/academicpages/academicpages.github.io/wiki), and you can always [ask a question on GitHub](https://github.com/academicpages/academicpages.github.io/discussions). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful.
