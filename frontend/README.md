# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

1. vite+react (npm create vite@latest .)
2. npm install express dotenv cookie-parser bcryptjs mongoose socket.io jsonwebtoken
3. "scripts": {
    "server": "node backend/server.js"
  }, npm run server
4. npm i nodemon --> route changes reflect aagurathukkaga every time terminal kill pannittu re run panna venum auto rerun pannirum intha package
5. JWT token
   ====================
   const generateTokenAndSetCookie = (userId, res) => {
    const token = jwt.sign({userId}, process.env.JWT_SECRET, {
        expiresIn: '15d'
    })

    res.cookie("jwt",token,{
        maxAge: 15 * 24 * 60 * 1000, //ms
        httpOnly: true, //prevent XXS attacks cross-site scripting attacks
        sameSite:"strict", // CSRF attacks cross-site request forgery attacks
    })
  };

  openssl rand -base64 32 (generate from bash)
  37vrDkLjYq839NrmD4Wxzoj+LD9vKttB6+/NU8qduq4=(sample key)

6. send msg and get msg

Frontend(React+Vite, Daisy UI, tailwind css)
1. Install rect_vite
2. Config tailwind css
3. install daisy ui


