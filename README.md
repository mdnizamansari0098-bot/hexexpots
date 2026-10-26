# HEX ESPORTS

| File | Kaam |
|---|---|
| `index.html` | Player app (GitHub Pages ka main link) |
| `admin.html` | Admin panel |
| `staff.html` | Staff panel |
| `server/` | HexPay payment server (Render/Railway par alag deploy karo, GitHub Pages par nahi chalta) |

## GitHub Pages
Settings > Pages > Deploy from a branch > `main` / `(root)` > Save.
Link: `https://<username>.github.io/<repo>/`

## Firebase
Authentication > Email/Password ON. Authorized domains me `<username>.github.io` add karo. Firestore Database banao (Mumbai).

## Payment server
1. `server/` ko Render/Railway par deploy karo (Node 18+, build `npm install`, start `npm start`).
2. Env vars `server/.env.example` jaise set karo. Service-account JSON aur API key kabhi repo me commit mat karo.
3. `index.html` me `HEX_SERVER` me server ka https URL daalo.

## Pehli baar
`admin.html` kholo, Register as Admin se pehla admin banao (wahi lock ho jata hai).
