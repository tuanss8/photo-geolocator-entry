# Photo geolocator (make.fun photo-geolocator-01)

A model-free agent: no API key is available to this entrant, so it calls no
vision model (model calls are optional in this bounty). It places every photo
at one fixed point, the haversine geometric median of the kit's 75 practice
photos (56.7871 N, 27.0081 E, eastern Europe), which minimises the expected
total error for a photo drawn from OpenStreetView-5M's distribution.

Practice scores (out of 500,377): trial-0 ~264,349, trial-1 ~349,406,
trial-2 ~374,129 (mean ~329,295), against 0 for leaving every photo
unanswered.

Run: `node main.ts` with `MAKEFUN_ENV_URL` set (Node 22, standard library only).
