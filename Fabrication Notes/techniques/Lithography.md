Lithography is pattering on a material or substrate. It is used in order to create protective patterns or etch designs into materials.  In microfabrication there are several types of lithorgraphy. Mainly:

- Photolithography (Optical; DUV, EUV)
	- The most widely used method in semiconductor manufacturing
	- Uses a mask to transfer (block or allow pass through) certain patterns onto a [[Photoresist|photoresist]] covered substrate 
	- Can create small features, typically a few nanometers depending on the technique
	- Relatively easy to scale to production (hence why everyone uses it)
	- Feature size of ~7-200 nm
- X-Ray Lithography
	- Can create very small features (0.1 - 10 nanometers)
	- Less common due to high cost and complexity
	-  [[Photoresist|Photoresist]] is used. Uses a mask to transfer features
- Electron Lithography
	- Maskless
	- Can create features around 1-10 nanometers
	- Very slow 
	- Generally used for either prototyping or mask production for photolithography at scale (since you only need one mask per design per photolithography station)
	- Uses e-beam resist (specially made resist that behaves similar to photoresist). Electrons break the bonds which makes the substrate soluble
- Ion Beam Lithography
	- Extremely high resolution and can be used for etching (<10 nanometers)
	- Very slow and hard to scale to production
	- Can use resist or can be resistless
	- Uses no masks
	- Directly sputters ions from the substrate
- Scanning Probe Lithography
	- Atomic level precision (<1nm )
	- Scratches the surface of the substrate to etch 
	- Extremely slow and not scaleable. Only used in research cases typically


#### Notes on Photolithography

Photolithrography is organized into:
- Contact Printing
- Proximity Printing
- Projection Printing

In the first two methods, the mask is brought close to the substrate for masking off the light. In contact, the mask is allowed to touch the photoresist layer. The resolution $b$ is depends on the wavelength $\lambda$ and the distance $s$ between the mask and photoresist layer:

$b = 1.5 \sqrt{\lambda s}$  (Contact and Proximity Printing Resolution)

For projection printing we can use

$b = \frac{\lambda s}{2NA}$ 

Where $NA$ is the numerical aperture of the imaging lens system


#### Notes on Resist Thickness for lithography

Resist thickness depends on the type of device you are making. Certain devices need thicker resists (or a higher aspect ratio between feature widths and depths, or feature widths and resist thickness) such as microfluidics. This is because microfluidics typically use resist as a structural material such as with SU-8 (negative photoresist). Tuning this property can be done by applying multiple coats or by changing spin coating RPMs or changing viscosity of the photoresist.
