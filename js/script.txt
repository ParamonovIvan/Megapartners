const langButton = document.querySelector('.lang')
const langButtonMobile = document.querySelector('.lang_mobile')

const langButtonTexts = document.querySelectorAll('.header__lang-text')

const burgerButton = document.querySelector('.burger-button')
const mobileMenu = document.querySelector('.header__menu__wrapper')

langButton.addEventListener('click', () => {
  changeLang()
})

langButtonMobile.addEventListener('click', () => {
  changeLang()
})

const changeLang = () => {
  langButtonTexts.forEach((langButtonText) => {
    langButtonText.classList.toggle('header__lang-text_hidden')
  })
}

burgerButton.addEventListener('click', () => {
  mobileMenu.classList.toggle('header__menu__wrapper_visible')
  burgerButton.classList.toggle('burger-button_close')
})
