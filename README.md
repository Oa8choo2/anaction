# anaction

test a github action

[![pages-build-deployment](https://github.com/Oa8choo2/anaction/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/Oa8choo2/anaction/actions/workflows/pages/pages-build-deployment)

## steps

* mkdocs/docs/HPC -> original md files
* gent.yml -> file with jinja variables
* zdocs/docs -> md files after minijinja conversion  
   this is the same file you can see with te read option of zensical,  
   pointing to https://raw.githubusercontent.com/Oa8choo2/anaction/main/zdocs/docs/connecting.md  
* zdocs/site -> html files after build by zensical
* https://oa8choo2.github.io/anaction -> site hosting all files
  * https://oa8choo2.github.io/anaction/mkdocs/docs/HPC/connecting.md -> original md file
  * https://oa8choo2.github.io/anaction/zdocs/docs/connecting.md -> converted md file
  * https://oa8choo2.github.io/anaction/zdocs/site/connecting -> converted html version
  * https://oa8choo2.github.io/anaction/ -> final site [TOBE]


