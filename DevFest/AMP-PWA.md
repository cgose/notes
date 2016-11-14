# AMP
## Why web
- user acquisition is lower
- always up to date
- cross-platform
- 

## Problems
- non-responsive
- different devices with different capabilities
- Load times
- 53% of users bounce from sites that take longer than 3 seconds to Load
- 19 sec average load times
- 50% are ad related
- 77% mobile sites take longer that 10s to load
- People thing internet = free

## Monetization vs User Experience
- Agressive ad, analytics and beacon blockers
- deathtobullshit.com
- walled content distribution platforms

## The ideal user journey
### Speed Source
- AMP (Accelerated Mobile Pages)
  - One http request to load Pages
  - Use Http2 through AMP Cache
  - 3rd party javasscript allowed in sandboxed iframes
  - Optimizes to resources currently in view
  - Reserves space on Pages
- Caching
  - Edge server caches at multiple locations world wide
- Pre-rendering
  - Pre rendering can make loding instant
### Missing Device capabilities
- Capabiliy and Reach
  - mobile apps highly capable
  - web highly reachable not very capable
  - How do we get web to be more capable
    - reliability
    - Push notifications
    - Add to home screen
    - Authentication Signing in
    - Payment
### Progressive Web Apps
- Service worker works independent of the web browser
- Web manifest (add to home screen)
- Signing in is a big pain point for users
  - 54% users will quit before doing another setup
- Credential Manager API: Make sign in easy.

### AMP vs PWA
- AMP 
 - Better user experience with AMP
 - Over 1000 AMP articles every day
 - instant delivery, optimized discovery, no user scripts, static content
- PWA
 - 3x more time spent on sites
 - 3 x lower
### AMP to PWA
- AMP syntactic sugar (custom components)
- Validation is key
 - Append #developer=1 to url see validation results in chrome devtools
- AMP for desktop too !!!!
### Level 2
- Javascript runs in service worker
- install service worker
- application panel of chrome dev tools
- intercept requests
### Level 3
- Manifest.json
- Cache isn't unlimited
- AMP forces inlining of css
### Level 5
- reroute. Intercept requests to serve data
# Resources
- Look up making offline web applications
- Chrome dev summit in November
- github amphtml examples
- ampproject.org/docs
- developer.google.web
- @pbaukus


