# Summary of my test

## Getting Started

Getting strarted in the project had deemed a much more difficult task than I had envisioned. Beginning my setup process, I had followed the instructions for installing the Stencil CLI. On the final step, after installing and configuring Python and Node.js. I ran the final command to actually get the Stencil CLI, but was reciving an error.

```
throw err;
              ^ Error: Cannot find module 'npmconf'
```

My researech had been been unsuccessful, the only resource I could find was over 5 years old, and was referring to a depracticated module. Given the context, I took a step back and removed Node.js from my computer completely. Then reinstalled, thinking a clean Node enviroment could be the cause of the error. Attempted a install of the Stencil CLI, failed. Research. Attempted install of the Stencil CLI, failed. I fell into this cycle before I came to a conclusion. Local environments can be volatile.

---

## Learning DevOps

The only path I could see forward was to create an environment from scratch & use a technology that I had no previous expericne with, but had an interest in learning. Docker. I can tell you first hand, learning Docker is a pretty steep learning curve. I had no idea where to start, and ended up reading countless documentations plus watching hours of "What is Docker?" & "Docker for beginners videos".

A day and a half had passed, with little sleep. But, at this point, I had learned how to create a Docker Image that preinstalled Node, NPM & the Stencil CLI. I had learned that Docker is a super light weight OS layerd ontop of the Host OS's Kernal. And I had learned how to establish and SSH key with my GitHub and clone my test store repo directly into the Docker container, install dependancies and establish a TCP connection on a PORT of my choosing to ultimaelty view my store.

Feeling pretty good about myself, I moved onto the next tasks. Scaling the CodeBase provided by Big Commerce and make the changes assigned to me. What I had just realized will also be a steep learning curve.
