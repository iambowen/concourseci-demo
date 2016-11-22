### Requirements
- must use [virtualbox version >= 5.1](https://www.virtualbox.org)
- install [fly cli](https://concourse.ci/fly-cli.html)
- [example](http://danoncoding.com/programming/2015/12/17/setting-up-a-simple-pipeline-with-concourse-ci/)
### run
1. vagrant up

2. `fly -t lite login -c http://192.168.100.4:8080`

3. `fly -t lite set-pipeline -p hello-world -c hello.yml`

4. `fly -t lite unpause-pipeline -p hello-world`

5. `fly -t lite set-pipeline -p hello-world -c eventservice.yml` #play with event service
