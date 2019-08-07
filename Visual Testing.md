# Visual Testing

## Aim

The design of the GUI is provided by a third party. This includes the UX design and accessibility. Therefore this design must match what is eventually implemented.

In addition, any unnecessary changes to the DOM will disrupt E2E test automation and may also affect UX, accessibility or the requirements.

## Guidance

No visual testing is currently being performed.

## Continuous Improvement

Snapshot testing of the DOM with Karma can be used to ensure it doesn't change accidentally. Visual Testing could be performed with BackstopJS, Gemini or Happo (and/or Applitools).
