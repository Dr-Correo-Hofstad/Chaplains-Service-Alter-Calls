The impact that created the South Pole-Aitken (SPA) basin occurred **between 4.25 and 4.33 billion years ago**. Based on the blast pattern, the asteroid came from the **North** and traveled **Southward** at an oblique, glancing angle of **30° to 45°**. \[1, 2, 3, 4\]

## **Blast Pattern Evidence**

* **Teardrop Shape**: The basin is not a perfect circle; it is an ellipse that **tapers and narrows toward the south**. This teardrop outline is a definitive hallmark of a downrange oblique impact.  
* **Asymmetrical Rubble Piles**: High-resolution gravity data from NASA's GRAIL mission shows massive piles of excavated mantle material and heat-producing elements (thorium, iron, and KREEP) stacked thickly on the **southern rim**. This represents the directional "splash" of the impact. \[4, 5, 6, 7, 8\]

## ---

**The Math and Equations**

Planetary scientists reconstruct this multi-billion-year-old blast using physics, geometry, and radioactive decay equations. \[1, 2\]

## **1\. Blast Geometry (The Flattening Factor)**

To quantify the "blast pattern" asymmetry and confirm the angle, scientists measure the crater's tapering or flattening factor ($f$):  
$$f \= \\frac{a \- b}{a}$$  
Where: \[9\]

* $a$ \= semi-major axis (the north-south length)  
* $b$ \= semi-minor axis (the east-west width) \[6\]

Gravity and topographic mapping yield a value of **$f \\approx 0.16 \\text{ to } 0.18$**. This mathematical asymmetry rules out a vertical strike and perfectly matches 3D hydrocode models of a southward-glancing impact. \[9, 10\]

## **2\. Total Kinetic Energy of the Blast**

To form a basin this large, a differentiated asteroid roughly **260 kilometers wide** hit the surface at **13 km/s**. \[11\]

First, the mass ($M\_p$) of the projectile is calculated using volume and an average density ($\\rho \\approx 3,000 \\text{ kg/m}^3$):  
$$M\_p \= \\frac{4}{3}\\pi \\left(\\frac{D}{2}\\right)^3 \\rho \\approx 2.76 \\times 10^{19} \\text{ kg}$$

The total kinetic energy ($E\_k$) released upon impact equals:  
$$E\_k \= \\frac{1}{2} M\_p v^2 \\approx \\frac{1}{2} (2.76 \\times 10^{19} \\text{ kg}) \\times (13,000 \\text{ m/s})^2 \\approx 2.33 \\times 10^{27} \\text{ Joules}$$

## **3\. Oblique Angle Modification (Melt Scaling)**

Because the asteroid struck at an angle ($\\theta \\approx 30^\\circ\\text{–}45^\\circ$), the vertical energy distribution that digs the hole behaves differently than a straight-down impact. According to the standard **Pierazzo-Melosh scaling laws** for oblique impacts, the volume of impact melt ($V\_{\\text{melt}}$) scales directly with the sine of the impact angle:  
$$V\_{\\text{melt}}(\\theta) \\approx V\_{\\text{melt}}(90^\\circ) \\cdot \\sin(\\theta)$$

At a $30^\\circ$ angle, $\\sin(30^\\circ) \= 0.5$, meaning **50% less rock was melted** compared to a vertical strike. This lower vertical efficiency explains why the impactor failed to completely shatter the Moon, leaving its metallic iron core buried under the basin floor instead. \[12, 13, 14\]

## **4\. Determining the Time (Radioactive Decay)**

To calculate exactly *when* this blast happened, scientists use the **Radioactive Decay Law** on isotopes found inside basin-melt samples (like those from the Chang'e-6 mission and lunar meteorites):  
$$N(t) \= N\_0 e^{-\\lambda t}$$  
Where: \[2, 3\]

* $N(t)$ \= remaining parent atoms (e.g., Uranium-238)  
* $N\_0$ \= original number of atoms  
* $\\lambda$ \= decay constant  
* $t$ \= time elapsed since the impact solidified the rock

By solving for $t$, scientists calculate the exact age of **4.32 to 4.33 billion years**. \[2, 3\]

---

If you want to dive deeper, we can explore **how NASA plans to sample these southern rubble piles** during the upcoming Artemis missions, or look at **how this blast compares to the impact that formed Mars's giant Hellas basin**. Let me know what you prefer\! \[10, 11\]

import math  
D \= 260000 *\# meters*  
v \= 13000 *\# m/s*  
rho \= 3000 *\# kg/m3*  
volume \= (4/3) \* math.pi \* (D/2)\*\*3  
mass \= volume \* rho  
energy \= 0.5 \* mass \* (v\*\*2)  
print(f"Mass: {mass:.2e} kg")  
print(f"Energy: {energy:.2e} Joules")

\[1\] [https://agupubs.onlinelibrary.wiley.com](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2024GL110034)  
\[2\] [https://pmc.ncbi.nlm.nih.gov](https://pmc.ncbi.nlm.nih.gov/articles/PMC11757148/)  
\[3\] [https://www.inceptivemind.com](https://www.inceptivemind.com/blurb/moons-largest-impact-basin-formed-over-4-32-billion-years-ago/)  
\[4\] [https://www.sci.news](https://www.sci.news/space/southward-impact-south-pole-aitken-basin-14272.html)  
\[5\] [https://www.science.org](https://www.science.org/doi/10.1126/sciadv.aea1984)  
\[6\] [https://www.earth.com](https://www.earth.com/news/moons-largest-impact-crater-south-pole-aitken-basin-is-250-miles-deep-full-of-secrets/)  
\[7\] [https://www.facebook.com](https://www.facebook.com/Spacewalk2021/posts/425-billion-years-ago-this-is-when-the-south-pole-aitken-basin-spabasinthe-moons/1209040851225651/)  
\[8\] [https://www.facebook.com](https://www.facebook.com/newscientist/posts/the-impact-that-carved-out-the-south-pole-aitken-basin-on-the-moon-appears-to-ha/1242378471264101/)  
\[9\] [https://www.nature.com](https://www.nature.com/articles/s41586-025-09582-y)  
\[10\] [https://www.newscientist.com](https://www.newscientist.com/article/2499287-the-moons-largest-crater-didnt-form-in-the-way-we-thought/)  
\[11\] [https://www.linkedin.com](https://www.linkedin.com/posts/phys-org_the-moons-largest-impact-crater-scattered-activity-7458588364586450945-y8NU)  
\[12\] [https://www.sciencedirect.com](https://www.sciencedirect.com/science/article/abs/pii/S001910351200214X)  
\[13\] [https://ntrs.nasa.gov](https://ntrs.nasa.gov/api/citations/20120012900/downloads/20120012900.pdf)  
\[14\] [https://www.facebook.com](https://www.facebook.com/newscientist/posts/the-impact-that-carved-out-the-south-pole-aitken-basin-on-the-moon-appears-to-ha/1239513798217235/)