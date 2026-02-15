// ==UserScript==
// @name        Block This
// @namespace        http://tampermonkey.net/
// @version        0.3
// @description        PCブログページからブロックボタンを表示
// @author        Ameba Blog User
// @match        https://ameblo.jp/*
// @match        https://www.ameba.jp/profile/general/*
// @exclude        https://ameblo.jp/*/image*
// @noframes
// @icon        https://www.google.com/s2/favicons?sz=64&domain=ameba.jp
// @grant        none
// @updateURL        https://github.com/personwritep/Block_This/raw/main/Block_This.user.js
// @downloadURL        https://github.com/personwritep/Block_This/raw/main/Block_This.user.js
// ==/UserScript==


if(location.hostname=='ameblo.jp'){ // ブログページ

    let target=document.querySelector('head');
    let monitor=new MutationObserver(catch_key);
    monitor.observe(target, { childList: true });

    catch_key();

    function catch_key(){
        document.addEventListener("keydown", check_key);
        function check_key(event){
            let gate=-1;
            if(event.altKey==true){
                if(event.keyCode==116){
                    event.preventDefault(); gate=1; }} // ショートカット「Alt＋F5」

            if(gate==1){
                event.stopImmediatePropagation();
                event.preventDefault();
                do_block(); }} // ブロックを実行
    } // catch_key


    function do_block(){
        let url=location.href.toString();
        let url_parts=url.split('/');
        let profile_page='https://www.ameba.jp/profile/general/'+ url_parts[3] +'/?blockthis';
        window.location.href =profile_page; }

} // ブログページ



if(location.pathname.includes('profile/general')){ // プロフィール画面
    let query=window.location.search.slice(1);
    if(query=='blockthis'){
        let url=location.href.toString().replace('?blockthis', '');
        history.replaceState('','', url); // クエリ文字列を削除

        setTimeout(()=>{
            let report_trigger=document.querySelector('.report__trigger');
            if(report_trigger){
                let dropdown_style=
                    '<style .class="dpd_style">.spui-DropdownMenu-menu--leftTop { '+
                    'position: fixed; top: 80px; left: calc(50% - 190px); '+
                    'width: 380px; font-size: 24px; outline: 3px solid red; }</style>';
                if(!document.querySelector('.dpd_style')){
                    document.body.insertAdjacentHTML('beforeend', dropdown_style); }

                report_trigger.click(); }}, 500);
    }

} // プロフィール画面
