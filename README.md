# LKE Hugo Test Site

Content of this repository is create following the
[How to Deploy a Static Site on Linode Kubernetes Engine](https://www.linode.com/docs/guides/how-to-deploy-a-static-site-on-linode-kubernetes-engine/)
article.

```zsh
hugo new posts/first_post.md
docker build -t carltonj2000/lke-example:v1 .
docker run -p 8080:80 -d carltonj2000/lke-example:v1
docker login
docker push carltonj2000/lke-example:v1
```
