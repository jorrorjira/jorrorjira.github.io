# Transitions.dev motion used in this portfolio

Copyright (c) 2026 Jakub Antalik / Transitions.dev.
Source: https://github.com/Jakubantalik/transitions.dev/tree/6a7d68260d624eb66661cc3af17e0989476f48ae
Terms: https://transitions.dev/terms.html — complete upstream license: [TRANSITIONS-LICENSE.txt](./TRANSITIONS-LICENSE.txt).

Only four free recipes from `cli/free/` are adapted into this website:

- `modal.md`: 250ms entry / 150ms exit, scale0.96, cubic-bezier(0.22,1,0.36,1). Native language/recovery dialogs use CSS starting styles plus discrete display/overlay transitions instead of closing timers. The media viewer keeps its existing GSAP cleanup/focus lifecycle with the same scale/easing.
- `panel-reveal.md`: 400ms entry / 350ms exit and the same easing. Travel is reduced to16px; the large work panel does not animate blur. Only its content translates, not the fixed Close control. Existing camera timing and project-swap interruption guards remain.
- `tabs-sliding.md`: 250ms measured active indicator. Adapted to the portfolio's gold underline rather than a new pill design. Both axes support wrapped rows. The existing ResizeObserver snaps it on layout/font changes; existing pressed filter-button semantics remain (not a tablist).
- `menu-dropdown.md`: 250ms entry / 150ms exit, top-right origin and scale0.97. The native Switch view details disclosure retains keyboard behavior and preview-video pause handling. Closing also uses0.97 to avoid a separate transient class/timer.

All respect prefers-reduced-motion, including live changes. Native dialog animation is progressive enhancement: unsupported discrete transitions retain a static, functional native dialog. No new framework, runtime package, external script, Pro recipe, Transitions.dev branding or demo imagery is included. This is a portfolio website, not a redistributed transitions library or template product.
