<template>
    <screen>
        <Header/>
        <div class="sign-in">
            <div class="sign-in-inner">
                <h3>
                    Log in
                </h3>
                <form>
                    <div class="sign-in-input-wrap">
                        <input type="email" placeholder="E-mail">
                    </div>
                    <div class="sign-in-input-wrap">
                        <input type="password" placeholder="Password">
                    </div>
                    <div class="sign-in-input-wrap">
                        <a href="/" class="forgot">Forgot password?</a>
                    </div>
                    <div class="sign-in-submit-wrap">
                        <input type="submit">
                    </div>
                    <span class="separetor">
                        or
                    </span>
                    <div class="sign-in-input-wrap">
                        <a href="/" class="btn-like"> Continue with Apple</a>
                    </div>
                    <div class="sign-in-input-wrap">
                        <a href="/" class="inv">Continue with Google</a>
                    </div>
                    <div class="sign-in-input-wrap">
                        <a href="/" class="inv">Continue with Facebook</a>
                    </div>
                </form>
            </div>
        </div>
    </screen>
</template>

<script>
import Header from "./Header.vue";


export default {

    components: {
        Header
    }

}
</script>

<style>

h3 {
    text-align: center;
    font-weight: normal;
    padding: 2em;
    color: #fff;
}

div.sign-in {
    height: calc(100vh - 72px);
    display: flex;
    align-items: center;
    justify-content: center;
}

div.sign-in form {
    margin: 0;
}

.sign-in-input-wrap {
    margin-bottom: .75em;
    
}

.sign-in-input-wrap input {
    width: 220px;
}

.sign-in-input-wrap a.forgot {
    text-decoration: none;
    display: block;
    color: #fff;
    font-size: 0.75em;
    text-align: right;
    padding: .5em;
}

.sign-in-input-wrap input::placeholder {
  color: #fff;
}

.sign-in-submit-wrap input {
    padding: .5em 2.5em;
    margin: 0 .5em;
    width: calc(100% - 1em);
    color: #333333;
    border-radius: 3px;
    border: none;
    outline: none;
    background: #fff;
    font-size: .9em;
}

a.btn-like {
    text-align: center;
    text-decoration: none;
    display: block;
    padding: .5em 0;
    margin: 0 .5em;
    width: calc(100% - 1em);
    color: #333333;
    background: #fff;
    border-radius: 3px;
    border: none;
    outline: none;
    font-size: .9em;
}

span.separetor {
    display: block;
    text-align: center;
    color: #fff;
    padding: .5em;
}

.inv {
    text-align: center;
    text-decoration: none;
    display: block;
    padding: .5em 0;
    margin: 0 .5em;
    width: calc(100% - 1em);
    border-radius: 3px;
    outline: none;
    font-size: .9em;
    background: #333333;
    color: #fff;
    border: 1px solid #fff;
}




</style>