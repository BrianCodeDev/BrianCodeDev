### Hi there <a href="https://briancodedev.org"><img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="5%"></a>
This is the place where I opensource stuff and break things :rofl:

- 🔭 &nbsp;I’m currently working on something cool. :wink:
- 🌱 &nbsp;I’m currently learning AWS, CI/CD pipeline.
- 💬 &nbsp;Ask me about anything related to Javascript/Typescript/Python or Java/React/Express/WebSockets/AWS.
- 👨‍💻 &nbsp;Read more about my projects at [briancodedev.org](https://briancodedev.org/projects).
- ⚡ &nbsp;Fun fact: I love coffee before anything.

# GitHub Action for generating a contribution graph with a snake eating your contributions.

name: Generate Snake

# Controls when the action will run. This action runs every 6 hours.

on:
  schedule:
      # every 6 hours
    - cron: "0 */6 * * *"

# This command allows us to run the Action automatically from the Actions tab.
  workflow_dispatch:

# The sequence of runs in this workflow:
jobs:
  # This workflow contains a single job called "build"
  build:
    # The type of runner that the job will run on
    runs-on: ubuntu-latest

    # Steps represent a sequence of tasks that will be executed as part of the job
    steps:

    # Checks repo under $GITHUB_WORKSHOP, so your job can access it
      - uses: actions/checkout@v2

    # Generates the snake  
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: BrianCodeDev
          # these next 2 lines generate the files on a branch called "output". This keeps the main branch from cluttering up.
          gif_out_path: dist/github-contribution-grid-snake.gif
          svg_out_path: dist/github-contribution-grid-snake.svg

     # show the status of the build. Makes it easier for debugging (if there's any issues).
      - run: git status

      # Push the changes
      - name: Push changes
        uses: ad-m/github-push-action@master
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          branch: master
          force: true

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          # the output branch we mentioned above
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
🔗 &nbsp;**Connect with me**
<p align="left">
<a href="https://briancodedev.org/about" target="blank"><img align="center" src="https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/dev-dot-to.svg" alt="briancodedev" height="30" width="40" /></a>
<a href="https://www.linkedin.com/in/brian-kelley-profile/" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="briancodedev" height="30" width="40" /></a>
  
### ✨&nbsp; About Me

Skilled Software Engineer with 3 years of self taught experience. Excels in maximizing web performance and creating customized solutions to expand my user experience.

```
  ____                  ____                      
 / __ \___  ___ ___    / __/__  __ _____________  
/ /_/ / _ \/ -_) _ \  _\ \/ _ \/ // / __/ __/ -_) 
\____/ .__/\__/_//_/ /___/\___/\_,_/_/  \__/\__/  
   _/_/                  __  __   _               
  / __/  _____ ______ __/ /_/ /  (_)__  ___ _     
 / _/| |/ / -_) __/ // / __/ _ \/ / _ \/ _ `/ _ _ 
/___/|___/\__/_/  \_, /\__/_//_/_/_//_/\_, (_|_|_)
                 /___/                /___/       
```

  
I create most of my open-source projects to solve the challenges I encounter in life, with many more still waiting to be addressed. I am embarking on a quest to find solutions for each one, one problem at a time.

<details>
<p>Open to collaborations and exciting projects, I'm eager to connect with fellow developers and tech enthusiasts. Let's build something amazing together!

Happy coding!</p>

</details>

