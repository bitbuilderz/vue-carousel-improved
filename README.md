# Forked Vue Slick Carousel with active maintaining and fixed issues

## Fixed problems:

- slick autoplays in Chrome even if prop autoplay is set to false (https://github.com/gs-shop/vue-slick-carousel/issues/229)
- on mobiles after orientation change carousel is not properly resized
- unwanted animation stop and slider reset when scrolling page on mobiles

## Added:
- arbitraryRewind flag to allow proper rewinding to a random slide over the limit of the number of slides (when the infinite flag is true). With arbitraryRewind = false, scrolling to an element outside the slider's bounds results in a scroll to element zero index. With arbitraryRewind = true, scrolling occurs to the desired element

| Prop name        | Description                                                                                                                                                                      | Type    | Values                | Default      |
| ---------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------- | --------------------- | ------------ |
| arbitraryRewind  | rewind to any slide                                                                                                                                                              | boolean | -                     | false        |