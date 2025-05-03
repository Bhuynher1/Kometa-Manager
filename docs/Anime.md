# Implementation of Anime Metadata with Posters and Title Cards

This configuration should provide information on the metadata regarding Anime and Episodes. 

** Features **
- Anime posters and backgrounds
- Resolution and Audio Quality
- Season specific Title Cards
- Working and Personalized metadata

## Implementation

  Anime:
   overlay_files:
     - url: https://raw.githubusercontent.com/Bhuynher1/Kometa-Manager/main/overlays/studio_top_left.yml
     - pmm: status
       template_variables:
         text_airing: .
         url_airing: https://raw.githubusercontent.com/s0len/meta-manager-config/main/overlays/status-top-left/airing.png
         text_returning: .
         url_returning: https://raw.githubusercontent.com/s0len/meta-manager-config/main/overlays/status-top-left/returning.png
         text_canceled: . 
         url_canceled: https://raw.githubusercontent.com/s0len/meta-manager-config/main/overlays/status-top-left/cancelled.png
         text_ended: .
         url_ended: https://raw.githubusercontent.com/s0len/meta-manager-config/main/overlays/status-top-left/ended.png
         horizontal_align: left
         horizontal_offset: 25
         vertical_align: top
         vertical_offset: 0
         font_size: 1
         font_color: '#00000000'
         back_color: '#00000000'
         back_width_airing: 1000
         back_width_returning: 1000
         back_width_ended: 1000
         back_width_cancelled: 1000
         back_height_airing: 1500
         back_height_returning: 1500
         back_height_ended: 1500
         back_height_cancelled: 1500
         final_horizontal_offset: 0
         final_vertical_offset: 0

## Preview