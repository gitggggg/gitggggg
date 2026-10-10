- 👋 Hi, I’m @gitggggg
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...123
- 📫 How to reach me ...11

<!---
gitggggg/gitggggg is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

const wait = (time = 1500) => {
    return new Promise((resolve) => {
        setTimeout(() => {
            resolve()
        }, time)
    })
}
const closeWindow = () => {
  var userAgent = navigator.userAgent
  if (userAgent.indexOf('Firefox') !== -1 || userAgent.indexOf('Chrome') !== -1) {
    window.location.replace('about:blank')
  } else {
    window.opener = null
    window.open('', '_self')
  }
  window.close()
}
(async () => {

    const menu = document.querySelector(".nav-item.menu > .avatar-wrapper")
menu.click()
await wait()

const menuItems = document.querySelectorAll('.dropdown-item')
menuItems[1].querySelector(".open-menu-page").click()
await wait()

document.querySelector(".signin .btn").click()
await wait()

document.querySelectorAll(".success-modal .byte-modal__body .btn")[0].click()
await wait()

document.querySelector(".text-free").click()
await wait()

document.getElementsByClassName("stick-btn")[2].dispatchEvent(new Event('click'))

await wait()

document.querySelectorAll(".byte-menu--vertical .item a")[4].click()
await wait()

document.querySelectorAll(".item-container .item").forEach( item => {

    item.click()
})
await wait()

document.querySelectorAll(".item-container .item").forEach( item => {

    item.click()
})
})()
