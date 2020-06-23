# issues to keep in mind for v2

- the image was created multiple times - before testing on travis CI and every time code was pushed from travis CI to elastic beanstalk. Web server should only be concered with being a web server and not building a image especially since it is the
  active running web server. Causes longer time for deployment after every succesful change to the master branch.
