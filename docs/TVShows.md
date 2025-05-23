# Implementation of TV Show Metadata with Posters and Title Cards

This configuration should provide information on the metadata regarding TV Shows and Episodes. 

** Features **
- Movie Posters and backgrounds
- Resolution and Audio Quality
- Season specific Title Cards
- Working and Personalized metadata

## Implementation

  TV Shows:
    collection_files:
      - url: https://raw.githubusercontent.com/s0len/meta-manager-config/main/collection_files/better_new_and_old_tv_shows_releases.yml
    overlay_files:
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
      - url: https://raw.githubusercontent.com/s0len/meta-manager-config/main/overlays/network_fallback.yml
      - pmm: network
        template_variables:
          horizontal_align: left
          horizontal_offset: 0
          vertical_offset: 0
          vertical_align: top
          back_width: 1000
          back_height: 1500
          url: https://raw.githubusercontent.com/s0len/meta-manager-config/main/overlays/network-top-left/<<key>>.png 
          back_color: 00

## Preview