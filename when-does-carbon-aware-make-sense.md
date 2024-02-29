# 4. When does carbon-aware software make sense?

Let’s be absolutely clear on the answer to the question “is carbon-aware computing just bad?” No. We don’t intend to bash the core concepts of carbon-aware software. 

The core concept that shifting compute jobs to respond to the electricity available is sound.

**The criticism is that current approaches never apply any warning labels.**

There is no real acknowledgement of the nuances of how balancing electricity supply and demand works in practice. We fail to mention that the current patterns are only helpful in certain circumstances, futile in most, and seriously harmful in others. It seems the uncomfortable outcome is all this effort hampers tech’s sustainability efforts as we try to help them. 

Most crucially we see don’t carbon-aware software meaningfully addressing the elephant in the room. **It is simply not possible to optimise our way to the reductions needed in the tech sector, whilst tech’s overall energy and resource demands grow rampantly.**
The damage of runaway climate change to populations around the world demands that we do better, and we believe the tech sector is <a href="https://rtl.chrisadams.me.uk/2023/07/comparing-what-is-spent-on-share-buybacks-vs-the-cost-of-decarbonising-the-grid/">well resourced enough to tackle this in a meaningful way</a>.


## What are the warning labels that need to be applied?

There are two ways in which we think the logic of the carbon-aware approach holds true.

**Way 1:** Time-shifting or location-shifting compute to when demand is naturally low and then using electricity that would otherwise be curtailed.

**Way 2:** When jobs run on electricity that is additive to the grid.

Don't just take our word for these two. The shortest, clearest authoritative summary on this is from a <a href="https://www.whitehouse.gov/wp-content/uploads/2022/09/09-2022-Crypto-Assets-and-Climate-Report.pdf">White House investigation into crypto mining</a> (see page 24). The useful part says:

> "There are two primary ways.... using grid electricity would result in zero direct GHG emissions:
>
> 1) constructing or contracting for new clean electricity sources or
> 
> 2) using existing renewable electricity that would otherwise be curtailed by the grid.
>
> When... electricity [comes] from existing renewable sources, it displaces the GHG emissions in the near-term, shifting users of renewable sources to fossil fuel sources. This is because coal and natural gas often supply electricity generation for each additional unit of electricity demanded in the United States. As the amount of renewable sources is held constant, but electricity demand increases, additional fossil power will likely be dispatched. This displacement results in no net change or in increases in total global emissions through a process called leakage.”

We get into these two ways in the sections below. In the next section, we discuss [addressing the elephant in the room](elephant-in-room.md) - the net increases in resources demanded by the tech sector even with all this optimisation effort. This leads us to present a third way.

### Way 1: Run compute when demand is low, using curtailed electricity in stable grids

> #### TL;DR:
>
> We propose the refinement to current carbon-aware time-shifting or location-shifting approaches is to **prioritise demand intensity first and carbon intensity second**. We need to do this in collaboration with one another and local grid systems.

Scheduling compute to run at already predicted low demand times contrasts to the current approach of dynamically time-shifting to periods of high renewables/low carbon intensity, which fluctuates day-to-day and is hard to forecast. If we time-shift compute within our own grids based on grid demand in a highly predictable, stable fashion we don’t create unpredictable daily spikes.

This sounds simple for routine jobs. As a concept perhaps it is. But that doesn’t mean it isn’t a valuable contribution.

And for compute that’s more spontaneous? There’s some good demand-focused tweaks available here too.

Our beneficial impact can be even greater if running compute can play a part in helping the grid to avoid ramp-ups/downs. Going up or down can inflate carbon emissions, as we explored in [what software engineers need to know about how the grid works](how-the-grid-works.md). Ramping down also typically involves curtailing electricity, which is essentially wasting electricity. Getting compute to make use of that, regardless of the carbon intensity at the time, is an approach worth working on.

We think an alternative version of location-shifting, that factors in demand, could also be helpful. What if we first looked for grids that currently have low demand AND then sought those with a period of naturally high renewable electricity production? This contrasts to the current carbon-aware location-shifting approach that just looks at electricity carbon intensity.

In our proposed way we might look for places with low demand, let’s say between 2am and 4am, with high winds in a grid that does a solid job of harnessing wind energy. If that grid were unable to make use of all that wind and had to curtail it, our compute could use it for something productive.

The above has merit when happening at a relatively small scale. But if everyone does this at the same time? Then we *still* have the problem of creating demand spikes, one our core worries about the current approaches.

### A long-term vision 

So, let’s take the approach even further and imagine a long-term goal. Let’s make it standard that our compute jobs, and more specifically the data centres running these jobs, interface with grids and become part of the solution rather than the problem. These ideas fall into the realm of **demand management**, which we introduce in [what software engineers need to know about how the grid works](how-the-grid-works.md) and touch on again in [addressing the elephant in the room](elephant-in-room.md).

By interacting with grid management systems, ideally in an automated, collaborative, and democratic way, we could identify times that assist with managing the grid, rather than placing additional burdens on it. Democratic here is key as well.

This can’t just be the realm of the Big Tech players. We all need a chance to participate through open source standards and protocols. By doing so, we can actually prevent fossil fuels from being used, further reducing net emissions – a win/win across the board.


### Way 2: Run compute on additive renewable energy

> #### TL;DR:
>
> To be in any way effective, computing must target green energy sources that are in fact additive, and transparently address and mitigate the risks of perverse effects.

There are two common ways running compute on additive renewable energy can be achieved. 

> ### Quick reference – Additive renewable energy 
>
> “Additive” or “additional” renewable electricity means your purchase is financing new renewable electricity that would otherwise not exist. Related is applying the principle of "<a href="https://www.electricitymaps.com/blog/what-is-additionality-and-emissionality">additionality</a>" to renewable energy generation, particularly in <a href="https://en.wikipedia.org/wiki/Carbon_emission_trading">carbon markets</a>. 
>
> If your compute consume 50 terawatts of electricity and you pay for new solar panels that generate 50 terawatts of electricity, you achieve additionality. You can claim, in theory, that your compute is emissions neutral. In practice <a href="https://kvenkatm.medium.com/we-need-a-better-way-of-purchasing-and-accounting-for-renewable-electricity-34c0ee66070e">it’s less clear-cut</a>, but this is the general idea.
>
> Traditional carbon markets often sell ‘carbon credits’ based on already existing renewable electricity. In this scenario there is no additionality. You are merely claiming the existing renewable energy production as yours and giving responsibility for the existing dirty energy production to someone else. This is not reducing emissions at all. 
  

#### Power Purchase Agreements (PPAs) and Renewable Energy Certificates (RECs)

The primary way that many organisations tackle this is through <a href="https://en.wikipedia.org/wiki/Carbon_emission_trading">carbon markets</a>. These in turn sell two main instruments:  <a href="https://en.wikipedia.org/wiki/Renewable_Energy_Certificate_(United_States)">Renewable Energy Certificates</a> (RECs) and <a href="https://en.wikipedia.org/wiki/Power_purchase_agreement">Power Purchase Agreements</a> (PPAs). 

This remains a highly problematic approach. Why? Because <a href="https://www.spglobal.com/esg/insights/problematic-corporate-purchases-of-clean-energy-credits-threaten-net-zero-goals">the vast majority of RECs are non-additive</a>. 

They enable you to buy into the existing green energy mix, and simply take credit for their contribution. But you have zero effect on what’s called ‘**emissionality**’, which has similarities to the **displacement effect**. 

> ## Quick reference – Emissionality
>
> New renewable energy projects don’t always pull emissions out of the atmosphere. The reason they help is because they **displace fossil fuel power plants** that would otherwise keep polluting.
>
> But which projects are effective? That can vary greatly from project-to-project as well as the fuel-mix of the grid to which the project will be connected. For example, adding one more solar power purchase agreement (PPA) in California increasingly reduces output from a mix of natural gas plants and existing solar farms. But adding a new wind PPA in Wyoming nearly always reduces output at a coal plant, avoiding more emissions. This practice of comparing and acting on the avoided emissions of different renewable energy projects is called “emissionality.”
> 
> You can <a href="https://www.watttime.org/solutions/renewable-energy-siting-emissionality/">read more on this by WattTime</a>, who popularised the emissionality term.

PPAs are commonly employed throughout the business world, especially by <a href="https://www.datacenterdynamics.com/en/opinions/ppa-evolution-in-the-data-center-industry/">data centres</a>. Corporate purchasers make agreements with energy companies promising to purchase the power and RECs generated by the renewable project for a specific time period, often the next 10-15 years. 

While PPAs are often touted as a critical mechanism responsible for a company’s green credentials and central to its <a href="https://en.wikipedia.org/wiki/Environmental,_social,_and_corporate_governance">ESG strategy</a>, they can be misleading. Even if PPAs are attributed to particular renewable projects, <a href="https://www.datacenterdynamics.com/en/analysis/everything-data-center-operators-need-to-know-about-power-purchase-agreements-ppas/">they do not generally directly power data centres</a>. In other words, just because green electrons are being produced, does not mean those electrons are directly powering the compute within a data centre – despite often being <a href="https://www.electricitymaps.com/blog/green-electricity-contracts">touted as so</a>. There is also the risk of <a href="https://www.epa.gov/green-power-markets/double-counting">double counting</a>.

Therefore the best implementation of carbon markets involves ensuring that the renewable energy you purchase is *additive*.

### Your own renewable sources

A second, much rarer version of additionality - yet far more effective. 

Instead of purchasing some remote renewable infrastructure and “accounting” your claim to being powered by renewables, **actually** power your compute directly from your own renewable sources.

If your compute is being directly powered by your own solar panels or wind turbines etc., there is no sleight of hand or complex statistical projections. Your compute is effectively off grid to the extent that it is directly powered by your own renewable sources.

While preferable in terms of emissions, this approach is challenging to scale and risks perverse effects as get into below. 

### Innovation with distributed alternatives
As a complement to this section, it’s worth mentioning there’s room to innovate with distributed alternatives. Distributed compute and renewable electricity generation. We've pulled out some of the ideas/research around this into [Appendix 1](/appendices/appendix-1.md).


## Next section
Continue the journey: [Addressing the elephant in the room](elephant-in-room.md)
