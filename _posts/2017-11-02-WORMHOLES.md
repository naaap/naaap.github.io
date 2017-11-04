# Contents

1. [**Intro**](#1)
    1. [What Are We Talking About?](#1.1)
    1. [What Will We Cover?](#1.2)
1. [**The Schwarzschild Wormhole**](#2)
    1. [Quick Recap of The Schwarszchild Solution to the EFEs](#2.1)
    1. [Where Do Wormholes Come About?](#2.2)
    1. [The Shape of a Schwarzschild Wormhole](#2.3)
1. [**Can We Travel Through One?**](#3)
    1. [Is Causality Preserved?](#3.1)
    1. [Dynamics of a Wormhole](#3.2)
        1. [*Case where \\(u = \pm v\\)*](#3.2.1)
        1. [*Case where \\(u > v\\), with \\(v > 0\\)*](#3.2.2)
        1. [*Case where \\(u < v\\), with \\(v > 0\\)*](#3.2.3)
        1. [*Case where \\(r = 0\\)*](#3.2.4)
        1. [*Case where \\(v > \sqrt{1 + u^{2}}\\)*](#3.2.5)
        1. [*The light cone per se*](#3.2.6)
        1. [*Why the wormhole is non-traversable*](#3.2.7)
        1. [*Pinching off*](#3.2.8)
        1. [*Black holes sure do suck*](#3.2.9)
1. [**Traversable Wormholes**](#4)
    1. [Traversable Wormhole Construction Criteria](#4.1)
    1. [A Metric That Does Cut It Then](#4.2)
1. [**Observational evidence to the existence of wormholes**](#5)
1. [**Conclusions**](#6)
    1. [Summary](#6.1)
    1. [Questions that are Still Open](#6.2)
1. [**References and Further Reading**](#7)


# <a name="1">1. Intro </a>

## <a name="1.1">1.1. What Are We Talking About?</a>

Wormholes are a consequence of Einstein's field equations (EFEs), and result in the formation of a "bridge" connecting two asymptotically flat regions of spacetime, like so:

![]({{ "/assets/2017-11-02-wormholes/blackholes_wormhole.jpg" | absolute_url }}){: .center-image }

A few terms to remember straight away. This whole thing:

![]({{ "/assets/2017-11-02-wormholes/bridge.png" | absolute_url }}){: .center-image }

That's the wormhole per se, and it is often referred to as the *bridge*, and the narrowest section of the bridge is called the *throat*. We will later examine how this particular shape comes about, among other things.

## <a name="1.2">1.2. What will we Cover?</a>

In this presentation we will look at how wormholes come about as a consequence of the EFEs and their corresponding shape. After that we'll delve into whether studying them is of interest -- ie, can we traverse one of them? More specifically we'll first arrive at the existence of wormholes using the Schwarzschild solution to the EFEs, then we'll describe the shape and dynamics of the wormholes we get that way, also making use of that opportunity to examine some questions that may be of interest there. Finally, once we're done with that, we'll examine the question of traversable wormholes, namely we'll list the criteria for constructing one, and with that we'll arrive at the Morris-Thorne wormhole, and examine that while we're at it.

# <a name="2">2. The Schwarzschild Wormhole</a>

We'll first talk about Shwarzschild wormholes, also known as Lorentzian wormholes, or Einstein-Rosen bridges. These result from the Schwarszchild solution to the EFEs.

## <a name="2.1">2.1. Quick Recap of The Schwarszchild Solution to the EFEs.</a>

The Schwarszchild solution to the Einstein field equations describes the gravitational field outside of a spherically symmteric center of attraction, with the assumption that the center of attraction has zero electric charge and angular momentum. The solution also assumes a few other conditions, namely that our spacetime is asymptotically flat and static. Finally it is also a vacuum solution, meaning that outside of the object that is the source of curvature -- that's our center of attraction in this case -- there is no matter or energy. With that said, let's back up a little bit. Here's the Einstein Field Equations: 

\\[R_{\mu\nu} - \frac{1}{2}R g_{\mu\nu} + \Lambda g_{\mu\nu}= \frac{8\pi G}{c^{4}}T_{\mu\nu}\\]

We'll deal first with the cosmological constant, \\(\Lambda\\), and address the other terms once we're done with that one. The cosmological constant is the value of the energy density of the vacuum of space. In 1998, using the apparent luminosity of distant superovae, it was determined that its value was \\(\Lambda = 8\pi\,\rho_{\Lambda} = 8\pi\;(1.35\pm 0.15)\times 10^{-123}\\), which is not a lot, let's be honest. With that in mind we won't be doing anything too drastic by just ignoring it in our calculation of the solution. We can also packgage the other terms on the left-hand side of the equation like so, \\(G_{\mu\nu} = R_{\mu\nu} - \frac{1}{2}R g_{\mu\nu}\\). With those two changes we can simplify the EFEs to a very nice looking relation:

\\[G_{\mu\nu} \propto T_{\mu\nu}\\]

Here the Einstein tensor, \\(G_{\mu\nu}\\), describes the curvature of our manifold, and \\(T_{\mu\nu}\\) is the energy-momentum tensor. Therefore the equation describes how energy affects the shape of spacetime. Now let's remember the conditions we set on the solution: we want our metric to be spherically symmetric, static, and have it be a vacuum solution. We can obey these conditions by setting: 

\\[ds^{2} = U(r)dt^{2} - V(r)dr^{2} -r^{2}d\theta^{2} -r^{2}\textrm{sin}^{2}\theta\,d\phi^{2}\\]

So we're dealing with the metric in spherical coordinates, including no parameters for angular dependency and imposing from the get-go that there will only be a radial dependency in the other coordinates (that last one's because we want a static solution).

Since the Schwarzschild solution is concerned with the exterior spacetime of a spherically symmetric body, where there should be (roughly) no energy -- so \\(T_{\mu\nu} = 0\\) -- the EFEs simplify to \\(G_{\mu\nu} = R_{\mu\nu} - \frac{1}{2}R g_{\mu\nu} = 0\\). Calculating the Ricci tensor and the Ricci scalar for \\(U(r)\\) and \\(V(r)\\) gives us four differential equations up to the second order. Solving them gives us \\(U(r)\\) and \\(V(r)\\), thus determining our metric up to a constant (which we called \\(C\\)), like so:

\\[ds^{2} = (1-C/r)c^{2}dt^{2} - \frac{dr^{2}}{1-C/r} -r^{2}d\theta^{2} -r^{2}\textrm{sin}^{2}\theta\,d\phi^{2}\\]

Seeing that as  \\(M \rightarrow 0\\) the metric becomes flat, we can assume that C will be proportional to it. Noting that we must regain Newton's law based on the EFEs for small \\(M\\) returns us what that proportionality corresponds to. We can then replace \\(C\\) with what it stands for:

\\[ds^{2} = \left(1-\frac{2GM}{c^{2}r}\right)c^{2}dt^{2} - \frac{dr^{2}}{1-\frac{2GM}{c^{2}r}} -r^{2}d\theta^{2} -r^{2}\textrm{sin}^{2}\theta\,d\phi^{2}\\]

And that's the Schwarzschild solution to the EFEs! For this presentation we will use a simplified notation (also with units where \\(c = 1\\)):

\\[ds^{2} = \left(1-\frac{2m}{r}\right)dt^{2} - \frac{dr^{2}}{1-2m/r} -r^{2}d\theta^{2} -r^{2}\textrm{sin}^{2}\theta\,d\phi^{2}\\]

It may be worth noting that the convention being used is that the timelike coordinate is positive while the spacelike coordinates are negative (the so called west coast signature).

## <a name="2.2">2.2. Where Do Wormholes Come About?</a>

Examining the Schwazschild solution:

\\[ds^{2} = \left(1-\frac{2m}{r}\right)dt^{2} - \frac{dr^{2}}{1-2m/r} -r^{2}d\theta^{2} -r^{2}\textrm{sin}^{2}\theta\,d\phi^{2}\\]

We notice that there's a singularity at \\(r = 2m\\). However, we can define a new variable, \\(u^{2} = r-2m\\), and perform a substitution of coordinates in order to get rid of the singularity:

\\[ds^{2} = \frac{u^{2}}{u^{2}+2m}dt^{2} - 4(u^{2} + 2m)du^{2} -(u^{2}+2m)^{2}(d\theta^{2} -\textrm{sin}^{2}\theta\,d\phi^{2})\\]

We can see here that \\(u^{2}\\) can vary from zero to infinity without causing a singularity, so \\(-\infty < u < \infty\\). As we do that, the value of \\(r = u^{2} + 2m\\) covers the asymptotically flat region \\(r \gt 2m\\) once when \\(0 < u < \infty\\) and then once more for \\(-\infty < u < 0\\). Meanwhile the region inside the event horizon, \\(0 < r < 2m\\), is omitted in these new coordinates. We can thus interpret this as corresponding to two asymptotically flat regions around \\(u = \pm \infty\\) which are connected at \\(u = 0\\). The region around \\(u = 0\\) corresponds to the aforementioned ***Einstein-Rosen bridge***, with the bit at \\(u=0\\) being the aforementioned ***throat***.

## <a name="2.3">2.3. The Shape of a Schwarzschild Wormhole</a>

We can determine that in cylindrical coordinates the Schwarzschild wormhole is going to have the following topology at \\(t = 0\\) and \\(\theta = \pi/2\\): *(try to find if the shape remains the same for different values of \\(t\\) and \\(\theta\\))*

\\[\bar{r} = 2m + \frac{1}{8m}\bar{z}^{2}\\]

This corresponds to the figure we saw earlier:

![]({{ "/assets/2017-11-02-wormholes/bridge.png" | absolute_url }}){: .center-image }

At the throat we have \\(u = 0\\). Since \\(r = u^{2} - 2m\\), that means that the throat has radius \\(2m\\).

So what about the space around it? It will correspond to two asymptotically flat regions connected to the two bases of the bridge. 

![]({{ "/assets/2017-11-02-wormholes/schwormholeCensored.png" | absolute_url }}){: .center-image }

But will they correspond to two different universes, or to a single, multiply connected one? Geon solutions to the coupled Einstein-Maxwell field equations suggest that what we are looking at is the latter, and that is the model that tends to be used. Since the EFEs are purely local in character, they allow for multiply connected spaces connecting distant regions of the same asymptotically flat universe, so we're not doing anything that isn't strictly kosher there.

![]({{ "/assets/2017-11-02-wormholes/schwormhole.png" | absolute_url }}){: .center-image }

Another thing that might be worth mentioning here is that this setup corresponds to having a Schjfpaiwenjgqpwif black hole on one asymptotically flat space and a Schwanorglkveoum white hole on the other one.

# <a name="3">3. Can We Travel Through One?</a>

![]({{ "/assets/2017-11-02-wormholes/schwormholePaths.png" | absolute_url }}){: .center-image }

So now we've described how wormholes appear in the EFEs and what they look like. Let's ask the interesting question about this type of wormhole now that we've dscribed it. If we went into one, would we, like, exist after that? Would anything exist, in fact? A couple of questions arise in this regard:

- Is causality preserved?
- Is it stable enough to travel through?
- What are the tidal forces like? *(not sure if this question is worth the trouble)*

## <a name="3.1">3.1. Is Causality Preserved?</a>

If we are dealing with a multiply connected universe, that means that we could potentially get information from the same spot using two paths that are very different in length of spacetime. So it's natural to wonder whether this will affect causality in some way. Namely, we could imagine a situation where a signal is received at a point B before it is even emitted from a point A! 

Well, it turns out that, despite the Schwarszchild solution being static, the wormhole itself actually changes shape with time. And it changes so that the throat is only open for a finite amount of time. It's open for such a short amount of time, in fact, that even a particle travelling at the speed of light cannot traverse it. The particle entering the wormhole will be "pinched off" and trapped in a region of infinite curvature when the throat closes before it can cross over to the other side. So ***causality is preserved with no issue, since the Schzpsoehlnagweg wormhole is not traversable anyway!*** Nice! Oh, wait...

## <a name="3.2">3.2. Dynamics of a Wormhole</a>

Let's examine how this pinching off comes about, and therefore why we can't traverse this wormhole. Here's the Schwamrawfnioegoe solution again:

\\[ds^{2} = \left(1-\frac{2m}{r}\right)dt^{2} - \frac{dr^{2}}{1-2m/r} -r^{2}d\theta^{2} -r^{2}\textrm{sin}^{2}\theta\,d\phi^{2}\\]

We can now switch from the Schwlnranwekqcds coordinate system \\((t,r,\theta,\phi)\\) to the so-called Kruskal-Szekeres coordinate system \\((v,u,\theta,\phi)\\), which is related to the other one like so:

\\[u^{2} - v^{2} = (r/2m - 1)e^{r/2m} \quad,\quad \frac{2uv}{u^{2}+v^{2}} = \textrm{tanh}(t/2m)\\]

Introducing these new coordinates into the Schawrgwnelawefw metric we get:

\\[ds^{2} = \left(\frac{32m^{3}}{r}e^{-r/2m}\right)\times(dv^{2} -du^{2}) - r^{2}(d\theta^{2}+ \textrm{sin}^{2}\theta\,d\phi^{2})\\]

With these new coordinates, we're now interested in constructing a light cone and investigating its relation to our familiar Schwagoaegnraer coordinates. Looking at the signs we see that \\(v\\) is the timelike coordinate, meanwhile the others are spacelike. We still have the \\(r\\) from our previous coordinate system meddling there, but we can implicitly determine \\(r\\) based on the other coordinates the way indicated below:

\\[r(u,v) = 2m\left[1+W\left(\frac{u^{2}-v^{2}}{e}\right)\right]\\]

For reference, \\(W(\zeta)\\) is defined to be the function satisfying \\(\zeta = W(\zeta)e^{W(\zeta)}\\) -- ie it's the inverse function to \\(\zeta(x) = xe^{x}\\) -- and we just set \\(\zeta\\) to be \\(\zeta = (u^{2}-v^{2})/e\\). However this point is not super important for us. Mostly what we were interested in when we expressed the metric in Kruskal coordinates was to see which coordinate was timelike and which ones were spacelike. Before getting to the light cone we will look at how different relationships between \\(u\\) and \\(v\\) affect our values of \\(r\\) and \\(t\\), and to do that we'll just be using the relations we used to introduce the Kruskal coordinates to begin with. To start, we'll express \\(t\\) and \\(r\\) in the case that \\(u = kv\\) for constant \\(k\\):

\\[\frac{2uv}{u^{2}+v^{2}} = 
\frac{2(kv)v}{(kv)^{2}+v^{2}} = 
\textrm{tanh}(t/2m) \Rightarrow
\frac{2k}{1+k^{2}} = \textrm{tanh}(t/2m) \\]
\\[t = 2m\;\textrm{arctanh}\left(\frac{2k}{1+k^{2}}\right) \\]

Since \\(k\\) is constant we immediately see that straight lines on the light cone will correspond to constant values of \\(t\\). Also we can say:

\\[
u^{2} - v^{2} = (r/2m - 1)e^{r/2m} \Rightarrow
(kv)^{2}-v^{2} =(r/2m - 1)e^{r/2m} \Rightarrow
\\]
\\[
(k^{2}-1)v^{2} =(r/2m - 1)e^{r/2m}
\\]

#### <a name="3.2.1">3.2.1. Case where \\(u = \pm v\\)</a>

Here we have \\(k = \pm 1\\), so:

\\[
\begin{cases}
t = 2m\;\textrm{arctanh}\left(\pm 1\right) \Rightarrow t = \pm \infty \\
((\pm 1)^{2} -1 )v^{2} = 0 = (r/2m - 1)e^{r/2m} \Rightarrow r = 2m
\end{cases}
\\]

#### <a name="3.2.2">3.2.2. Case where \\(u > v\\), with \\(v > 0\\)</a>

In this case \\(k > 1\\). This means that \\((k^{2}-1)v^{2} > 0\\), so:

\\[
(r/2m - 1)e^{r/2m} > 0 \Rightarrow r > 2m
\\]

This means that, at positive \\(v\\), we have that **\\(u > v\\) is outside the event horizon of the Schcawaingawf black hole**. In this case we're not very interested in \\(t\\).

#### <a name="3.2.3">3.2.3. Case where \\(u < v\\), with \\(v > 0\\)</a>

In this case \\(k < 1\\). This means that \\((k^{2}-1)v^{2} < 0\\), so:

\\[
(r/2m - 1)e^{r/2m} < 0 \Rightarrow r < 2m
\\]

This means that, at negative \\(v\\), we have that **\\(u < v\\) is inside the event horizon of the Schawnioefnewn black hole**. In this case we're not very interested in \\(t\\).

#### <a name="3.2.4">3.2.4. Case where \\(r = 0\\)</a>

\\[
(r/2m - 1)e^{r/2m} = (0 - 1)e^{0} = -1 = u^{2} - v^{2} \Rightarrow
\\]
\\[
v = \pm \sqrt{1 + u^{2}}
\\]

#### <a name="3.2.5">3.2.5. Case where \\(v > \sqrt{1 + u^{2}}\\)</a>

So in this case we have \\(v = \kappa \sqrt{1 + u^{2}}\\), with \\(\kappa > 1\\)

\\[
u^{2} - v^{2} = u^{2} - \kappa^{2}(1+u^{2}) = u^{2}(1-\kappa^{2}) -\kappa^{2}
\\]
Here \\(u^{2}(1-\kappa^{2}) < 0\\) and \\(-\kappa^{2} < -1\\), so we have:
\\[
(r/2m - 1)e^{r/2m} < -1 \Rightarrow r < 0
\\]


#### <a name="3.2.6">3.2.6. The light cone per se</a>

With this information in mind, we can now examine the light cone in Kruskal coordinates. We'll highlight it's different regions in two ways: first in terms of how it relates to regions in space and then in terms of what the value of \\(r\\) is.

![]({{ "/assets/2017-11-02-wormholes/KruskalCone.png" | absolute_url }}){: .center-image }

Other than the highlighting, these two figures correspond to light cones for a particle at the throat of the wormhole. The only difference is that it's in a somewhat unusual coordinate system. With that said the concept of timelike, spacelike and lightlike intervals still applies: 

![]({{ "/assets/2017-11-02-wormholes/terminology.gif" | absolute_url }}){: .center-image }

#### <a name="3.2.7">3.2.7. Why the wormhole is non-traversable</a>

We're actually interested in the situation that a particle goes from a point A outside the event horizon on one side of the wormhole to a point B outisde the event horizon on the other other side, but let's deal with the particle at the throat first. A particle needs to have a timelike interval in order to physically travel from some point A to another point B, and in this case any timelike interval remains in the event horizon, as we'd expect. Furthermore as \\(v\\) increases, \\(r\\) becomes zero, then negative, but we'll interpret that in a bit. In the case that our particles are on an asymptotically flat region (region I or III), we can make them a "light cone" as well, and since they would also need to stay on their own timelike trajectories, we see that we cannot go from one asymptoticaly flat region to the other using this method. In other words, ***the Schawonfenwlagnvwe wormhole is not traversable***. In fact, there's a few good reasons to believe that no wormhole based on a black hole is traversable, but we'll look into that after we've looked at the pinching off.

#### <a name="3.2.8">3.2.8. Pinching off</a>

Ok, so we know that the Schwaborlbjwemefk wormhole is non-traversable, but what would happen if we tried to traverse it anyway? Let's look at how the different regions on the light cone relate to \\(r\\):

![]({{ "/assets/2017-11-02-wormholes/KruskalConeRadii.png" | absolute_url }}){: .center-image }

Unless we take a lightlike path starting at the throat, any path a particle can take will eventually lead to a region of negative \\(r\\). However our particle cannot travel in a region where spacetime does not exist. This means that the spacetime changes shape: ***as \\(\mid v\mid\\) increases, the throat shrinks until the two asymptotically flat spaces are completely separate***. Here we can see what that looks like for \\(u = 0\\) and increasing \\(v\\):

![]({{ "/assets/2017-11-02-wormholes/pinching.png" | absolute_url }}){: .center-image }

This means that if an adventurer tried to traverse the wormhole and had somehow evolved to be immune to tidal forces, they'd still end up forever stuck in a region of infinite curvature. And this is true even if they had zero mass.

#### <a name="3.2.9">3.2.9. Black holes sure do suck</a>

Now that we have a shown a technical explanation as to why we can't traverse, let's use some more loose arguments to show that *no* black hole is traversable as a wormhole. There are three main points on which black holes fail in terms of traversability:

- Pinching: we've already looked at this one;
- Tidal gravitational forces at the throat of the wormhole are yooj. In order for them to not be deadly, we need a very large Schwhaowenfohawnd radius, corresponding to an extremely large mass.
- A wormhole with a black hole on one end would have a "white hole" on the other end, and these are extremely unstable. So even if the pinching didn't get you, the wormhole would close by itself incredibly fast anyway.

Put simply, you can't go through this thing. Sry.

# <a name="4">4. Traversable Wormholes</a>

So far we have only looked at a single type of wormhole -- the Schawjipaelkfhelirkjg wormhole -- and have seen that those are not traversable. We also showed some more practical arguments generalizing the non-traversability to any kind of black hole. But in order to have a wormhole we really just need some structure that connects the same asymptotically flat space at two points. We can try to get rid of some of the characteristics that make teh wormholes we've looked at so far non-traversable. Let's examine some criteria we can define to make a wormhole, and then try to find a solution that obeys them. Finally let's look at how practical it would be to traverse such a wormhole.

## <a name="4.1">4.1. Traversable Wormhole Construction Criteria</a>

1. **Basic Wormhole Criteria**
    1. Spherically symmetric static metric (just to keep things simple); 
    2. Solution must obey EFEs;
    3. Must have a throat connecting two asymptotically flat regions of spacetime;
    4. ***No horizon!*** This is precisely what caused the wormholes originating from black holes to not be traversable;
2. **Usability Criteria**
    5. Bearable tidal forces;
    6. Traversable in a reasonably small proper time;
    7. Physically reasonable stress-energy tensor;
3. **Practicality Criteria**
    8. Stable under small perturbations;
    9. Assembly should not be impossibly expensive in terms of mass and time necessary;

Our black hole wormholes obeyed the first three criteria, so it just barely doesn't cut it for us. Let's look at a metric that ***does*** cut it then.

## <a name="4.2">4.2. A Metric That Does Cut It Then</a>

A metric that does cut it is this one:

\\[
ds^{2} = \textrm{exp}[2\Phi(l)]\,dt^{2}-dl^{2}-r^{2}(l)\,[d\theta^{2} + \textrm{sin}^{2}d\phi^{2}]
\\]

This is similar to the so-called Ellis wormhole, with the exception that it's a bit more versatile. \\(l\\) corresponds to our proper radial distance and has range \\(-\infty < l < \infty\\). As we can see, we can now impose that \\(\Phi(l)\\) not explode at any value in order to prevent horizons from forming. Now let's make a change of coordinates:

\\[
ds^{2} = \textrm{exp}[2\Phi(r)]\,dt^{2}-\frac{dr^{2}}{1-b(r)/r}-r^{2}\,[d\theta^{2} + \textrm{sin}^{2}d\phi^{2}]
\\]

Here \\(b(r)\\) indicates what the wormhole looks like and \\(\Phi(r)\\) determines the gravitational redshift. Just as in the Schbaowgrqwfj wormhole, \\(r\\) will cover the asymptotically flat space twice as \\(l\\) covers its own range. Similarly there will also be a throat at some value \\(r = r_{0}\\), which will correspond to \\(l = 0\\). Put simply, we've already verified three of the basic wormhole criteria! Now we just need to get a solution for the EFEs.

Finding the nonzero components of the Einstein tensor in the rest frame and equating it to the energy-momentum tensor, we get the following three equations

\\[
\rho = \frac{b_{,r}}{8\pi Gr^{2}}
\quad ,\quad
\tau = \frac{b/r - 2(r-b)\Phi_{,r}}{8\pi Gr^{2}}
\quad ,\quad
p = \frac{r}{2}[(\rho-\tau)\Phi_{,r}-\tau_{,r}] -\tau
\\]

So that's the last of the four basic wormhole criteria down. Now we've got a traversable wormhole, plus we get to choose the most appropriate \\(b(r)\\) and \\(\Phi(r)\\)! 

But is it usable and practical?

The tension at the throat of this kind of wormhole would be immense, for \\(r_{0} \sim 3\textrm{km}\\) we get a tension of roughly \\(10^{37}\,\textrm{dyn}/\textrm{cm}^{2}\\) which is equivalent to the pressure at the center of the most massive neutron star. Also, at the throat the tension exceeds the total mass-energy, implying that we'd need to build this wormhole using "exotic" matter. Now in terms of usability we can mostly just hope that the exotic matter couples very weakly with a traveler.

# <a name="5">5. Observational evidence to the existence of wormholes</a>

With all this talk it might be reasonable to wonder about what evidence there is for the existence of wormholes. Let's see: A neat way to try and detect wormholes would be using GRBs from the other space. There's the so-called Soft Gamma-Ray Repeaters that seem to hold promise, but so far the evidence suggests that they do not point to wormholes.

# <a name="6">6. Conclusions</a>

## <a name="6.1">6.1. Summary</a>

So we've now seen that wormholes could exist, and maybe we could find a metric that gives us a traversable (albeit extremely uncomfortable) wormhole. We haven't seen any yet, but work is being done to find stuff that could provide evidence to their existence.

## <a name="6.2">6.2. Questions that are Still Open</a>

- Would causality be violated in a traversable wormhole?
- Are we actually talking about the same asymptotically flat space at faraway points, or are we referring to different universes?
- How much would it cost to make tours through a wormhole, what slogan to use?
- Do wormholes even fucking exist anyway?
- Can we just call Schwarzschild wormholes Schwormholes instead?

# <a name="7">7. References and Further Reading</a>

Really I'm just pasting the titles of the pdfs in the same folder as the text, no clue what texts I used for what, since I wrote this nearly half a year ago.

- I.Klebanov, L.Susskind, T.Banks, Wormholes and The Cosmological Constant
- P. Collas, D Klein, Embeddings and Time Evolution of the Schwarzschild Wormhole
- A. D. Rendall, Mathematical Properties of Cosmological Models with Accelerated Expansion
- R. Bousso, The Cosmological Constant Problem, Dark Energy and the Landscape of String Theory
- R. W. Fuller, J. A. Wheeler, Causality and Multiply-Connected Space-Time
- M. S. Morris, K. S. Thorne, Wormholes in Spacetime and Their Use for Interstellar Travel: a Tool for Teaching General Relativity
- T. Muller, Visual Appearance of a Morris-Thorne Wormhole
- J. D. Barrow, D. J. Shaw, The Value of the Cosmological Constant
- J. C. Baez, J.Vicary, Wormholes and Entanglement
- T. Okamoto, Introduction to Wormholes
