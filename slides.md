---
title-slide: false
bibliography: references.bib
csl: vancouver.csl
citeproc: true
theme: serif
background-color: "#ffffff"
transition: slide
navigationMode: linear
hash: true
---

:::: {.columns}
::: {.column width="50%"}

## Sample slides
#### PlaceHolderName
#### Universiti Malaysia Perlis
#### [placeholder@email.com](mailto:placeholder@email.com)

<audio id="bg-music" src="media/audio/sb.m4a" loop></audio>

<div id="audio-credit"
     style="position: absolute; bottom: 40px; right: 20px; font-size: 0.6em; opacity: 0.6;">
  Music: “Adrift” by Scott Buckley (CC BY 4.0)
</div>

<script>
  document.addEventListener('DOMContentLoaded', () => {
    const audio = document.getElementById('bg-music');
    const credit = document.getElementById('audio-credit');

    // hide credit by default
    credit.style.display = 'none';

    const test = new Audio('media/audio/bgm.mp3');

    test.addEventListener('canplaythrough', () => {
      // bgm.mp3 exists → use it, keep credit hidden
      audio.src = 'media/audio/bgm.mp3';
    }, { once: true });

    test.addEventListener('error', () => {
      // bgm.mp3 missing → sb.m4a will play → show credit
      credit.style.display = 'block';
    }, { once: true });

    document.addEventListener('click', () => {
      if (Reveal.getIndices().h === 0) {
        audio.volume = 0.5;
        audio.play();
      }
    }, { once: true });

    Reveal.on('slidechanged', (event) => {
      if (event.indexh > 0) { audio.pause(); }
      else { audio.play(); }
    });
  });
</script>

:::

::: {.column width="50%"}
![](media/pics/logo1.png)
:::

::::

---

:::: {.columns}
::: {.column width="50%"}
### Slide one
**Key Concepts:**
- Energy conservation per @carnot1824.
- $\Delta U = Q - W$
:::

::: {.column width="50%"}
![](media/pics/sample.png)
:::
::::

---

<span class="slide-title" data-title="My Hidden Slide Name"></span>

![](media/pics/wide.jpeg)

---

:::: {.columns}
::: {.column width="50%"}
### The Master Equation
The fundamental relation of thermodynamics:

$$\Delta U = Q - W$$

The work done $W$ is positive when the system expands against an external pressure.
:::

::: {.column width="50%"}
<video data-src="media/videos/sample.mp4" data-autoplay loop muted width="100%"></video>
:::

::::

---

:::: {.columns}
::: {.column width="50%"}
### Visualizing the Gas Law
**Interactive Model:**

- P, V, and T relationships.
- Use the slider to adjust pressure.
- Observe the phase boundary.
:::

::: {.column width="50%"}
<iframe 
  data-src="media/plots/sample.html" 
  width="100%" 
  height="500px" 
  style="border:none;" 
  scrolling="no">
</iframe>
:::
::::

---

# Bibliography
<div id="refs"></div>

---

:::: {.columns}
::: {.column width="50%"}
### Distribution of Weight
We can visualize the distribution of student weights using a histogram.
:::

::: {.column width="50%"}
<iframe
  data-src="media/plots/histogram_weight.html"
  width="100%"
  height="500px"
  style="border:none;"
  scrolling="no">
</iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Verbal Scores by Gender
Comparing average verbal scores between male and female students.
:::

::: {.column width="50%"}
<iframe
  data-src="media/plots/barchart_verbal_sex.html"
  width="100%"
  height="500px"
  style="border:none;"
  scrolling="no">
</iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Height Distribution
An examination of height distribution, stratified by student sex, using a boxplot.
:::

::: {.column width="50%"}
<iframe
  data-src="media/plots/boxplot_height_sex.html"
  width="100%"
  height="500px"
  style="border:none;"
  scrolling="no">
</iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Height and Weight Correlation
A scatterplot illustrating the relationship between height and weight, with points colored by sex.
:::

::: {.column width="50%"}
<iframe
  data-src="media/plots/scatterplot_height_weight_sex.html"
  width="100%"
  height="500px"
  style="border:none;"
  scrolling="no">
</iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Distribution of Age
We can visualize the distribution of student ages using a histogram.
:::

::: {.column width="50%"}
<iframe
  data-src="media/plots/histogram_age.html"
  width="100%"
  height="500px"
  style="border:none;"
  scrolling="no">
</iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Math Scores by Gender
Comparing average Math scores between male and female students.
:::

::: {.column width="50%"}
<iframe
  data-src="media/plots/barchart_math_sex.html"
  width="100%"
  height="500px"
  style="border:none;"
  scrolling="no">
</iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Weight Distribution
An examination of weight distribution, stratified by student sex, using a boxplot.
:::

::: {.column width="50%"}
<iframe
  data-src="media/plots/boxplot_weight_sex.html"
  width="100%"
  height="500px"
  style="border:none;"
  scrolling="no">
</iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Height and Weight Correlation
A scatterplot illustrating the relationship between height and weight, with points colored by sex. (Reprise)
:::

::: {.column width="50%"}
<iframe
  data-src="media/plots/scatterplot_height_weight_sex_reprise.html"
  width="100%"
  height="500px"
  style="border:none;"
  scrolling="no">
</iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Part Length Analysis
A scatterplot showing the distribution of part lengths over the recorded observations.
:::

::: {.column width="50%"}
<iframe
  data-src="media/plots/scatterplot_partlength.html"
  width="100%"
  height="500px"
  style="border:none;"
  scrolling="no">
</iframe>
:::
::::
