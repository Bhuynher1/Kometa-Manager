# Implementation of Movie Metadata with Posters and Title Cards

This configuration should provide information on the metadata regarding Movies and Movie Collections. 

** Features **
- Movie Posters and backgrounds
- Resolution and Audio Quality
- Season specific Title Cards
- Working and Personalized metadata

## Implementation

  Movies:
    collection_files:
      - url: https://raw.githubusercontent.com/s0len/meta-manager-config/main/collection_files/better_new_and_old_movie_releases.yml
      - pmm: content_rating_cs
        template_variables:
          use_separator: false
          collection_mode: hide
          url_poster: https://raw.githubusercontent.com/s0len/meta-manager-config/main/posters/commonsense/<<key>>.jpg
    overlay_files:
      - url: https://raw.githubusercontent.com/s0len/meta-manager-config/main/overlays/background_top_left_313_wide.yml
      - pmm: resolution
        template_variables:
          url: https://raw.githubusercontent.com/s0len/meta-manager-config/main/overlays/resolution-top-left-45deg/<<overlay_name>>.png
          horizontal_align: left
          horizontal_offset: 0
          vertical_offset: 0
          vertical_align: top
          final_horizontal_offset: 0
          final_vertical_offset: 0
          back_width: 1000
          back_height: 1500
          back_color: 00
      - pmm: audio_codec
        template_variables:
          url: https://raw.githubusercontent.com/s0len/meta-manager-config/main/overlays/audio-top-left-45deg/<<key>>.png
          horizontal_align: left
          horizontal_offset: 0
          vertical_offset: 0
          vertical_align: top
          back_width: 1000
          back_height: 1500
          back_color: 00
      - url: https://raw.githubusercontent.com/s0len/meta-manager-config/main/overlays/ribbon_rotten.yml

## Preview