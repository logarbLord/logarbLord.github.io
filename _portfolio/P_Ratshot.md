---
title: "Ratshot"
order: 2
excerpt: "A breakdown of how I made my ratshot models. <br/><img src='/images/Portfolio Images/icons500x300/RatshotIcon.png'>"
collection: portfolio
---

[comment]: <> (Talk about how it started and how it blew out of control. 50bmg -> all non-shotgun calibers 50 bmg original meme vs model image took 2 months off and on restarted multiple times after learning new processes for game model making and texturing.)

The first rat shot mod ([Ratshot of Unusual Size](https://sp-mod.com/mod/2561/ratshot-of-usual-size)) was just for .50 BMG after seeing a meme image of a ratshot variant, 
but shortly after posting it, my 'friends' brought up the idea of making ratshot for all calibers. Two months, 3 blend files, 2 substance files, and dozens of restarts later, I released the final mod [Ratshot of usual size](https://sp-mod.com/mod/2487/ratshot-of-unusual-size). Which I had my friend [bushtail](https://bushtail.ca) publish so I wouldn't have to maintain the code, lol. <br/>
<br/> 
While there was nothing too worthwhile for modeling the bullet casings, working with the shell-shot was certainly a challenge! 
I quickly realized simulating the pellets into the plastic tips was not going to work, so I dipped my toes into geometry nodes. 
After _many_ revisions I ended up using this node tree for my final result. <br/>
<figure style="display: flex; flex-direction: column; align-items: center;">
    <img src='/images/Portfolio Images/P_Ratshot/Old_Geonode_Screenshot.png'
    alt="Geometry Node Image"
    width="400" />
        <figcaption style="text-align:center">
            Geometry node for pellets
        </figcaption>
</figure>
Though to be noted, I recall having to make a different tip mesh, separate from the plastics, for this to fill the tips how I was wanting. <br/>
After having made the geometry nodes, what was left was to simplify the now-realised nodes into a game-ready mesh. 
The process that I ended up following was to use a boolean modifier to merge the mesh into one single object. 
Then using the mesh that the node was generated on as a boolean collider and voiding what the mesh came in contact with, 
thus making a hollow object. After which, using a decimate modifier until the vertex count dropped to an acceptable amount. 
(I set sub 7k verts my goal on every caliber except for .338 lapua and .50bmg) <br/>
<figure style="display: flex; flex-direction: column; align-items: center;">
    <img src='/images/Portfolio Images/P_Ratshot/tkm_UV.png'
    alt="UV of the tkm model"
    width="200"
    >
        <figcaption style="text-align:center">
            UV Map of 366TKM
        </figcaption>
</figure>
When making the UVS, a hurdle I faced was properly UV-packing the meshes, but I think the final result is acceptable. 
Though if there was one thing I could go back and change, I'd properly island the UVS of the spent shell casings. 
The bullet casings for both the live and spent shells use the same material and are stacked aside from the spent primer. <br/>
Why not go back and fix it? Because I'd be obligated to re-make the bundles and update my mod. Not gonna happen haha.<br/>
<br/>
After making the bullets, I decided that instead of re-texturing the base game ammo packs, I'd make my own models from scratch.
From a flat plane to a box shape, I added a solidify modifier to give them depth similar to a cheap cardboard box and bevelled them for some additional smoothness.
A large focus of these specific meshes was 'expandability'- what I mean by this is that I could manually scale the meshes in vertex mode to get the models to whatever size needed for the bullets.<br/>
Speaking of, all the ammunition boxes for my mod are to (bullet) scale! See the images below.<br/>
<figure>
    <img src='/images/Portfolio Images/P_Ratshot/BulletBoxTrueScaleProof.PNG'
    alt="Bullet Box with Patrons"
    width="400px"> <br/>
    <div style="display:flex; justify-content:center; gap:10px;">
        <img src='/images/Portfolio Images/P_Ratshot/BigBoxTemplateB.PNG'
        alt="Image of the Big Box Template model"
        width="32%">
        <img src='/images/Portfolio Images/P_Ratshot/BigBoxTemplateA.PNG'
        alt="Image of the Big Box Template model with Thumb Holes"
        width="32%">
        <img src='/images/Portfolio Images/P_Ratshot/LongBoxTemplate.PNG'
        alt="Image of the Long Box Template model"
        width="32%">
    </div>
        <figcaption style="text-align:center">
            Box Templates
        </figcaption>
</figure>

<br/>
One last thing I'd like to brag about is that on every box; The Grain is calculated to the estimated projectile weight, and all the barcodes are custom per caliber. Keep an eye out on the boxes ;) <br/>
<figure>
    <video controls width="100%">
            <source src="/images/Portfolio Images/P_Ratshot/RatshotModelShowcase.mp4" type="video/mp4">
            Your browser does not support the video tag.
    </video>
</figure>