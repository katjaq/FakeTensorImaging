# Hypothesis-driven white matter tractography from T1-weighted MRI images

Anastasia Osoianu, Charl Linssen, Katja Heuer, Roberto Toro



Background: Polarized light imaging (PLI) as well as the tractography of high angular resolution diffusion weighted imaging (DWI) data reveal a geometry of striking regularity. This makes the neuroanatomist wonder whether it would be possible to generate a connectome based exclusively on a small set of hypotheses:
more than 90% of white matter connections are cortico-cortical;
the density of fibres is homogeneous throughout the white matter;
fibres are oriented perpendicular to gyral crowns and parallel to sulcal fundi;
fibres are sticky, which makes them aggregate in bundles of similar orientation.
How much of a real brain connectome would be recovered by such a simple and reductionistic model?

Project aims: We propose to approach this question in the simple case of a 2D coronal slice. We will propagate random particles constrained by the above assumptions and calculate a direction map from the average orientation of the fibres at each voxel, and introduce a smoothing term where the orientation of each individual fibre tends to the local average. This process will produce a tensor field which will be then used to propagate a new set of fibres in an iterative manner. We will test our model in coronal slices of mouse, macaque, chimpanzee and human slices for which we have both T1-weighted and DWI data. We will also use one PLI slice from a vervet monkey for validation.

Methods: In a first step, we will use a Monte Carlo (MC) method to place particles on a randomly chosen point on the pial surface, and from there they will propagate into a random direction within the white matter mask. During numerous iterations of this step, we will update a density map (figure, left) and a direction map (right). Tensors will be formulated as quaternions to simplify the computations, in particular the local smoothing. The MC process will then be repeated taking into account the maps computed in the previous MC run.






