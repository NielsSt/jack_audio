# 
# nologo aka niels.stjernborg@gmail.com
# for
# jack_audio
# startup & shutdown sh
# for QjackCtl Archlinux, setup scripts
#  
#    The flow of how this setup works:
#
#    PulseAudio releases the sound card
#    JACK grabs sound card and starts up
#    script redirects PulseAudio to JACK
#    manually send PulseAudio apps to JACK output (pavucontrol may come in helpful for this)
#    use JACK programs etc
#    via script, stop redirecting PulseAudio to JACK
#    stop JACK and release sound card
#    PulseAudio grabs sound card and reroutes audio t
#   
# See https://wiki.archlinux.org/index.php/PulseAudio/Examples#PulseAudio_through_JACK 
#
#
