# Docs

**Start publishing with Datahub Cloud!**

# Quick Start Guide

At the end of this tutorial, you'll know how to use DataHub Cloud to turn datasets and data-driven content on GitHub into a published, shareable site.

> Note: While our tutorial focuses on publishing a dataset, with a few tweaks, you can turn this into an engaging data story.

## Start out from our template 

- Go to [Datahub Cloud Template](https://github.com/new?template_name=datahub-cloud-template&template_owner=datahubio)
- Give your new repository a name
- You can make it either public or private - it works with both
- Create the repository
- Done! This is what it should look like:

![[Screenshot-repo.png]]

- Now that you've got your own copy, it's time to publish it with Datahub Cloud

### Understanding the template

The template repository you just created contains the following files:
- The data.csv
- README.md which has: 
  - Structured data: Frontmatter with Frictionless data package spec in the `datapackage` field. It describes the data file(s) in the repository (in this case, the `data.csv`). 
  - Unstructured data: Below the frontmatter, you can add a description / free text in markdown format

> Note: If you want to edit the README, refer to the [Frictionless data package spec](https://specs.frictionlessdata.io/data-package/). 

## Sign up 

If you have your invite link head over and sign up.

If you don't yet have an invite, please [sign up for early access here](https://tally.so/r/wad1O2) - we're onboarding people as quickly as possible.

## Publish your dataset

- Click on "Create New Site" and follow the steps
> Note: Make sure to choose the GitHub repository you just created.
- This was quite quick, right?
- Now, hit "Visit" and let's see what it looks like:

![[Dataset page part 1.png]] 

![[Dataset page part 2.png]] 

You are ready to roll! 

Now you can either enhance this dataset or try publishing your own dataset (continue reading).

> Note: To ensure that your site displays the most recent version of your GitHub repository, simply click on the "Sync" button within Datahub Cloud App. This allows you to manage updates according to your preferences before making them public.

## Enhancing your dataset

Start populating your new repository with data. Enhance your content with other data visualisation components and markdown features. Update your README using Markdown to provide insights into your dataset. Let your data tell its story!

- For a full list of supported markdown features visit https://flowershow.app/docs/syntax
- For a full list and API of available data visualisation components visit [https://storybook.portaljs.org](https://storybook.portaljs.org/)

## Try Datahub Cloud with your own dataset

Do you have an existing dataset on Github that you want to publish with Datahub Cloud? 

- Navigate to Datahub Cloud 
- Create a new site
- Publish your dataset by choosing your dataset repository
- Done! Click "Visit" to see the outcome
- Show off the URL of your dataset here https://github.com/datahubio/datahub/discussions/305
- If something isn't rendering properly or there is an issue with your dataset being published, make sure to report it at support@datahub.io

## Feedback and Contribution

- Please share your feedback or ideas for improvement by opening a discussion here https://github.com/datahubio/datahub/discussions
- If you want to contribute and help improve Datahub Cloud, you can write a react component, we import it and it's done! This way, you get to shape your own experience.

## Have questions?

If you have a question, please ping us on [Discord](https://discord.gg/wzvSgGDt) or send us an email at support@datahub.io

