# Summary of my test

## Getting Started

Getting started in the project had deemed a much more difficult task than I had envisioned. Beginning my setup process, I had followed the instructions for installing the Stencil CLI. On the final step, after installing and configuring Python and Node.js, I ran the final command to actually get the Stencil CLI, but was reciving an error.

```
throw err;
              ^ Error: Cannot find module 'npmconf'
```

My research was unsuccessful. The only resource I could find was over 5 years old, and was referring to a depracticated module. Given the context, I took a step back and removed Node.js from my computer completely. Then I reinstalled, thinking a clean Node enviroment could be the cause of the error. I attempted an install of the Stencil CLI, which failed. Research. Attempted install of the Stencil CLI, failed. I fell into this cycle before I came to a conclusion. Local environments can be volatile.

---

## Learning DevOps

The only path I could see forward was to create an environment from scratch & use a technology that I had no previous experience with, but had an interest in learning, Docker. I can tell you firsthand, learning Docker is a pretty steep learning curve. I had no idea where to start, and ended up reading countless documentations plus watching hours of "What is Docker?" & "Docker for beginners" videos.

A day-and-a-half had passed, with little sleep. But at this point, I had learned how to create a Docker Image that preinstalled Node, NPM & the Stencil CLI. I had learned that Docker is a super light weight OS layerd on top of the Host OS's Kernal. And I had learned how to establish and SSH key with my GitHub and clone my test store repo directly into the Docker container, install dependancies, and establish a TCP connection on a PORT of my choosing to ultimately view my store.

Feeling pretty good about myself, I moved onto the next tasks: scaling the CodeBase provided by Big Commerce, and making the changes assigned to me, which I realized would also be a steep learning curve.

## Scaling Big Commerce Theme

I had a outline of what was expected of me. Add button, delete button, make them work with feedback. There was a bonus of customer details displayed on the category page. I was not familiar with the file structure. I had used Handlebars before, but not on this scale. So I started getting an idea of what I could do, just using the Big Commerce Page Builder. I inserted an HTML widget, then built out a few buttons to the size and position that I wanted using the provided theme CSS & flexbox positioning. I realized I could write custom JavaScript inside of a `<script>` element, then built upon that. I used DOM manipulation to change text content and color, and I was able to give the user feedback on what action was to take place.

From here, I wanted to transtion out of the Page Builder and actually use the theme in my Docker container. I remembered that you could export the theme from `Storefront > My Themes` in the Big Commerce managment GUI. I exported my theme using my local computer, I created a new branch and cherry-picked the files I wanted to replace, and pushed it to GitHub. Then, inside of my Docker container, pulled the new branch so I could use the Docker Evironment to display my theme. Unfortunately, it does not export widgets from the Page Builder, but I didn't have to restart. I was able to grab the code from the Page Builder, then paste it right under the breadcrumbs in the export.

Satisfied with my buttons and user feedback, I began working on the API. The documentation was pretty clear about how to implement certain functionality, but I was receiving errors about `Same-Site`, `Secure`, & `Http` back from the API when I was sending requests. But I did successfully pull the item IDs off the items on the page, then use a `.forEach` to actually add items to the cart.

## Conclusion

I am not fully satisfied with my final results as far as the custom components in the theme go. Learning Docker took up much of my time, but because I don't have the option of using another environment, I found it essential to use the provided CLI. I have learned a lot about Handlebars & coding on a production code base. I have made a lot of progress in the last four days, given how little time I actually had to work on it. Even if I am not deemed a viable candidate, I would like to thank my reviewer for pushing me to learn and adapt in a short amount of time. Given I do not want to push the time allotted, I have turned in what I completed.

Thank you for your time and consideration.
