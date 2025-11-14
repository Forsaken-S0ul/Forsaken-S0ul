# 👋 Welcome to My GitHub!

✨ **"I am a** <span id="role"></span> **."**
<script>
const roles = ["game designer", "developer", "web designer"];
let current = 0;
const el = document.getElementById("role");

function glitchTransition(newText) {
  const chars = "^&!@#*$%(){}[]<>?/|";
  let iterations = 0;
  const original = newText;

  const interval = setInterval(() => {
    el.textContent = original
      .split("")
      .map((char, i) => {
        if (i < iterations) return original[i];
        return chars[Math.floor(Math.random() * chars.length)];
      })
      .join("");

    iterations++;
    if (iterations > original.length) clearInterval(interval);
  }, 50);
}

function cycleRoles() {
  glitchTransition(roles[current]);
  current = (current + 1) % roles.length;
}

cycleRoles();
setInterval(cycleRoles, 3500);
</script>

---

## 🌟 About Me

* 🛠️ **Currently Building:** an interactive project that mixes design, tech, and way too much curiosity
* 🚀 **Learning:** how to make 3D worlds come alive
* 📫 **Reach Me:** [LinkedIn](https://www.linkedin.com/in/prayash-dhungana-bb895a244/)
* 😄 **Pronouns:** She/Left
* 🎮 **Fun Fact:** I play every game like it’s my first time… every time

---

Thanks for stopping by — hope something here sparks an idea! ✨
