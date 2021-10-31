# pyimgui-overlayable
Draw over imgui images

# Example
    import imgui
    import from overlayable import *
    ...
    
    # calls down to imgui.image() under the hood
    image_overlayable = draw_overlayable_image(texture_id, image_pixel_width, image_pixel_height, imgui_display_width)
    
    # calls down to imgui.get_window_draw_list().add_circle() under the hood
    # but transforms the coordinates from image pixel space to screen space
    overlay_circle(image_overlayable, pixel_x, pixel_y, pixel_radius, color=..., thickness=...)
