> [!info]
>  This is the guidelines for formatting tags and other elements when writing HTML blog posts. 

## Tags

The HTML formatted blog posts will recognize most standard tags. 

If additional tags are required, these can be ‘allowed’ via the sanitize tag in Rails.
## Images

```
<div itemscope itemtype="https://schema.org/ImageObject">

     <img

       alt="alt text goes here"

       itemprop="contentUrl"

       src="https://bubblecow.com/assets/average-short-story-word-count"

       class="post-media img-fluid rounded mx-auto d-block mt-1 mb-1"

       width="700" height="400"

       />

     <span itemprop="creator" itemtype="https://schema.org/Person" itemscope>

       <meta itemprop="name" content="Gary Smailes" />

     </span>

   </div>
```
  
**Notes**:

- The use of ‘post-media’ is essential since it applies global formatting. 
- The use of ‘img-fluid’ is essential since it makes the image responsive. 
- The use of size (height/width) is essential and must not be missed out. To determine the size of an image. Add the image to the post, and then inspect the image in the browser to get the size. 
- The use of ‘mx-auto d-block’ centralizes the image, this can be left out if needed. 
- The use of ‘rounded’ in class is optional.
- Optimising:
	- https://www.iloveimg.com/compress-image
## Iframes

```
<video>

<div class="post-media ratio ratio-16x9">  
<iframe src="https://www.youtube.com/embed/zpOULjyy-n8?rel=0" title="YouTube video" allowfullscreen></iframe>  
</div>

</video>
```

**Notes**:
- The use of ‘post-media’ is essential since it applies global formatting. 
- The use of ‘ratio’ makes the iframe responsive and is essential, as is the ratio size. More information here: [https://getbootstrap.com/docs/5.1/helpers/ratio/#example](https://getbootstrap.com/docs/5.1/helpers/ratio/#example). This also counters CLS. 
## Table of Contents

TOCs are formatted from Bootstrap and custom CSS. 

Part 1:

```
<div class="toc card bg-light" id="toc">

 <p class="card-header"><strong>Table of Contents</strong></p>

  <div class="card-body">

    <ul>

      <li><a href="#item-1">Link 1</a></li>

      <li class="child-link"><a href="#item-1-1">Link 1-1</a></li>

    </ul>

  </div>

</div>
```

Part 2:

```
<div data-spy="scroll" data-target="#toc" data-offset="0">  
  <h2 id="item-1">Item 1</h2>  
  <p>...</p>  
  <h3 id="item-1-1">Item 1-1</h3>  
  <p>...</p>  
</div>
```
## FAQ

FAQ sections are formatted via Bootstrap and the theme CSS. They are also presented in a way that includes structured data. 

More information here: [https://developers.google.com/search/docs/advanced/structured-data/faqpage](https://developers.google.com/search/docs/advanced/structured-data/faqpage)

```

```

|   |
|---|
|<h2>Frequently Asked Questions</h2>  <br><p>Below are some frequently asked questions that will provide you with more information.</p><br><br>  <br><div itemscope itemtype="[https://schema.org/FAQPage](https://schema.org/FAQPage)" class="faq"><br><br><div itemscope itemprop="mainEntity" itemtype="https://schema.org/Question"><br><br><h3 itemprop="name">Question here</h3><br><br><div itemscope itemprop="acceptedAnswer" itemtype="https://schema.org/Answer"><br><br>   <div itemprop="text"><br><br>     <p>Answer here</p><br><br>   </div><br><br></div><br><br>  </div><br><br> </div>|

  
  

## Interlinking

These are links to include to link to sales pages.

### Developmental Editing

  

<div class="alert alert-info" role="alert">

<p>You can discover more about <a href="https://bubblecow.com/book-editing">developmental editing</a>, and how this can make you a better writer.</p>

</div>

### Copy Editing

  

<div class="alert alert-info" role="alert">

<p>You can discover more about <a href="https://bubblecow.com/copy-editing">copy editing</a>, and how this can help you prepare your book for publication.</p>

</div>

  

### Manuscript Assessment

  

<div class="alert alert-info" role="alert">

<p>You can discover more about our <a href="https://bubblecow.com/manuscript-assessment">manuscript assessment service</a>, and how this can help you prepare your book for the next step.</p>

</div>

  
  
  
**