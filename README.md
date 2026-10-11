# Torque_Bay

Torque Bay is a workshop for modifying bikes and cars, built as a single web page.

**Live site: https://premuthung.github.io/Torque_Bay/**

- Pick one of 14 bikes and cars and put it on the lift.
- Swap parts at eight stations (exhaust, intake, fuelling, gearing or turbo, wheels, suspension, brakes, body).
- Each part has a job card: whether it fits, what it takes to make it fit, what you gain, what you lose and what to do instead.
- Twelve speedometer dials show the effect on power, torque, top speed, 0 to 100 km/h, weight, sound, handling, braking, reliability, mileage and cost.
- The test strip runs your build over 400 m against the stock vehicle, with engine sound that follows the exhaust you fitted. Auto run sends both to top speed and back to a stop and compares the results.
- The 3D wind tunnel shows how outer body parts (lip, wing, diffuser, roof box, screen, luggage) change the airflow, drag and downforce.

## Hosting

The site is served by GitHub Pages from the `gh-pages` branch, which mirrors `main`. To publish a change, push it to both:

```bash
git push origin main main:gh-pages
```

## Run it locally

Serve the folder and open it in a browser:

```bash
python -m http.server 8780
```

Then visit http://localhost:8780/.

## About the numbers

Stock figures are approximate. The dials and the test strip come from a simplified model (percentage gains per part, power to weight, gearing limits). They show the direction and rough size of a change. They are not dyno results.

The wind tunnel uses one generic car shape and one generic bike, with streamlines drawn from the body outline. It is a picture of how the air behaves, not a fluid simulation, and its drag and downforce figures are typical values for each kind of part.

## Photos

Vehicle and part photos in `img/` are from Wikimedia Commons, cropped and resized. Author, licence and source link for each are listed in the page footer and in the `PHOTO` table in `index.html`. Most are CC BY or CC BY-SA, which require that credit to stay with them.

`img/hero-bg.jpg` is a stock-site image supplied by the project owner. Check its licence before reusing it.
