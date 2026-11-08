# Surprise Gift Box 🎁

An interactive 3D gift box website. Send a personal surprise to someone you love with just a link.
Built with plain **HTML, CSS and JavaScript**. No frameworks, no build step.

## What the receiver sees

1. A glowing 3D gift box with floating stars. They tap **OPEN YOUR GIFT**.
2. The lid opens, light shines out, and confetti and hearts fly.
3. A message card with the receiver's name and a personal message.
4. A photo gallery with polaroid frames, 3D hover and a full-screen preview.
5. A secret envelope that opens and types out a letter.
6. A final screen with a glowing heart and a replay button.

## Features

- Real CSS 3D gift box (no images needed)
- Confetti, hearts, shooting stars and floating sparkles
- Photo gallery with full-screen preview (arrow keys and Esc work)
- Different watermark photo behind each section
- 4 colour themes: aurora, rose, ocean, forest
- Works on phones, tablets and desktops
- Keyboard friendly and respects "reduced motion" settings
- No tracking, no backend, no external libraries (only Google Fonts)

## Project files

```
surprise-gift-box/
├── index.html     page structure
├── style.css      all design and animation
├── script.js      all behaviour (edit the DEF object to change the gift)
├── images/        your photos (photo1.jpg ... photo4.jpg)
└── README.md
```

## How to personalise a gift

Open `script.js` and find the `DEF` object near the top:

| Field      | What it changes                         |
|------------|-----------------------------------------|
| `receiver` | Name of the person receiving the gift   |
| `sender`   | Your name                               |
| `title`    | Big heading, for example "Happy Birthday!" |
| `message`  | The message card text                   |
| `letter`   | The secret letter text                  |
| `closing`  | The last line on the final screen       |
| `theme`    | `aurora`, `rose`, `ocean` or `forest`   |
| `photos`   | List of `{src, cap}`: image path and caption |

To use your own photos, put them in the `images/` folder and update the `src` paths.
Square or portrait photos around 600 to 800 px wide work best.

> Tip: make one copy of the folder for each customer, and change only `DEF`.

There is also a built-in editor in the code (`#custBtn`). It is hidden by default with CSS.
To show it for yourself, remove `.cust{display:none!important}` from `style.css`.



## License

Free to use and change. Only use photos you have permission to share.
