<template functional>
    <footer class="footer section__footer">
        <div class="footer__content">
            <div class="footer__left">
                <span>Copyright &copy; 2022 Omer Mazor</span>
            </div>
            <div class="footer__right">
                <a
                    href="https://github.com/omermazorgroup/real-time-chat.git"
                    target="_blank"
                    class="nav__link"
                >
                    <ion-icon name="logo-github" class="footer__icon"></ion-icon>
                </a>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'Footer'
};
</script>

<style lang="scss">
@import '@/assets/scss/components/footer.scss';
</style>
