<template>
<link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet" />
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
<div class="headerbg" style="text-align: center;">
                CONTACT
            </div>
    <div id="contact" class="row contact-details">
                <div title="phone ">
                    <a href="tel: +1 203 450 5159 "><span
                                class="material-icons inline-icon md-36 ">phone</span></a>
                </div>
                <div title="e-mail">
                    <a href="mailto: manish.singarapu@gmail.com " target="_blank"><span
                                class="material-icons inline-icon md-36 ">mail</span></a>
                </div>
                <div title="twitter">
                    <a href="https://twitter.com/" class="fa fa-twitter" target="_blank"></a>
                </div>
                <div title="facebook">
                    <a href="https://www.facebook.com/ " class="fa fa-facebook" target="_blank"></a>
                </div>
                <div title="linked in">
                    <a href="https://www.linkedin.com/in/smanishc/" class="fa fa-linkedin" target="_blank"></a>
                </div>
            </div>
</template>

<script>
export default {
    name:'MyFooter',
    props:{

    }
}
</script>

<style scoped>
        .headerbg {
            background-color: black;
            padding: 10px;
            color: white;
            font-size: 17px;
            font-weight: 500;
        }
        .fa {
            padding: 10px;
            width: 20px;
            text-align: center;
            text-decoration: none;
        }
        
        .fa:hover {
            opacity: 0.7;
        }
        
        .fa-facebook {
            background: #3B5998;
            color: white;
        }
        
        .fa-twitter {
            background: #55ACEE;
            color: white;
        }
        
        .fa-linkedin {
            background: #044a80;
            color: white;
        }
        
        .padd {
            padding: 10px;
        }
        
        .row {
            display: flex;
            flex-direction: row;
            width: 100%;
        }
        
        .vertical-line {
            height: 80px;
            position: relative;
            top: 5px;
            padding-left: 5px;
            border-right: 2px solid gray;
        }
        
        .contact-details {
            background-color: #5885AF;
            justify-content: space-around;
            height: 50px;
            padding-top: 2%;
        }
        
</style>