<template>
    <el-row class="footer-section">
        <el-col :span="12" class="policy-and-terms-section">
            © 2024 Riny Yadav. All rights reserved.
        </el-col>
        <el-col :span="12" class="social-section">
            <a href="https://www.behance.net/rinyyadav" target="_blank"><img src="../../assets/icons/dribble-icon.png" alt="Dribble Icon" class="dribble-icon social-icon" /></a>
            <a href="https://www.behance.net/rinyyadav" target="_blank"><img src="../../assets/icons/linkedin-icon.png" alt="LinkedIn Icon" class="social-icon" /></a>
            <a href="https://www.behance.net/rinyyadav" target="_blank"><img src="../../assets/icons/behance-icon.png" alt="Behance Icon" class="social-icon" /></a>
        </el-col>
    </el-row>
</template>
<script>
    export default {
        name: "FooterSection",
    };
</script>
<style scoped>
.footer-section {
    width: 100%;
    min-height: 80px;
    height: auto;
    max-height: 200px;
    background: transparent;
    backdrop-filter: blur(2px);
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    align-self: center;
    border-top: 1px solid #261F221A;
}
.policy-and-terms-section {
    cursor: pointer;
    color: var(--black75, rgba(38, 31, 34, 0.75));
    font-family: "Brandon";
    font-size: 16px;
    font-style: normal;
    font-weight: 500;
    line-height: 80px;
}
.social-section {
    a {
        margin: 0 10px;
    }
    img {
        width: auto;
        height: 20px;
    }
    .dribble-icon {
        height: 25px !important;
        margin-bottom: -4px;
    }
}
@media (max-width: 768px) {
    .footer-section {
        max-height: 250px;
        display: flex;
        flex-direction: column-reverse;
        justify-content: center;
        align-items: center;
        align-self: center;
    }
    .policy-and-terms-section {
        line-height: 20px;
        margin-bottom: 20px;
    }
    .social-section {
        margin-top: 20px;
        margin-bottom: 20px;
        a {
            margin: 0 10px;
        }
        img {
            width: auto;
            height: 20px;
        }
        .dribble-icon {
            height: 25px !important;
            margin-bottom: -4px;
        }
    }
}
</style>