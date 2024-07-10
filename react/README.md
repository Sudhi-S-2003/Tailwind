Create your project
--------------------
npx create-react-app my-project
cd my-project

Install Tailwind CSS
-----------------------

npm install -D tailwindcss
npx tailwindcss init

Configure your template paths
------------------------------
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: [
    "./src/**/*.{js,jsx,ts,tsx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}

Add the Tailwind directives to your CSS
-----------------------------------------
@tailwind base;
@tailwind components;
@tailwind utilities;

Start your build process
-------------------------
npm run start

Start using Tailwind in your project
-------------------------------------
<code>
export default function App() {
  return (
    <h1 className="text-3xl font-bold underline">
      Hello world!
    </h1>
  )
}
</code>