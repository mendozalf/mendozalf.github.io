project: 
  type: website

website:
  title: "Luis Fernando Mendoza Data Science Portfolio"
  favicon: Images/favicon.png
  back-to-top-navigation: true
  repo-url: https://github.com/mendozalf/mendozalf.github.io
  #repo-actions: [issue] #if you want to allow others to report issues on your site uncomment this line

  page-footer: 
    border: true
    left: "Luis Fernando Mendoza"
    right: 
      - icon: linkedin
        href: https://www.linkedin.com/in/lf-mendoza/

  navbar:
    background: primary
    search: true   
    right:
      - text: "Home"
        file: index.qmd
      - text: "DS250 Projects"
        file: projects.qmd
      - text: "My Resume"
        file: resume.qmd
      - text: "Data Cleansing"
        file: cleansing.qmd
      - text: "Data Exploration"
        file: exploration.qmd
      - text: "Story Telling"
        file: story_telling.qmd
      - text: "Machine Learning"
        file: ml.qmd
      - text: "Full Stack"
        file: full_stack.qmd
      - text: "Competition"
        file: competition.qmd
      
  sidebar:
    - title: "DS 250 Projects"
      style: "docked"
      background: light
      contents:
        - text: "DS250 Projects"
          file: projects.qmd
        - text: "---"
        - text: "Project 1"
          file: Projects/project1.qmd
        - text: "---"
        - text: "Project 2"
          file: Projects/project2.qmd
        - text: "---"
        - text: "Project 3"
          file: Projects/project3.qmd
        - text: "---"
        - text: "Project 4"
          file: Projects/project4.qmd
        - text: "---"
        - text: "Project 5"
          file: Projects/project5.qmd
        - text: "---"
        #continue the pattern if you need more links
        #copy paste from title and keep it indented to sidebar to add additonal sidebar navigation for other pages

format:  
  html:
    theme: #see this link to customize the theme with css (https://quarto.org/docs/output-formats/html-themes.html#dark-mode)
      light: flatly # more themes can be found [here](https://quarto.org/docs/output-formats/html-themes.html)
      dark: darkly
      #light: cosmo
      #dark: [cosmo, theme-dark.scss]
    css: styles.css
    toc: true
