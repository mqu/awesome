# Video-surveillance / 
Awesome links in French ; collection de liens en Français ; video-monitoring.

[TOC]

tags: NVR,  CCTV, DIY, Linux, Self-Hosted, Open-source.

# camera de surveillance

## Logiciels
- [ZoneMinder](https://zoneminder.com/) : [doc](https://zoneminder.readthedocs.io/), [wiki](https://wiki.zoneminder.com), [liste de compatibilité](https://wiki.zoneminder.com/Hardware_Compatibility_List) ; [docker](https://github.com/ZoneMinder/zmdockerfiles), [github](https://github.com/ZoneMinder/ZoneMinder/)
- [Viseron](https://viseron.netlify.app/) : self-hosted, local only NVR and AI Computer Vision software.
  - détection d'objets, reconnaissance faciale
  - [compatible home-assistant](https://community.home-assistant.io/t/viseron-self-hosted-local-only-nvr-and-ai-computer-vision-software/223152) via MQTT
  - supporte l'accélération matérielle CUDA, CORAL (TPU)
  - [installation](https://viseron.netlify.app/docs/documentation/installation) uniquement sur environnement [Docker](https://hub.docker.com/r/roflcoopter/viseron) , avec ou sans accélération matérielle ([CUDA](https://fr.wikipedia.org/wiki/Compute_Unified_Device_Architecture), [VAAPI](https://fr.wikipedia.org/wiki/Video_Acceleration_API), Google Coral Edge TPU)
  - source [github](https://github.com/roflcoopter/viseron) ; codé principalement en Python.

- [Shinobi](https://shinobi.video/) : the open-source CCTV solution ;
  - [doc](https://docs.shinobi.video/), [repository](https://gitlab.com/Shinobi-Systems/Shinobi) ;
  - [installation](https://docs.shinobi.video/installation/docker) sur Docker ;
  - 2 [versions](https://shinobi.video/pro) : community [CE](https://gitlab.com/Shinobi-Systems/ShinobiCE) et pro.
  - [description](https://linuxfr.org/news/presentation-de-shinobicctv-community-edition) (fr ; un peu ancienne)

- [Frigate](https://frigate.video/): Monitor your security cameras with locally processed AI
  - 2 version : community et [pro](https://frigate.video/plus/) (Frigate+)
  - très bonne intégration à Home Assistant ; nombreux [addons](https://www.home-assistant.io/addons/) ; 
  - plusieurs méthodes [d'installation](https://www.home-assistant.io/installation/) dont Docker et [docker-compose](https://www.home-assistant.io/installation/generic-x86-64#docker-compose).
  - [doc](https://docs.frigate.video/), [github](https://github.com/blakeblackshear/frigate). 

- Moonfire NVR : a security camera network video recorder
  - [github](https://github.com/scottlamb/moonfire-nvr), 

- motionEye : a web frontend for the motion daemon.    
  - [github](https://github.com/motioneye-project/motioneye)

- Motion : Motion is a highly configurable program that monitors video signals from many types of cameras.
  - [doc](https://motion-project.github.io/), [github](https://github.com/Motion-Project/motion)

- [JeVois](http://jevois.org/)
  - accélération matérielle CORAL ;
  - [dépot](https://github.com/jevois/jevois) Github ; écrit en C, C++ ; solution miniaturisée.


domotique

- [Home Assistant](https://www.home-assistant.io/) : 
  - slogan : Open source home automation that puts local control and privacy first. 
  - [démo](https://demo.home-assistant.io/), [doc](https://www.home-assistant.io/docs/), [compatibilité et intégration](https://www.home-assistant.io/integrations/), [github](https://github.com/home-assistant), [docker](https://hub.docker.com/r/homeassistant/home-assistant), [openhub](https://www.openhub.net/p/home-assistant) ;
  - alternatives : [IoBroker](https://www.iobroker.net/), [OpenHAB](https://www.openhab.org/), [CometVisu](https://www.cometvisu.org/), [Domoticz](https://domoticz.com/), [Jeedom](https://jeedom.com/en/). Faire son choix en matière de [controleur domotique](https://blog.bemotique.com/comment-choisir-un-controleur-domotique/).

# accélération matérielle

tags: Intelligence Artificielle, réseau de neuronnes, Tensorflow, TPU

- https://coral.ai/products/accelerator : accélérateur USB / Coral.

- Intel NCS2 : accélérateur USB TPU / [description](https://www.lemondeinformatique.fr/actualites/lire-intel-sort-son-deuxieme-neural-compute-stick-73430.html).

- [Intel Movidius Myriad X](https://www.intel.fr/content/www/fr/fr/products/details/processors/movidius-vpu/movidius-myriad-x.html).

## comparatifs
- https://www.lesnumeriques.com/camera-surveillance.html
- https://community.home-assistant.io/t/my-opinion-zoneminder-vs-motioneye-vs-shinobi/316831
- https://blog.desdelinux.net/fr/shinobi-un-servidor-de-video-vigilancia-open-source/
- https://community.home-assistant.io/t/my-opinion-zoneminder-vs-motioneye-vs-shinobi/316831
- https://www.makeuseof.com/tag/awesome-diy-security-camera-clients-linux/
- https://www.ubuntupit.com/best-linux-camera-software/
- https://linuxpip.org/open-source-nvr/
- https://medevel.com/10-cctv-open-source-solutions/

# liens
- Github / [motion-dectection](https://github.com/topics/motion-detection).
- Openhub : [zoneminder](https://www.openhub.net/p/zoneminder), [mition-eye](https://www.openhub.net/p/motioneye), [iSpy-Motion](https://www.openhub.net/p/ispysoftware), [motion](https://www.openhub.net/p/Motion).
- reconnaissance / IA :
  - Darknet / [YOLO](https://pjreddie.com/darknet/yolo/) : système de reconnaissance d'objets temps-réel ; [doc](https://thedatafrog.com/fr/articles/object-detection-darknet/) ; nécessite CUDA+OpenCV.


# Glossaire
- NVR : Network Video Recorder, enregistrement vidéo via le réseau ;
- [PTZ](https://fr.wikipedia.org/wiki/Cam%C3%A9ra_pan_tilt_zoom) : Caméra orientable (Pan Tilt Zoom) ;
- CCTV : Closed-Circuit TV ; système de TV privé ;
- TPU : Tensor Processing Unit ([WP](https://fr.wikipedia.org/wiki/Tensor_Processing_Unit)) : unité de traitement d'intelligence artificielle basé sur [Tensorflow](https://fr.wikipedia.org/wiki/TensorFlow) permettant l'accélération matérielle ;
- [ONVIF](https://en.wikipedia.org/wiki/ONVIF) : Open Network Video Interface Forum : forum de standardisation des moyens de video-surveillance sur réseau IP ([lien](https://www.onvif.org/)) ; [lien-fr](https://camera-videosurveillance.fr/blog/143_Qu-est-ce-que-le-protocole-onvif.html).
  - [enregistreur vidéo](https://fr.aliexpress.com/item/1005004317130185.html) basé sur le standard ONVIF.
  - [nombreuses cameras IP compatibles ONVIF](https://fr.aliexpress.com/premium/onvif.html).
- [MQTT](https://fr.wikipedia.org/wiki/MQTT) : bus logiciel très simple largement utilisé au niveau de IOT (Internet des Objets) et domotique.
