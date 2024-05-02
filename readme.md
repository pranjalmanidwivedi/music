let list = document.querySelector(".right");

let arr = [
    {
        songname : "Main Nikla Gaddi Leke",
        imgsrc : "./Song-cover/id3Picture_793840555.jpg",
        songsrc : "./Songs/p.mp3"
    },
    {
        songname : "Aane se uske aaye bahar",
        imgsrc : "./Song-cover/11981_4.jpg",
        songsrc : "./Songs/Aane-Se-Uske-Aaye-Bahar(PaglaSongs).mp3"
    },
    {
        songname : "Tum Agar Saath Dene",
        imgsrc : "./Song-cover/id3Picture_891426438.jpg",
        songsrc : "./Songs/Tum Agar Saath Dene Ka Vada Karo 128 Kbps.mp3"
    },
    {
        songname : "Yeh Wada Rha",
        imgsrc : "./Song-cover/id3Picture_1394269229.jpg",
        songsrc : "./Songs/Yeh Vaada Raha - Yeh Vaada Raha 128 Kbps.mp3"
    },
    {
        songname : "O Saathi Re",
        imgsrc : "./Song-cover/10571_4.jpg",
        songsrc : "./Songs/O-Saathi-Re(PaglaSongs).mp3"
    },
    {
        songname : "Sau Saal Pehle",
        imgsrc : "./Song-cover/id3Picture_1502125638.jpg",
        songsrc : "./Songs/Sau Saal Pahle 128 Kbps.mp3"
    },
    {
        songname : "Zindagi Ek Safar Hai",
        imgsrc : "./Song-cover/5647_4.jpg",
        songsrc : "./Songs/Zindagi-Ek-Safar-Hai-Suhana(PaglaSongs).mp3"
    },
    {
        songname : "Neele Neele Ambar Par",
        imgsrc : "./Song-cover/10569_4.jpg",
        songsrc : "./Songs/Neele-Neele-Ambar-Par-Kishore-Kumar(PaglaSongs).mp3"
    },
    {
        songname : "Chaand Si Mehbooba",
        imgsrc : "./Song-cover/11067_4.jpg",
        songsrc : "./Songs/Chand-Si-Mehbooba-Ho-Meri(PaglaSongs).mp3"
    },
    {
        songname : "Jane-Jigar Jaaneman",
        imgsrc : "./Song-cover/11418_4.jpg",
        songsrc : "./Songs/Jaane-Jigar-Jaaneman(PaglaSongs).mp3"
    },
    {
        songname : "Mere Saamne Wali ",
        imgsrc : "./Song-cover/11764_4.jpg",
        songsrc : "./Songs/Mere-Samne-Wali(PaglaSongs).mp3"
    },
    {
        songname : "Pyaar Hua Ikraar Hua",
        imgsrc : "./Song-cover/11767_4.jpg",
        songsrc : "./Songs/Pyar-Hua-Ikrar-Hua-Hai(PaglaSongs).mp3"
    },
    {
        songname : "Likhe Jo Khat Tujhe",
        imgsrc : "./Song-cover/11908_4.jpg",
        songsrc : "./Songs/Likhe-Jo-Khat-Tujhe-O-Teri-Yad-Main(PaglaSongs).mp3"
    },
    {
        songname : "Kitna Pyaara Waada Hai",
        imgsrc : "./Song-cover/11909_4.jpg",
        songsrc : "./Songs/Kitna-Pyara-Wada-Hai(PaglaSongs).mp3"
    },
    {
        songname : "Bahut Pyaar Karte Hai",
        imgsrc : "./Song-cover/14074_4.jpg",
        songsrc : "./Songs/Bahut-Pyar-Karte-Hai-Tumko-Sanam(PaglaSongs).mp3"
    },
    {
        songname : "Ek Ajnabee Haseena Se",
        imgsrc : "./Song-cover/id3Picture_880695672.jpg",
        songsrc : "./Songs/Ek Ajnabee Haseena Se.mp3"
    },
    {
        songname : "Tumhari Nazron Mein Humne",
        imgsrc : "./Song-cover/id3Picture_640339433.jpg",
        songsrc : "./Songs/Tumhari Nazron Mein Humne Dekha - Kal Ki Awaz 128 Kbps.mp3"
    },
    {
        songname : "Hontho Se Chhu Lo",
        imgsrc : "./Song-cover/id3Picture_1146524176.jpg",
        songsrc : "./Songs/Hothon Se Chhu Lo Tum (From Prem Geet) - Prem Geet 128 Kbps.mp3"
    },
    {
        songname : "Hai Apna Dil To",
        imgsrc : "./Song-cover/id3Picture_1372020204.jpg",
        songsrc : "./Songs/Hai Apna Dil To Aawara - Solva Saal 128 Kbps.mp3"
    }

]

let clutter = "";

arr.forEach(function(elem,idx) {
    clutter+= `<div class="songs" id="${idx}">
                    <img src="${elem.imgsrc}" id="${idx}">
                    <p class="songname">${elem.songname}</p>
                </div>`;
})

list.innerHTML = clutter;

let songs = document.querySelectorAll(".songs");

let defaultsongname = document.querySelector(".song-name")

defaultsongname.innerHTML = arr[0].songname;

let music = new Audio()

let img = document.querySelector(".left-player img");
img.src = arr[0].imgsrc;

songs.forEach(function(songs) {
    songs.addEventListener("click", function(dets){
        music.src = arr[dets.target.id].songsrc;
        if(dets.target.id == 0){
            music.play();
            document.querySelector(".song-name").innerHTML = arr[dets.target.id].songname;
            img.src = arr[dets.target.id].imgsrc;
            
        }
        else if(dets.target.id == 1){
            music.play();
            document.querySelector(".song-name").innerHTML = arr[dets.target.id].songname;
            img.src = arr[dets.target.id].imgsrc;
            
        }
        else if(dets.target.id == 2){
            music.play();
            document.querySelector(".song-name").innerHTML = arr[dets.target.id].songname;
            img.src = arr[dets.target.id].imgsrc;
            
        }
        else if(dets.target.id == 3){
            music.play();
            document.querySelector(".song-name").innerHTML = arr[dets.target.id].songname;
            img.src = arr[dets.target.id].imgsrc;
            
        }
        else if(dets.target.id == 4){
            music.play();
            document.querySelector(".song-name").innerHTML = arr[dets.target.id].songname;
            img.src = arr[dets.target.id].imgsrc;
            
        }
        else if(dets.target.id == 5){
            music.play();
            document.querySelector(".song-name").innerHTML = arr[dets.target.id].songname;
            img.src = arr[dets.target.id].imgsrc;
            
        }
        else if(dets.target.id == 6){
            music.play();
            document.querySelector(".song-name").innerHTML = arr[dets.target.id].songname;
            img.src = arr[dets.target.id].imgsrc;
            
        }
        else if(dets.target.id == 7){
            music.play();
            document.querySelector(".song-name").innerHTML = arr[dets.target.id].songname;
            img.src = arr[dets.target.id].imgsrc;
            
        }
        else if(dets.target.id == 8){
            music.play();
            document.querySelector(".song-name").innerHTML = arr[dets.target.id].songname;
            img.src = arr[dets.target.id].imgsrc;
            
        }
        else if(dets.target.id == 9){
            music.play();
            document.querySelector(".song-name").innerHTML = arr[dets.target.id].songname;
            img.src = arr[dets.target.id].imgsrc;
            
        }
        else if(dets.target.id == 10){
            music.play();
            document.querySelector(".song-name").innerHTML = arr[dets.target.id].songname;
            img.src = arr[dets.target.id].imgsrc;
            
        }
        else if(dets.target.id == 11){
            music.play();
            document.querySelector(".song-name").innerHTML = arr[dets.target.id].songname;
            img.src = arr[dets.target.id].imgsrc;
            
        }
        else if(dets.target.id == 12){
            music.play();
            document.querySelector(".song-name").innerHTML = arr[dets.target.id].songname;
            img.src = arr[dets.target.id].imgsrc;
            
        }
        else if(dets.target.id == 13){
            music.play();
            document.querySelector(".song-name").innerHTML = arr[dets.target.id].songname;
            img.src = arr[dets.target.id].imgsrc;
            
        }
        else if(dets.target.id == 14){
            music.play();
            document.querySelector(".song-name").innerHTML = arr[dets.target.id].songname;
            img.src = arr[dets.target.id].imgsrc;
            
        }
        else if(dets.target.id == 15){
            music.play();
            document.querySelector(".song-name").innerHTML = arr[dets.target.id].songname;
            img.src = arr[dets.target.id].imgsrc;
            
        }
        else if(dets.target.id == 16){
            music.play();
            document.querySelector(".song-name").innerHTML = arr[dets.target.id].songname;
            img.src = arr[dets.target.id].imgsrc;
            
        }
        else if(dets.target.id == 17){
            music.play();
            document.querySelector(".song-name").innerHTML = arr[dets.target.id].songname;
            img.src = arr[dets.target.id].imgsrc;
            
        }
        else if(dets.target.id == 18){
            music.play();
            document.querySelector(".song-name").innerHTML = arr[dets.target.id].songname;
            img.src = arr[dets.target.id].imgsrc;
            
        }
    })
})

let play = document.querySelector("#play");
let previous = document.querySelector("#previous");
let next = document.querySelector("#next");
let shuffle = document.querySelector("#shuffle");
let repeat = document.querySelector("#repeat");
let btn = document.querySelector(".play");
