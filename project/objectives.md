# Constraining Galactic Structure with Simulation Based Inference

## Project Objectives

### 0. Logging research progress

   **Status: Ongoing**
   
   *Learning objective*: Recognize the importance of tracking research objectives, progress, and questions.

   *Criteria for success*: Keep organized, meticulous notes of your research.

   <details>
   The most important part of the research process is probably being able to effectively communicate about the project. This means being able to explain to a random stranger on the street what you're doing, why it's important, and what it means. This is only possible if YOU know what you're doing. To this end, I ask that you keep diligent notes about everything you do related to this project. These notes don't have to be in any specific format, although it would be useful if they were saved in some what that I could also access them (like a google doc). Keep a record of what you do (e.g., I read this paper, I wrote a program that does this, I got confused about this topic, etc.), keep a record of what you want to do next (e.g., I need to write a program that does this other thing, I need to read about this topic, etc.), and, most importantly, keep track of all of the questions that come up (what does this acronym mean, how does this physical thing relate to this other physical thing, etc.). These notes will be invaluable to you as you work on the project. I often get distracted by other tasks and come back to a project after a few days or weeks only to have forgotten what exactly I was doing and what I needed to do next. Without these notes, I would have been lost!
   </details>

### 1. Start writing the "paper"

   **Status: Ongoing**

   *Learning objective*: Develop effective written communication skills

   *Criteria for success*: Start a draft of the introduction/background section of a "paper"

   <details>
   I hope that this project will ultimately result in a publication, but no matter what it will benefit YOU to start writing a "paper" or "final report" for the project right now, before you do anything else. In particular, I want you to focus on the "introduction" section of a paper, where you outline the major research questions and goals of the project. This will immensely benefit you because it will be something that you can look back on when you're knee-deep in data analysis and programming and you've forgotten what the "big picture" of the research project is. Don't worry about the formatting, the specific content, or anything like that now. Just write a paragraph or two about the project, and go back and read/edit it once in a while as you develop a stronger grasp on our research objectives. And it's OK if you don't know what the research questions/goals are yet - that's something we can talk about, which will guide your writing!
   </details>

### 2. Background research

   **Status: Ongoing**

   *Learning objective*: Develop a basic physical understanding of the algorithms and data sets that we'll be working with.

   *Criteria for success*: Be able to describe "simulation based inference" and the components of our model at a basic level

   <details>
   The first step for any project is to understand what's been done before. In this case, other people have figured out everything we need to know about the physics and algorithms. Here are some resources to get you started, although I hope you will do your own internet-searches to fill in the gaps and answer some questions. Take note of any questions or confusing topics that you come across along the way, and we can talk about them together.

   * Wikipedia: https://en.wikipedia.org/wiki/Milky_Way
   * The WISE Catalog of Galactic HII Regions. This paper provides an overview of the dataset that we'll be using. https://ui.adsabs.harvard.edu/abs/2014ApJS..212....1A/abstract
   * Simulation based inference: https://www.pnas.org/doi/10.1073/pnas.1912789117
   * Trigonometic Parallaxes of High-mass Star-forming Regions: in this paper, the authors are able to measure the distances and kinematics of some star forming regions in order to map out some of the structures that we're looking for. It's not directly related to this project, but it covers many of the topics that will be relevant to our work (Galactic rotation, spiral structure, etc.). https://ui.adsabs.harvard.edu/abs/2019ApJ...885..131R/abstract
   </details>

### 3. Preparing your research environment.

   **Status: Complete**

   *Learning objective*: Prepare software environment

   *Criteria for success*: Fork `galstruct` repository, submit a pull request

   <details>
   We're going to be writing some code for this project! In particular, we will be collaborating on a software package: https://github.com/tvwenger/galstruct

   Learn how to use Github to fork a repository, make changes on a branch, commit those changes, and submit them as a pull request to the repository.
   </details>

### 4. Understanding the `galstruct` model

   **Status: Complete**

   *Learning objective*: Understand the components of the `galstruct` model

   *Criteria for success*: Generate simulated longitude-velocity diagrams using `galstruct`

   <details>
   It's time to dig in to `galstruct`! To get started, familiarize yourself with the `galstruct` model: https://github.com/tvwenger/galstruct/tree/master/galstruct/model

   Create a list of the model parameters, learn how the model parameters are related to the model, and run `simulator.py` to generate synthetic HII region datasets from the model.

   Investigate the code and develop a firm understanding of how it works. Try to run it and keep notes about what is working and isn't working. Feel free to make pull requests to update the code as necessary!
   </details>

### 5. Simulation Based Inference

    **Status: Complete**

    *Learning objective*: Learn how to use the python package `sbi`

    *Criteria for success*: Run the `galstruct` `learn_likelihood.py` program

    <details>
    We're going to use the python package `sbi` for this project. Here is a link to the documentation: https://sbi-dev.github.io/sbi/latest/

    Familiarize yourself with this software, and take notes about what parts you understand or do not understand so we can discuss them.

    Ultimately, you will need to update the `learn_likelihood.py` program to work with the latest version of `sbi`. See what you can do, and we'll work on it together!
    </details>

### 6. Preparing for MCMC

    **Status: New**

    *Learning objective*: Learn about MCMC

    *Criteria for success*: Run the `galstruct` `mcmc_posterior.py` program

    <details>
    Now that we've got `learn_likelihood.py` working, we have to get
    `mcmc_posterior.py` working! Read about MCMC and work through some of the
    tutorials here: https://www.pymc.io/welcome.html

    I've gotten `mcmc_posterior.py` working, but we'll need to test it!
    Try generating a neural network output from `learn_likelihood.py`
    and then run it through `mcmc_posterior.py` and see what happens!
    I recommend limiting your tests to a single spiral arm for now. Keep notes
    about what works and doesn't work, what you understand and don't understand,
    and we'll address them next time!

    (Note, you might have to update your fork of `galstruct`!)
    </details>

