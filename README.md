Hello,

This is my current layer setup for a 5x12 ortholinear keyboard.
Hope this helps you in determining your own setup.


```

 default_layer {
            // ------------------------------------------------------------------------------------------
            // |  ESC  |  1*  |  2*  |  3*  |     4*    |   5*  |   6*   |    7*    |  8*  |  9*  |   0*  | BSPC  |
            // |  TAB  |  Q   |  W   |  E   |     R     |   T   |   Y    |    U     |  I   |  O   |   P   |   '*  |
            // |   `*  |  A   |  S   |  D   |     F     |   G   |   H    |    J     |  K   |  L   |   ;*  | ENTER |
            // | SHIFT*|  Z   |  X   |  C   |     V     |   B   |   N    |    M     |  ,*  |  .*  | UARW  |  /*   |
            // | LCTL  | LGUI | LALT | LOWR | 2uSpace(a)|4uSpace|  N/A** |2uSpace(b)| RAIS | LARW | DARW  | RARW  |


            bindings = <
                &kp ESC    &tdn1        &tdn2       &tdn3    &tdn4      &tdn5       &tdn6       &tdn7      &tdn8       &tdn9       &tdn0       &kp BSPC
                &kp TAB    &kp Q        &kp W       &kp E    &kp R      &kp T       &kp Y       &kp U      &kp I       &kp O       &kp P       &tdsqt
                &tdgrave   &kp A        &kp S       &kp D    &kp F      &kp G       &kp H       &kp J      &kp K       &kp L       &tdsemi     &kp RET
                &tdlshft   &kp Z        &kp X       &kp C    &kp V      &kp B       &kp N       &kp M      &tdcomma    &tddot      &kp UP      &tdfslh
                &kp LCTRL  &kp LGUI     &kp LALT    &mo 1    &kp SPACE  &kp SPACE   &kp SPACE   &kp SPACE  &mo 2       &kp LEFT    &kp DOWN    &kp RIGHT 
            >;
        };

        lower_layer {
            // -------------------------------------------------------------------------------------------
            // |   F1  |  F2   |  F3   |  F4   |    F5    |  F6   |   F7   |    F8    |  F9  | F10  |  F11  |  F12  |
            // |       |  INS  |  HOME | PG UP |          |       |        |          |      |      |  -*   |  =*   |
            // |       |  DEL  |  END  | PG DN |          |       |        |          |      |      |       |       |
            // |       |       |       |       |          |       |        |          |  [*  |  ]*  |       |   \*  |
            // |       |       |       | LOWR  |2uSpace(a)|4uSpace|  N/A** |2uSpace(b)| RAIS |      |       |       |
            bindings = <
                &kp F1     &kp F2      &kp F3      &kp F4    &kp F5     &kp F6      &kp F7      &kp F8       &kp F9    &kp F10    &kp F11    &kp F12
                &none      &kp INS     &kp HOME    &kp PG_UP &none      &none       &none       &none        &none     &none      &tdminus   &tdequal
                &none      &kp DEL     &kp END     &kp PG_DN &none      &none       &none       &none        &none     &none      &none      &none
                &none      &none       &none       &none     &none      &none       &none       &none        &tdlbkt   &tdrbkt    &none      &tdbslh
                &none      &none       &none       &mo 1     &kp SPACE  &kp SPACE   &kp SPACE   &kp SPACE    &mo 2     &none      &none      &none
            >;
        };

        raise_layer {
            // ------------------------------------------------------------------------------------------
            // | PRTSCN|       |       |       |          |BT_NXT | BT_CLR |          |      |      |        |    DEL   |
            // | C_S_E |   1   |   2   |   3   |          |       |        |          |      |   -  |   +    |          |
            // |       |   4   |   5   |   6   |          |       |        |          |      |   /  |   *    | KP ENTER |
            // |       |   7   |   8   |   9   |          |       |        |          |  [*  |  ]*  | VOL UP |    \*    |
            // | C_A_D |   .   |   0   | LOWR  |2uSpace(a)|4uSpace|  N/A** |2uSpace(b)| RAIS | PREV | VOL DN |   NEXT   |
            bindings = <
                &kp PSCRN       &none         &none      &none      &bt BT_NXT &bt BT_CLR   &none       &none        &none     &none         &none            &kp DEL
                &ctrl_shift_esc &kp KP_N1     &kp KP_N2  &kp KP_N3  &none      &none        &none       &none        &none     &kp KP_MINUS  &kp KP_PLUS      &none
                &none           &kp KP_N4     &kp KP_N5  &kp KP_N6  &none      &none        &none       &none        &none     &kp KP_DIVIDE &kp KP_MULTIPLY  &kp KP_ENTER
                &none           &kp KP_N7     &kp KP_N8  &kp KP_N9  &none      &none        &none       &none        &tdlbkt   &tdrbkt       &kp C_VOL_UP     &tdbslh
                &ctrl_alt_del   &kp KP_DOT    &kp KP_N0  &mo 1      &kp SPACE  &kp SPACE    &kp SPACE   &kp SPACE    &mo 2     &kp C_PREV    &kp C_VOL_DN     &kp C_NEXT
            >;
        };
        
```        
