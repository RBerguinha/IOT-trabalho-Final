# IOT-trabalho-Final



# Python code
#
basic.show_leds("""
  . . # . .
  . # # . .
  # # # # #
  . # # . .
  . . # . .
  """)

def on_button_pressed_a():
  basic.show_string("" + input.temperature())
  basic.show_icon(IconNames.Heart)
  basic.show_leds("""
    . . # . .
    . . # # .
    # # # # #
    . . # # .
    . . # . .
    """)
input.on_button_pressed(Button.A, on_button_pressed_a)

def on_button_pressed_b():
  basic.show_string("" + input.light_level())
input.on_button_pressed(Button.B, on_button_pressed_b)
