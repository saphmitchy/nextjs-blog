---
title: Euler–Lagrange equation
date: '2023-08-22'
---

$$
\global\def\diff{\mathrm{d}}
\global\def\eps{\varepsilon}
\global\def\del{\delta}
\global\def\dotx{\dot{x}}
\global\def\pd#1#2{\frac{\partial #1}{\partial #2}}
\frac{\diff}{\diff\eps}\int_{a}^{b}{f(\dotx+ \eps\dot{\del}(t), x + \eps\del(t), t)\diff x} \\
= \int_{a}^{b}{\left(\dot{\del}(t)\pd{f}{\dotx} + \del(t)\pd{f}{x}\right) \diff x} \\
= \left[ \del(t)\pd{f}{\dotx} \right]^b_a + \int_a^b{\left(-\del(t)\frac{\diff}{\diff t}\pd{f}{\dotx} + \del(t)\pd{f}{x}\right)\diff x} \\
= \del(t)\int_a^b{\left(-\frac{\diff}{\diff t}\pd{f}{\dotx} + \pd{f}{x}\right)\diff x} \\
\global\def\diff{\mathrm{d}}
\therefore -\frac{\diff}{\diff t}\pd{f}{\dotx} + \pd{f}{x} = 0
$$

