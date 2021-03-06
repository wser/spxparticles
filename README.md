# spxparticles
**Stream or a burst of image particles on HTML canvas**

Simple Javascript library for generating an infinine stream or a burst of image based particles on a HTML canvas. Only visible particles remain in memory to manage memory usage and browser performance. 

Please note: GIF animations on this page are running at low frame rate and does not make justice to an actual animation.

## Usage
    <script type="text/javascript" src="js/spxparticles.js"></script>
    <script>
        window.addEventListener('DOMContentLoaded',(e) => {
        spawnSPXParticles('SPX_ParticleCanvas');
        });
    </script>
    <canvas id="SPX_ParticleCanvas"></canvas>

![spxparticles screenshots](https://github.com/TuomoKu/spxparticles/blob/master/screenshots/SPXparticles-smoke.gif)

## Example configuration #1:
    var spxParticleSettings = {
        p_texture     :  '../img/fb-haha.png', 
        p_blending    :  'color-dodge',   /* (empty), screen, overlay, multiply, color-dodge... */
        emit_delay    :  30,              /* Delay between each new particle (performance warn!)  */
        emit_left     :  10,              /* Emitter zone left % */
        emit_right    :  90,              /* Emitter zone right % */
        emit_top      :  80,              /* Emitter zone top % */
        emit_bottom   :  90,              /* Emitter zone bottom % */
        zone_visible  :  false,           /* Preview emitter zone on canvas */
        gravity       :  -4,              /* Y move speed (negative: up) */
        rnd_grav_mult :  2,               /* Random speed multiplier */
        spread_x      :  0.5,             /* Dispersion value */
        wind          :  2,               /* Horizontal push force */
        wave_size     :  1,               /* Size of wavy motion */
        wave_freq     :  80,              /* Speed of wavy motion */
        p_life        :  250,             /* Maximum particle lifespan duration */
        p_rnd_life    :  20,              /* Randomize lifespan */
        p_size        :  110,             /* Particle born size in pixels */
        p_rnd_size    :  80,              /* Randomize size */
        p_size_mult   :  0.98,            /* Size multiplier, scale down/up gradually */
        p_rotation    :  0,               /* Spawn rotation (deg) */
        p_rnd_rot     :  15,              /* Randomize rotation (deg) */
        p_rot_wobble  :  true,            /* wobble back and forth? */
        p_rot_amount  :  1.2,             /* Rotation speed */
        p_rot_wofreq  :  40,              /* Wobble frequency */
        p_rot_dual    :  false,           /* both directions CW and CCW */ 
        p_opacity     :  100,             /* Opacity of a particle when born (%) */
        p_rnd_opa     :  0,               /* Randomize born opacity (%) */
        p_opa_mult    :  0.8,             /* Opacity multiplier, fade gradually */
        p_fade_start  :  150,             /* When do we start to fade out */
        p_rnd_fstart  :  20               /* Randomize fade start age */
    };


## Demos:

![spxparticles screenshots](https://github.com/TuomoKu/spxparticles/blob/master/screenshots/spxparticles_screenshots.jpg)

Demo 1 (index.html) : [smiley faces](https://smartpx.fi/demos/spxparticles/) rising up

Demo 2 (demo-2.html) : [stars falling](https://smartpx.fi/demos/spxparticles/demo-2.html) downwards, emitter zone visible

Demo 3 (demo-3.html): [disco](https://smartpx.fi/demos/spxparticles/demo-3.html) flashing lights

Demo 4 (demo-4.html): click handler to [emit few particles](https://smartpx.fi/demos/spxparticles/demo-4.html)

Demo 5 (demo-5.html): [smoke drifting](https://smartpx.fi/demos/spxparticles/demo-5.html) from left to right



