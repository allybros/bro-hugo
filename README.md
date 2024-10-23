# Bro Hugo Theme

An elegant and basic Hugo theme for software development organizations, theme of (https://allybros.com). Although 
we developed this theme for our own site, we tried to make it generic enough to allow people to use for their own needs.
Feel free to use it on your projects and modify it.

## 🕹 Demo
This theme is specifically developed for Ally Bros official webpage, therefore you can try it out here: https://allybros.com

## 🌟 Features
- Modern home page with customizable sections
- Application cards to organize projects
- Easy to understand and change
- Using Bulma.css without dark mode, let us know if you made it work better with dark mode :)

## 📀 How to install
We will explain this once we can recommend this theme.

## ⚙️ Customizations

### Home Page
Your home page consist of 3 sections: intro, content and features.

##### Home Intro (home-intro)
In this section, bro theme utilizes your site config.toml file to populate content. 
- `description` Title of the intro section
- `hero_description` Paragraph within the hero section
- `hero_button_label` Text on the button in intro section, if you don't provide this field, there won't be any button on home intro
- `hero_button_link` The URL that the button will point to

#### Home Content (home-content)

This section rendered if you set up a home content. (Create an index_md in your content root)

#### Features(home-features)

Use following fields to configure your feature list.

- `features_title`  If you don't have the features title, features section is not rendered
- `features_subtitle` Sub title for the feature section

You need to provide an array of features as follows;

**Example**:
```
[[params.features]]
image = "/img/idea.svg"
title = "Ideation and Analysis"
description = "At Ally Bros, we constantly ideate and try to find solutions for daily life problems, perform analysis of feasibility and market."
```
### Section pages
Section pages can behave in two different ways, portfolio listing or content listing. This is controlled by existence of `portfolio = true` in your sections pagefront field.

### Content pages
Content pages can behave in two different ways, depending on existince of `appIcon` on your post pagefront, you will get a card that uses following fields;

- `sourceCodeLink`, `storeLink` and `externalLink` controls the buttons and their urls.
- `appIcon` is the logo for the content, which appears both on the portfolio and left side of the card.

To find out more, please refer to the example site.