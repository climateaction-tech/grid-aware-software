# 1. Houston, we have a problem

Running compute jobs when and where the electricity grid is being powered by renewable energy must mean that the emissions associated with running that code are reduced. Running code using renewable “clean” electricity by definition means that it’s not consuming "dirty" fossil fuel energy. 

If we <a href="https://www.google.com/url?q=https://hackernoon.com/our-code-is-harming-the-planet-we-need-carbon-aware-design-patterns">make all our software carbon-aware</a>, timing it to run when and where the electricity grid is being powered by mostly renewable sources, then surely we can be confident we have effectively and innovatively reduced our environmental impact. Right?

This seems self-evident, and mostly the green computing community appears to agree. We’re full steam ahead and carbon-aware computing is being embraced at scale right now by Big Tech. Google implemented <a href="https://www.google.com/url?q=https://blog.google/outreach-initiatives/sustainability/carbon-aware-computing-location/">carbon-aware cloud computing in 2021</a>. Microsoft recently rolled out carbon-aware software updates for <a href="https://www.google.com/url?q=https://news.xbox.com/en-us/2023/01/11/xbox-carbon-aware-console-sustainability/">Xbox</a> and for <a class="c10" href="https://www.google.com/url?q=https://support.microsoft.com/en-us/windows/windows-update-is-now-carbon-aware">Windows 11</a>. In the US, the latest Apple iPhones have a <a class="c10" href="https://www.google.com/url?q=https://support.apple.com/en-us/HT213323&amp;sa=D&amp;source=editors&amp;ust=1699360648361683&amp;usg=AOvVaw29m8aO0kj_PQDUhCNdLNpm">carbon-aware charging feature</a>.

Carbon-aware approaches are being discussed for <a class="c10" href="https://www.google.com/url?q=https://ieeexplore.ieee.org/abstract/document/10105426">machine learning implementations</a>, gaining new momentum with the advent of generative models like ChatGPT. Blockchains too, with Bitcoin at the vanguard, <a class="c10" href="https://www.google.com/url?q=https://nordopen.nord.no/nord-xmlui/bitstream/handle/11250/2836156/Mellerud.pdf">have embraced carbon-aware patterns</a>, albeit in a more complicated way.

_We’re getting there, then, yes?_

**Not so fast.**

Who has actually paused to confirm whether these seemingly obvious claims are true? Does programming our software to responsively seek periods and locations with lower carbon intensity electricity actually make a tangible difference? Where are the studies that can prove this? If these patterns are implemented at scale, can the tech sector legitimately say it’s contributed to actually reducing global carbon dioxide (CO2) emissions?

Afterall, the ICT sector needs to be on a <https://www.itu.int/en/mediacentre/Pages/PR04-2020-ICT-industry-to-reduce-greenhouse-gas-emissions-by-45-percent-by-2030.aspx>pathway to reduce its carbon emissions by 45% in 2030</a> to be in-line with the <a hef="https://unfccc.int/most-requested/key-aspects-of-the-paris-agreement">Paris Agreement goals</a> of limiting global warming to 1.5ºC.

Those of us involved in writing this have paused to ask these questions. And we’re not the first to have done so [[1](#[1])][[2](#[2])].

Based on our exploration, we believe there is evidence to show current carbon-aware approaches may be mostly futile. What’s more, they might actually be _increasing_ emissions, while laying the foundations for the next generation of greenwashing across Big Tech. 

On the positive side, the evidence also suggests there are ways to implement such approaches with a greater likelihood of reducing emissions and avoiding perverse effects.

In this light, we believe our grand collective oversight is to omit any mention of the HUGE caveats to carbon-aware computing.

We explore these concerns and caveats. We start by acknowledging the technical detail of how electricity grids work in practice. We move to considering how current carbon-aware software approaches do not appear to take these realities into consideration. The post concludes by proposing an iteration on the current carbon-aware guidelines for a more responsible and effective implementation, which we call “grid-aware computing”.

## Next section

Continue the story -  [What software engineers need to know about how the grid works](how-the-grid-works.md)

#### [1]
https://github.com/Green-Software-Foundation/carbon-aware-sdk/issues/222

#### [2] 
https://adrianco.medium.com/dont-follow-the-sun-scheduling-compute-workloads-to-chase-green-energy-can-be-counter-productive-b0cde6681763

