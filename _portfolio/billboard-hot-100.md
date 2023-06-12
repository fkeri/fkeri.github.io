---
title: "A Data-driven Journey through Time:<br /> Exploring the Evolution of Popular Music Sound"
excerpt: "Exploring the evolution of popular music over time using the Billboard Hot 100 historical data to identify popular tracks, and leveraging Spotify Audio Features API to quantify the tracks' sound characteristics."
# excerpt_separator: "<!--more-->"
header:
  # image: /assets/images/billboardspotify_logo.png
  teaser: /assets/images/billboardspotify_logo.png
sidebar:
  - title: "### Skills:"
    image: /assets/images/billboardspotify_logo_teaser.png
    image_alt: "Billboard Spotify Project Logo"
    text: |
      * Web Scraping
      * Data Visualization
      * Hypothesis Testing
      * Interactive Data App with Plotly Dash
  - title: "### External links:"
    text: |
      * ##### [Jupyter Notebook](https://nbviewer.org/github/fkeri/BillboardSpotify/blob/master/src/notebooks/SpotifyAudioFeatures.ipynb){:target='_blank'}
      * ##### [Interactive Data App - Audio Feature Distributions](https://billboard-spotify-data-app.onrender.com){:target='_blank'}
      * ##### [Interactive Data App - Animated Joint Audio Feature Distributions](https://billboard-spotify-animation-data-app.onrender.com){:target='_blank'}
gallery:
  - url: /assets/images/animated_contour_plot.gif
    image_path: /assets/images/animated_contour_plot.gif
    alt: "Animated Contour Plot: Danceability vs Valence over Billboard Decades"
  - url: /assets/images/acousticness_box_plot.png
    image_path: /assets/images/acousticness_box_plot.png
    alt: "Acousticness Box Plot over Billboard Decades"
  - url: /assets/images/duration_ridge_plot.png
    image_path: /assets/images/duration_ridge_plot.png
    alt: "Duration (minutes) Ridge plot over Billboard Decades"
  - url: /assets/images/valence_ridge_plot.png
    image_path: /assets/images/valence_ridge_plot.png
    alt: "Valence Ridge plot over Billboard Decades"
classes: wide
---
{% include gallery caption="Fig 1. Sample plots of Billboard Decade popular tracks' Audio Features that can be found in the [Jupyter Notebook](https://nbviewer.org/github/fkeri/BillboardSpotify/blob/master/src/notebooks/SpotifyAudioFeatures.ipynb){:target='_blank'} and the Interactive Data Apps [1) Audio Feature Distributions](https://billboard-spotify-data-app.onrender.com){:target='_blank'} and [2) Animated Joint Audio Feature Distributions](https://billboard-spotify-animation-data-app.onrender.com){:target='_blank'} for this project." layout="half" %}
## Motivation

In this project, I was interested to explore how the sound of popular music evolved over time. Thus, I set out to quantify and visualize something as intangible as the concept of the *"sound of the 1960s"* and draw comparisons to the contemporary music landscape.

To achieve this, I sought to obtain relevant data that would enable me to answer two fundamental questions:
1. What tracks could be deemed representative of the sound of a particular decade?
2. Given a set of tracks that represents the sound of a particular decade, how can I quantify the decades' sound characteristics?

To answer these questions, I turned to the data sources outlined in the following section.

## Data Sources

### 1. Billboard Hot 100 Historical Data

To answer Question 1: *"What tracks could be deemed representative of the sound of a particular decade?"*, I turned to the Billboard Hot 100 historical data.

The Billboard Hot 100 is a weekly chart that ranks the top 100 songs in the United States based on their popularity and sales. It is published by Billboard magazine and is considered one of the most authoritative and influential music charts in the industry. The chart is based on a combination of factors: including radio airplay, streaming activity, and physical and digital sales. Each week, the chart is updated to reflect the latest trends in popular music. The Billboard Hot 100 has been published since 1958 and has become a significant indicator of a song's success in the US music industry.

### 2. Spotify Audio Features API

To answer Question 2: *"Given a set of tracks that represents the sound of a particular decade, how can I quantify the decades' sound characteristics?"*, I turned to the Spotify Audio Features API.

The Spotify Audio Features API is a tool that provides access to audio analysis and metadata for music tracks hosted on the Spotify platform. The API allows developers to retrieve a range of audio features for a given track, such as tempo, key, mode, time signature, loudness, and more. The API is based on machine learning algorithms that analyze the audio content of a track to extract its key characteristics.