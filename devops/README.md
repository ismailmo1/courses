# Devops Resources

My interest in devops mostly comes from improving my personal experience as a developer - and the concepts were discovered through trying to overcome some sort of pain. A clear example I can recall is after building [formpy](https://github.com/ismailmo1/formpy-app), I wanted to improve the codebase and do some refactoring. It had been a while since I last touched the codebase so it took me days to setup my own dev environment and from that I learnt about Docker, containerisation and how to make reproducible environments which made [deployment](formpy.ismailmo.com) a whole lot smoother too.

I haven't taken any courses (yet) so all of my learning is from blogs, documentation and YouTube:

<details>
<summary><b>Linux</b></summary>

I have an ubuntu instance from [linode](https://linode.com) and I host most of my work on there as containers, the whole setup uses nginx as a reverse proxy which itself runs in a container using a really cool [image from jwilder](https://github.com/nginx-proxy/nginx-proxy) that listens for new docker containers and adds them to the config. You can checkout how my linode instance is setup [here](https://github.com/ismailmo1/linode-config)

I used to run ubuntu for a while on my laptop but I now use windows subsystem for linux (WSL) so I know a bit of bash and like to think I know my way around the terminal a little bit (I'm no wizard though).

My favourite resources for linux stuff:

- [Linode guides](https://www.linode.com/docs/guides/)
- [Digital Ocean's community guides](https://www.digitalocean.com/community/tutorials)
- [Learn Linux TV](https://www.youtube.com/c/LearnLinuxtv)

</details>

<details>
<summary><b>Docker</b></summary>
I probably use docker for things where it's not really necessary and kind of overkill, but it makes things so much easier so I just containerise everything and haven't regretted it yet. Writing a dockerfile is pretty straightforward and using docker-compose to seamlessly deploy a full stack application with very little effort is a blessing.

I mostly just use the Docker documentation, but language/framework specific guides are available on VSCode's documentation also:

- [Docker docs](https://docs.docker.com/)
- [VSCode Language guides](https://code.visualstudio.com/docs/containers/overview)
- [VSCode devcontainers](https://code.visualstudio.com/docs/remote/containers-tutorial)

</details>

<details>
<summary><b>CI/CD</b></summary>
This is an area I definitely want to spend some more time learning, but for now I've been using github actions, mostly because it's convenient as I already host all my code on github.

I've used github actions to setup a CI/CD workflow in multiple projects:

- Automated tests and publishing for the [formpy library](https://github.com/ismailmo1/formpy/blob/master/.github/workflows/test_deploy.yml) on pypi
- Automated testing, docker image updating and deployment to my linode instance for [formpy's website](https://github.com/ismailmo1/formpy-app/blob/master/.github/workflows/deploy.yml)
- Same as above for the [mfp-wrapped website](https://github.com/ismailmo1/mfp-wrapped/blob/main/.github/workflows/docker-image.yml)

</details>
