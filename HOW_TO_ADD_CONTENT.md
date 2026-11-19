# How to add content

This site is a Jekyll site using the [Academic Pages](https://github.com/academicpages/academicpages.github.io) theme. You edit text files, then GitHub Pages rebuilds the website. You do not need to write HTML for a normal update.

Preview on your own computer first. The commands are in `README.md`.

## Replace the profile photo

The sidebar uses one file:

`images/profile.jpg`

1. Save the new photo with exactly that name and put it in the `images` folder, replacing the old file.
2. A square picture works best. 600 by 600 pixels, or larger, is enough. The theme shows it in a circle about 175 pixels wide on a desktop.
3. Leave this line in `_config.yml` as it is, unless you change the filename:

```yaml
avatar: "profile.jpg"
```

If you do rename the file, change `profile.jpg` in that line to the new name.

`images/profile-original.jpg` is the untouched headshot, if it is present. The site does not show that file. It is only a spare copy.

## Add or edit a publication

Each paper is one Markdown file in `_publications/`. The filename starts with a date so the newest papers stay at the top, for example `_publications/2026-11-03-aftbody-vortex-shedding.md`.

Copy an existing file and change the fields. The fields that matter:

| Field | What to put |
| --- | --- |
| `title` | The paper title, exactly |
| `date` | `YYYY-MM-DD`. This sets the sort order |
| `year` | The year to print, if it should differ from `date` |
| `venue` | Journal or conference name |
| `category` | `manuscripts` for a journal, `conferences` for a conference, `under_review` for a manuscript still in review |
| `status` | `under-review` for a manuscript still in review. Leave it out for a published paper |
| `paperurl` | `https://doi.org/...` when a DOI exists |
| `authors_html` | Authors in order. Wrap your own name as `<strong class="author-me">Hamdoon Ijaz</strong>` |
| `citation` | The line that appears on the CV |
| `permalink` | A short web address, such as `/publication/short-name` |

A paper under review has `category: under_review` and `status: under-review`. Add `review_label` if the status is more specific than “Under review”, for example `Revised manuscript under review`. Leave `paperurl` empty until there is a DOI. The Ocean Engineering manuscript is `_publications/2026-11-19-ocean-engineering-under-review.md`.

Below the `---` block, write a few sentences in your own words. That text is the paper’s page on the site. The list of papers uses the fields above, not this paragraph.

## Add a project, with figures

1. Create a folder for the pictures, for example `images/projects/my-project/`.
2. Copy `_portfolio/wave-metamaterials.md` to `_portfolio/my-project.md`.
3. Change `title`, `excerpt`, `permalink`, and the text.
4. Put each figure in the folder you created. JPEG or PNG. About 1600 pixels wide is enough for the main column, and a few hundred kilobytes is plenty.

The page shows a dashed box until the image file exists. On the next build, the box becomes the picture. The path in the page and the path on disk must match, including capital letters.

This is the theme’s normal image syntax, if you would rather write the picture yourself instead of using the dashed box:

```markdown
![Flow at 50 degrees angle of attack](/images/projects/my-project/figure-1.jpg)

*Figure 1. One sentence saying what the reader is looking at.*
```

The address starts with `/images/...`. Alt text is the words in the square brackets. The caption is the italic line under the image.

The dashed-box version, which switches to the real image when the file is there:

```liquid
{% include media-slot.html
   path="/images/projects/my-project/figure-1.jpg"
   alt="Flow at 50 degrees angle of attack"
   label="Figure 1"
   caption="Figure 1. One sentence saying what the reader is looking at."
%}
```

### Copy-paste project template

Save this as `_portfolio/my-project.md`, then change every `my-project` and the sentences.

```markdown
---
title: "Project title"
excerpt: "One sentence for the projects list."
collection: portfolio
date: 2026-01-01
permalink: /projects/my-project/
---

Two or three sentences on what the project is and what you did.

{% include media-slot.html
   path="/images/projects/my-project/figure-1.jpg"
   alt="Describe the figure for someone who cannot see it"
   label="Figure 1"
   caption="Figure 1. Caption. File: images/projects/my-project/figure-1.jpg, about 1600 pixels wide."
%}

{% include media-slot.html
   youtube_id=""
   vimeo_id=""
   mp4=""
   alt="Describe the video"
   label="Video"
   caption="Video caption."
%}
```

`date` only controls the order on the projects page. It is not printed.

An empty `youtube_id=""` still counts as empty. Delete the line, or leave the quotes empty, and the dashed video box stays.

## Add a video

Use YouTube or Vimeo unless you have a reason not to. GitHub rejects any one file larger than 100 MB, and warns around 50 MB. A short screen recording can pass. A raw simulation movie usually will not.

**YouTube.** Upload the video, then copy only the id. In `https://www.youtube.com/watch?v=abcXYZ_123` the id is `abcXYZ_123`.

```liquid
{% include media-slot.html
   youtube_id="abcXYZ_123"
   alt="Wave gauge in the flume"
   caption="Video. Flume test, March 2026."
%}
```

**Vimeo.** In `https://vimeo.com/123456789` the id is `123456789`.

```liquid
{% include media-slot.html
   vimeo_id="123456789"
   alt="Wave gauge in the flume"
   caption="Video. Flume test, March 2026."
%}
```

**A file in this repository.** Put the MP4 at `files/videos/my-clip.mp4`. Keep it small.

```liquid
{% include media-slot.html
   mp4="/files/videos/my-clip.mp4"
   alt="Wave gauge in the flume"
   caption="Video. Local file."
%}
```

Set only one of `youtube_id`, `vimeo_id`, and `mp4`. YouTube is used first if more than one is filled in.

## Add a talk

Create `_talks/2026-05-01-seminar-title.md`:

```markdown
---
title: "Seminar title"
collection: talks
type: "Talk"
permalink: /talks/2026-05-01-seminar-title
venue: "Department seminar, The Hong Kong University of Science and Technology"
date: 2026-05-01
location: "Hong Kong"
---

Two or three sentences on what the talk covered.
```

It shows on the Talks page and on the CV. No talks are listed until you add a file.

## Update the biography and the CV

* Home page text, including the research-theme list: `_pages/about.md`
* Sidebar name, one-line title, city, university, email, and GitHub username: `_config.yml`, under `author:`
* CV sections: `_pages/cv.md`
* Top menu: `_data/navigation.yml`

The public email on the site is `hijaz@connect.ust.hk`. Do not add a phone number.

The blog is not in the menu. A post would be a file in `_posts/` named `YYYY-MM-DD-title.md`. Leave that folder empty until you want a blog.

## Publish on GitHub Pages

The site is meant to live at <https://hamdoon-ust.github.io/>, from a repository named `Hamdoon-UST.github.io`.

GitHub’s older Pages builder cannot run this theme’s Jekyll version. The repository includes `.github/workflows/jekyll.yml`, which builds the site and deploys it. In the repository on GitHub, open Settings, then Pages, and set the source to **GitHub Actions**.

After that, the usual update is:

1. Edit the files on your computer, or on the GitHub website.
2. Commit the change and push it to the `main` branch.
3. Wait for the Action named “Deploy Academic Pages template site to Pages” to finish. The live site updates when that Action succeeds.

A push to `main` is what publishes. You do not upload the `_site` folder.
