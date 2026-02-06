# Statistical testing in null worlds

> [!NOTE]
> **This repository isn't maintained.**
>
> This is only here as a reference for future me so I don't lose all the cool webR stuff I had set up. This isn't in production anywhere, and it is miserably slow, but it's still a neat use of webR and Quarto Live.

This is the repository for the original version of my statistical testing in null worlds simulation (still accessible at <https://andrewheiss.github.io/null-world-testing-webr/>), where I adapted the principles of [{infer}](https://infer.netlify.app/), [ModernDive](https://moderndive.com/v2/hypothesis-testing.html), and Allen Downey's idea of [there being only one statistical test](https://allendowney.blogspot.com/2016/06/there-is-still-only-one-test.html) into an interactive site using [webR](https://docs.r-wasm.org/webr/latest/) and [Quarto Live](https://r-wasm.github.io/quarto-live/).

Everything worked, but it was really slow and not super reactive—it would take 10–20 seconds to install and load all the webR R packages, and then would take a bit to simulate the data and propagate the changes to all the other webR chunks on the page, which was annoying.

So I converted it to Observable JS instead, since [Quarto natively supports that](https://quarto.org/docs/computations/ojs.html), and since Javascript was, like, designed for browsers. That repository is at <https://github.com/andrewheiss/null-world-testing> and the official corresponding site is at <https://nullworlds.andrewheiss.com/>.
