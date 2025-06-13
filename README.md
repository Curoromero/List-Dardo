# List-Dardo
import React, { useState } from "react";

const animeList = [
  {
    title: "YU-GI-OH!",
    subs: [
      "Yu-Gi-Oh! (1-27)",
      "Yu-Gi-Oh!",
      "Yu-Gi-Oh! Duel Monsters (1-49)",
      "Yu-Gi-Oh! Duel Monsters: Special",
      "Yu-Gi-Oh! Duel Monsters (50-144)",
      "Yu-Gi-Oh! Duel Monsters: Hikari no Pyramid",
      "Yu-Gi-Oh! Duel Monsters (145-198)",
      "Yu-Gi-Oh! Alex (1-12)",
      "Yu-Gi-Oh! Duel Monsters (199-224)",
      "Yu-Gi-Oh! Duel Monsters GX (1-180)",
      "Yu-Gi-Oh! 5D’s (1-26)",
      "Yu-Gi-Oh! 5D’s: Shinkasuru Kettō! Stardust vs. Red Demon's",
      "Yu-Gi-Oh! 5D’s (27-80)",
      "Gekijōban Yu-Gi-Oh!: Chō Yūgō! Toki wo Koeta Kizuna",
      "Yu-Gi-Oh! 5D’s (81-154)",
      "Yu-Gi-Oh! Zexal (1-73)",
      "Yu-Gi-Oh! Zexal Special",
      "Yu-Gi-Oh! Zexal II (1-8)",
      "Yu-Gi-Oh! Zexal II: Midokoro Tenkomori Special",
      "Yu-Gi-Oh! Zexal II (9-58)",
      "Yu-Gi-Oh! Zexal II: Iza! Saishuu Kessen e!! Special",
      "Yu-Gi-Oh! Zexal II (59-73)",
      "Yu-Gi-Oh! Arc-V (1-148)",
      "Yu-Gi-Oh! Vrains (1-120)",
      "Yu-Gi-Oh! Sevens (1-92)",
      "Yu-Gi-Oh! Go Rush!! (1-151)"
    ]
  },
  {
    title: "NARUTO",
    subs: [
      "Naruto 1-19",
      "Naruto: Akaki Yotsuba no Clover wo Sagase",
      "Naruto: The Cross Roads",
      "Naruto 20-100",
      "Naruto: Takigakure no Shitou - Ore ga Eiyuu Dattebayo!",
      "Naruto: Dai Katsugeki!! Yuki Hime Ninpouchou Dattebayo! - Konoha no Sato no Dai Undoukai",
      "Naruto Narutimate Hero 3: Tsuini Gekitotsu! Jounin vs. Genin!! Musabetsu Dairansen Taikai Kaisai!!",
      "Naruto Soyokazeden Movie: Naruto to Mashin to Mitsu no Onegai Dattebayo!!",
      "Naruto 101",
      "Naruto Movie 1: Dai Katsugeki!! Yuki Hime Ninpouchou Dattebayo!",
      "Naruto 102-160",
      "Naruto Movie 2: Dai Gekitotsu! Maboroshi no Chiteiiseki Dattebayo!",
      "Naruto 161-196",
      "Naruto Movie 3: Dai Koufun! Mikazuki Jima no Animal Panic Dattebayo!",
      "Naruto 197-220",
      "Naruto: Shippuden 1-10",
      "Hurricane! “Konoha Academy” Chronicles",
      "Naruto: Shippuden 11-32",
      "Naruto: Shippuuden Movie 1",
      "Naruto: Shippuden 33-53",
      "Naruto: Shippuuden Movie 2 - Kizuna",
      "Naruto: Shippuden 54-88",
      "Naruto: Shippuuden Movie 3 - Hi no Ishi wo Tsugu Mono",
      "Naruto: Shippuden 89-135",
      "Naruto: Shippuuden Movie 4 - The Lost Tower",
      "Naruto: Shippuden 136-176",
      "Naruto: Shippuuden Movie 5 - Blood Prison",
      "Naruto: Shippuden 177-216",
      "Naruto x UT",
      "Naruto: Shippuden 217-219",
      "Naruto: Honoo no Chuunin Shiken! Naruto vs. Konohamaru!!",
      "Naruto: Shippuuden - Sunny Side Battle",
      "Naruto: Shippuden 220-311",
      "Naruto: Shippuuden Movie 6 - Road to Ninja",
      "Naruto: Shippuden 312-369",
      "Hashirama Senju vs. Madara Uchiha",
      "Ninja Escapades",
      "Naruto: Shippuden 370-493",
      "The Last: Naruto the Movie",
      "Naruto: Shippuden 494-500",
      "Boruto: Naruto the Movie - Naruto ga Hokage ni Natta Hi",
      "Naruto SD: Rock Lee no Seishun Full-Power Ninden 1-51",
      "Boruto: Naruto the Movie",
      "Boruto: Naruto Next Generations 1-51",
      "Boruto: Jump Festa 2016 Special",
      "Boruto: Naruto Next Generations 52-293"
    ]
  },
  {
    title: "FAIRY TAIL",
    subs: [
      "Fairy Tail (2009) 1-68",
      "Fairy Tail OVA 1 Welcome to Fairy Hills!!",
      "Fairy Tail OVA 2 Fairy Academy",
      "Fairy Tail OVA 3 Memory Days",
      "Fairy Tail (2009) 69-124",
      "Fairy Tail Movie 1: Houou no Miko",
      "Fairy Tail Movie 1: Houou no Miko - Hajimari no Asa",
      "Fairy Tail (2009) 125-150",
      "Fairy Tail OVA 6 Fairy Tail X Rave",
      "Fairy Tail (2009) 151-154",
      "Fairy Tail OVA 4 Fairies’ Training Camp",
      "Fairy Tail (2009) 155-170",
      "Fairy Tail OVA 5 The Exciting Ryuzetsu Land",
      "Fairy Tail (2009) 171-175",
      "Fairy Tail (2014) 1-27 (176-203)",
      "Fairy Tail OVA 7 Fairies’ Penalty Game",
      "Fairy Tail (2014) 28-57 (204-233)",
      "Fairy Tail OVA 8 Natsu vs. Mavis",
      "Fairy Tail (2014) 58-102 (234-277)",
      "Fairy Tail OVA 9 Fairies’ Christmas",
      "Fairy Tail: Dragon Cry (Second Movie)",
      "Fairy Tail Final Series 1-51 (278-328)",
      "Fairy Tail: 100 Years Quest 1-13",
      "Fairy Tail: 100-nen Quest - Kanwa - Lucy's Diary",
      "Fairy Tail: 100 Years Quest 1-25"
    ]
  },
  {
    title: "BLEACH",
    subs: [
      "Bleach 1-8",
      "Bleach: Memories in the Rain",
      "Bleach: Gotei 13 Omake",
      "Bleach 9-63",
      "Bleach: Shuku! Rukia Dakkan! Kagayaku! Shinigami Juuban Shoubu! Mitai Shinigami Doon to Misemasu Special",
      "Bleach: The Sealed Sword Frenzy",
      "Bleach 64-109",
      "Bleach Movie 1: Memories of Nobody",
      "Bleach 110-137",
      "Bleach KaraBuri!: Gotei Juusan Yatai Daisakusen!",
      "Bleach Movie 2: The DiamondDust Rebellion - Mou Hitotsu no Hyourinmaru",
      "Bleach Movie 3: Fade to Black - Kimi no Na wo Yobu",
      "Bleach 138-299",
      "Bleach Movie 4: Jigoku-hen",
      "Bleach 300-366",
      "Bleach: Sennen Kessen-hen 1-13",
      "Bleach: Sennen Kessen-hen - Ketsubetsu-tan 1-8",
      "Bleach: Sennen Kessen-hen - Ketsubetsu-tan Recap",
      "Bleach: Sennen Kessen-hen - Ketsubetsu-tan 9-13",
      "Bleach: Sennen Kessen-hen - Soukoku-tan 1-14",
      "Bleach: Sennen Kessen-hen - Kashin-tan"
    ]
  },
  {
    title: "BOKU NO HERO",
    subs: [
      "Boku no Hero Academia 1-13",
      "Boku no Hero Academia: Sukue! Kyuujo Kunren!",
      "Boku no Hero Academia: Hero Note",
      "Boku no Hero Academia 2nd Season 1-20",
      "Boku no Hero Academia: Training of the Dead",
      "Boku no Hero Academia 2nd Season 21-25",
      "Boku no Hero Academia 3rd Season 1-14",
      "Boku no Hero Academia: Ikinokore! Kesshi no Survival Kunren",
      "Boku no Hero Academia 3rd Season 15-20",
      "Boku no Hero Academia the Movie 1: Futari no Hero",
      "Boku no Hero Academia the Movie 1: Futari no Hero Specials",
      "Boku no Hero Academia 3rd Season 21-25",
      "Boku no Hero Academia 4th Season 1-25",
      "Boku no Hero Academia 5th Season 1-18",
      "Boku no Hero Academia (ONA)",
      "Boku no Hero Academia: UA Heroes Battle",
      "Boku no Hero Academia 5th Season 19-24",
      "Boku no Hero Academia the Movie 2: Heroes:Rising",
      "Boku no Hero Academia the Movie 2: Heroes:Rising - Epilogue Plus - Yume wo Genjitsu ni",
      "Boku no Hero Academia 5th Season 25",
      "Boku no Hero Academia the Movie 3: World Heroes' Mission",
      "Boku no Hero Academia the Movie 3: World Heroes' Mission - Tabidachi",
      "Boku no Hero Academia 6th Season 1-25",
      "Boku no Hero Academia the Movie 4: You're Next",
      "Boku no Hero Academia the Movie 4: You're Next - A Piece of Cake",
      "Boku no Hero Academia: Memories",
      "Boku no Hero Academia 7th Season",
      "Vigilante: Boku no Hero Academia Illegals 1-13",
      "Boku no Hero Academia: Final Season"
    ]
  },
  {
    title: "INAZUMA ELEVEN",
    subs: [
      "Inazuma Eleven 1-127",
      "Inazuma Eleven: Saikyou Gundan Ogre Shuurai",
      "Inazuma Eleven Go 1-32",
      "Inazuma Eleven Go Specials 1-2",
      "Inazuma Eleven Go: Kyuukyoku no Kizuna Gryphon",
      "Inazuma Eleven Go 33-47",
      "Inazuma Eleven Go: Chrono Stone 1-25",
      "Inazuma Eleven Go vs. Danball Senki W Movie",
      "Inazuma Eleven Go: Chrono Stone 26-51",
      "Inazuma Eleven Go: Galaxy 1-43",
      "Inazuma Eleven: Chou Jigen Dream Match",
      "Inazuma Eleven: Soushuuhen Densetsu no Kickoff",
      "Inazuma Eleven: Reloaded - Soccer no Henkaku",
      "Inazuma Eleven: Outer Code 1-6",
      "Inazuma Eleven: Ares no Tenbin 1-26",
      "Inazuma Eleven: Orion no Kokuin 1-49",
      "Inazuma Eleven: Aratanaru Eiyuu-tachi no Joshou"
    ]
  },
  {
    title: "NANATSU NO TAIZAI",
    subs: [
      "Nanatsu no Taizai 1-24",
      "Nanatsu no Taizai OVA",
      "Nanatsu no Taizai: Seisen no Shirushi 1-4",
      "Nanatsu no Taizai: Imashime no Fukkatsu Joshou",
      "Nanatsu no Taizai: Imashime no Fukkatsu 1-24",
      "Nanatsu no Taizai Movie 1: Tenkuu no Torawarebito",
      "Nanatsu no Taizai: Eiyuu-tachi wa Hashagu",
      "Nanatsu no Taizai: Kamigami no Gekirin 1-24",
      "Hawk no Onayami Soudanshitsu 1-39",
      "Hawk no Onayami Soudanshitsu Special",
      "Nanatsu no Taizai: Funnu no Shinpan 1-24",
      "Gekidan Nanatsu no Taizai 1-13",
      "Nanatsu no Taizai Movie 2: Hikari ni Norowareshi Mono-tachi",
      "Nanatsu no Taizai: Ensa no Edinburgh",
      "Nanatsu no Taizai: Ensa no Edinburgh Part 2",
      "Nanatsu no Taizai: Mokushiroku no Yonkishi 1-24",
      "Nanatsu no Taizai: Mokushiroku no Yonkishi 2nd Season 1-12"
    ]
  },
  {
    title: "Air",
    subs: [
      "Air (1-9)",
      "Air in Summer (1-2)",
      "Air (10-12)",
      "Air Memories"
    ]
  },
  {
    title: "Alien 9",
    subs: [
      "Alien 9 (1-4)"
    ]
  },
  {
    title: "Aoi Sekai no Chūshin de",
    subs: [
      "Aoi Sekai no Chūshin de (1-3)"
    ]
  },
  {
    title: "Arifureta Shokugyou de Sekaisaikyou",
    subs: [
      "Arifureta Shokugyou de Sekaisaikyou: Prologue",
      "Arifureta Shokugyou de Sekaisaikyou (1-5)",
      "Arifureta Shokugyou de Sekaisaikyou: Picture Drama (1-5)",
      "Arifureta Shokugyou de Sekaisaikyou: Sōshūhen Orcus dai Meikyū",
      "Arifureta Shokugyou de Sekaisaikyou (6-13)",
      "Arifureta Shokugyou de Sekaisaikyou: Picture Drama (6-13)",
      "Arifureta Shokugyou de Sekaisaikyou Specials (1-2)",
      "Arifureta Shokugyou de Sekaisaikyou 2nd Season (1-6)",
      "Arifureta Shokugyou de Sekaisaikyou 2nd Season Picture Drama (1-6)",
      "Arifureta Shokugyou de Sekaisaikyou: Maboroshi no Bouken to Kiseki no Kaigō",
      "Arifureta Shokugyou de Sekaisaikyou 2nd Season (7-12)",
      "Arifureta Shokugyou de Sekaisaikyou 2nd Season: Picture Drama (6-12)",
      "Arifureta Shokugyou de Sekaisaikyou: Arifureta Yorimichi de Sekai Saikyō",
      "Arifureta Shokugyou de Sekaisaikyou Season 3 (1-16)",
      "Arifureta Shokugyou de Sekaisaikyou Season 3: Picture Drama (1-16)"
    ]
  },
  {
    title: "Asobi ni Iku yo!",
    subs: [
      "Asobi ni Iku yo! (1-12)",
      "Asobi ni Iku yo!: Asobi ni Oide",
      "Asobi ni Iku yo!: Asobi ni Oide - Owari"
    ]
  },
  {
    title: "Bokuha Tomodachiga Sukunai",
    subs: [
      "Bokuha Tomodachiga Sukunai: Yaminabe wa Bishoujo ga Zannen na Nioi",
      "Bokuha Tomodachiga Sukunai (1-12)",
      "Bokuha Tomodachiga Sukunai: Relay Shousetsu wa Ketsumatsu ga Hanpanai",
      "Bokuha Tomodachiga Sukunai Next (1-12)"
    ]
  },
  {
    title: "Chainsaw Man",
    subs: [
      "Chainsaw Man (1-12)"
    ]
  },
  {
    title: "Date a Live",
    subs: [
      "Date a Live Director's Cut (1-12)",
      "Date a Live: Date to Date",
      "Date a Live II Director's Cut (1-10)",
      "Date a Live: Kurumi Star Festival",
      "Gekijōban Date a Live: Mayuri Judgment",
      "Date a Live III (1-12)",
      "Date a Bullet (1-2)",
      "Date a Live IV (1-12)",
      "Date a Live V (1-12)"
    ]
  },
  {
    title: "Digimon",
    subs: [
      "Digimon Adventure (1-34)",
      "Digimon Adventure",
      "Digimon Adventure (35-54)",
      "Digimon Adventure: Bokura no War Game!",
      "Digimon Adventure 02 (1-21)",
      "Digimon Adventure 02 Zenpen: Digimon Hurricane Jōriku!!",
      "Digimon Adventure 02 Kōhen: Chouzetsu Shinka!! Ōgon no Digimental",
      "Digimon Adventure 02 (22-50)",
      "Digimon Adventure 02: Diablomon no Gyakushū",
      "Digimon Adventure 3D: Digimon Grand Prix!",
      "Digimon Adventure Tri. (1-6)",
      "Digimon Adventure: 20-shuunen Memorial Story (1-5)",
      "Digimon Adventure: Last Evolution Kizuna",
      "Digimon Adventure 02: The Beginning",
      "Digimon Tamers (1-20)",
      "Digimon Tamers: Bōkensha-tachi no Tatakai",
      "Digimon Tamers (21-51)",
      "Digimon Tamers: Bōsō Digimon Tokkyū",
      "Digimon Frontier (1-12)",
      "Digimon Frontier: Ornismon Fukkatsu!!",
      "Digimon Frontier (13-50)",
      "Digital Monster X-evolution",
      "Digimon Savers (1-48)",
      "Digimon Savers: Agumon! Gaomon! Lalamon! Bakuretsu! Jōgai Last Battle!",
      "Digimon Savers the Movie: Kyūkyoku Power! Burst Mode Hatsudō!!",
      "Digimon Savers 3D: Digital World Kiki Ippatsu!",
      "Digimon Xros Wars (1-30)",
      "Digimon Xros Wars: Aku no Death General to Nanatsu no Ōkoku (1-24)",
      "Digimon Xros Wars: Aku no Death General to Nanatsu no Oukoku (1-24)",
      "Digimon Universe: Appli Monsters (1-52)",
      "Digimon Adventure: (1-67)",
      "Digimon Ghost Game (1-24)",
      "Digimon Ghost Game: Takenaka Naoto ga Kataru Kaiki no Sekai",
      "Digimon Ghost Game (25-67)"
    ]
  },
  {
    title: "Dungeon ni Deai o Motomeru no wa Machigatte Iru Darōka",
    subs: [
      "Dungeon ni Deai o Motomeru no wa Machigatte Iru Darōka Familia Myth (1-13)",
      "Dungeon ni Deai o Motomeru no wa Machigatte Iru Darōka Familia Myth: Dungeon ni Onsen o Motomeru no wa Machigatte Iru Darōka",
      "Dungeon ni Deai o Motomeru no wa Machigatte Iru Darōka Gaiden: Sword of Oratoria (1-12)",
      "Gekijōban Dungeon ni Deai o Motomeru no wa Machigatte Iru Darōka: Orion no Ya",
      "Dungeon ni Deai o Motomeru no wa Machigatte Iru Darōka Familia Myth II: Past & Future",
      "Dungeon ni Deai o Motomeru no wa Machigatte Iru Darōka Familia Myth II (1-12)",
      "Dungeon ni Deai o Motomeru no wa Machigatte Iru Darōka Familia Myth II: Mujintō ni Yakusō o Motomeru no wa Machigatte Iru Darōka",
      "Dungeon ni Deai o Motomeru no wa Machigatte Iru Darōka Familia Myth III (1-12)",
      "Dungeon ni Deai o Motomeru no wa Machigatte Iru Darōka Familia Myth III: Orario ni Onsen o Motomeru no wa Machigatte Iru Darōka ~ O Furo no Kamisama Fōebā ~",
      "Dungeon ni Deai o Motomeru no wa Machigatte Iru Darōka Familia Myth IV: Play Back",
      "Dungeon ni Deai o Motomeru no wa Machigatte Iru Darōka Familia Myth IV: Shin Shō - Meikyū-hen (1-11)",
      "Dungeon ni Deai o Motomeru no wa Machigatte Iru Darōka Familia Myth IV: Shin Shō - Yakusai-hen (1-11)",
      "Dungeon ni Deai o Motomeru no wa Machigatte Iru Darōka Familia Myth V: Hōjō no Megami-hen (1-15)"
    ]
  },
  {
    title: "Chobits",
    subs: [
      "Chobits (1-26)",
      "Chobits: Hibiya, Kotoko: Kataru",
      "Chobits: Chibits - Sumomo, Kotoko: Todokeru"
    ]
  },
  {
    title: "Fruits Basket",
    subs: [
      "Fruits Basket (1-26)",
      "Fruits Basket 1st Season (1-25)",
      "Fruits Basket 2nd Season (1-25)",
      "Fruits Basket The Final (1-13)",
      "Fruits Basket Prelude"
    ]
  },
  {
    title: "Girls Bravo",
    subs: [
      "Girls Bravo (1-11)",
      "Girls Bravo Second Season (1-13)"
    ]
  },
  {
    title: "Golden Time",
    subs: [
      "Golden Time (1-24)"
    ]
  },
  {
    title: "Hayate no Gotoku!",
    subs: [
      "Hayate no Gotoku! (1-52)",
      "Hayate no Gotoku!!: Atsu ga Natsuize - Mizugi-hen!",
      "Hayate no Gotoku!! (1-25)",
      "Hayate no Gotoku! Heaven Is a Place on Earth",
      "Hayate no Gotoku! Can't Take My Eyes Off You (1-12)",
      "Hayate no Gotoku! Cuties (1-12)",
      "Hayate no Gotoku! OVA (1-3)"
    ]
  },
  {
    title: "Hi Score Girl",
    subs: [
      "Hi Score Girl (1-12)",
      "Hi Score Girl: Extra Stage (1-3)",
      "Hi Score Girl II (1-9)"
    ]
  },
  {
    title: "High School DxD",
    subs: [
      "High School DxD (1-12)",
      "High School DxD Specials (1-6)",
      "High School DxD OVA (1-2)",
      "High School DxD New Director's Cut (1-12)",
      "High School DxD New: Oppai, Tsutsumimasu!",
      "High School DxD BorN (1-12)",
      "High School DxD BorN: Ishibumi Ichiei Kanzen Kanshū! Mousou Bakuyō Kaijo Original Video (1-6)",
      "High School DxD BorN: Yomigaeranai Fushichō",
      "High School DxD Hero: Taīkukan-ura no Holy",
      "High School DxD Hero (1-12)"
    ]
  },
  {
    title: "Kage no Jitsuryokusha ni Naritakute!",
    subs: [
      "Kage no Jitsuryokusha ni Naritakute! (1-3)",
      "Kage no Jitsuryokusha ni Naritakute! (4-20)",
      "Kagejitsu! (1-17)",
      "Kage no Jitsuryokusha ni Naritakute! 2nd Season (1-12)",
      "Kagejitsu! Second (1-12)"
    ]
  },
  {
    title: "Kaifuku Jutsushi no Yarinaoshi",
    subs: [
      "Kaifuku Jutsushi no Yarinaoshi (1-12)"
    ]
  },
  {
    title: "Kanon",
    subs: [
      "Kanon (1-13)",
      "Kanon Kazahana",
      "Kanon (1-24)"
    ]
  },
  {
    title: "Katekyō Hitman Reborn!",
    subs: [
      "Katekyō Hitman Reborn! (1-203)",
      "Katekyō Hitman Reborn! Vongola Family Sōtōjō! Vongola Shiki Shūgakuryokō, Kuru!!",
      "Katekyō Hitman Reborn!: Mr. Rebokku no Ciao Ciao Interview (1-3)"
    ]
  },
  {
    title: "Kodomo no Jikan",
    subs: [
      "Kodomo no Jikan (1-4)",
      "Kodomo no Jikan: Anata ga Watashi ni Kureta Mono",
      "Kodomo no Jikan (5-12)",
      "Kodomo no Jikan: Rin no Gakkyuu Nisshi",
      "Kodomo no Jikan Ni Gakki (1)",
      "Kodomo no Jikan: Kuro-chan to Shiro-chan",
      "Kodomo no Jikan Ni Gakki (2-3)",
      "Kodomo no Jikan: Kodomo no Natsu Jikan"
    ]
  },
  {
    title: "Kono Subarashii Sekai ni Syukufuku wo!",
    subs: [
      "Kono Subarashii Sekai ni Syukufuku wo! (1-10)",
      "Kono Subarashii Sekai ni Syukufuku wo!: Kono Subarashī Choker ni Shukufuku wo!",
      "Kono Subarashii Sekai ni Syukufuku wo! 2 (1-10)",
      "Kono Subarashii Sekai ni Syukufuku wo! 2: Kono Subarashī Geijutsu ni Shukufuku wo!",
      "Eiga Kono Subarashii Sekai ni Syukufuku wo!: Kurenai Densetsu",
      "Kono Subarashii Sekai ni Bakuen wo! (1-12)",
      "Kono Subarashii Sekai ni Syukufuku wo! 3 (1-11)"
    ]
  },
  {
    title: "Make Heroine ga Ōsugiru!",
    subs: [
      "Make Heroine ga Ōsugiru! (1-12)"
    ]
  },
  {
    title: "Monogatari Series",
    subs: [
      "Bakemonogatari (1-5)",
      "Bakemonogatari Recap",
      "Bakemonogatari (6-15)",
      "Kizumonogatari (1-3)",
      "Kizumonogatari: Koyomi Vamp",
      "Nisemonogatari (1-11)",
      "Nekomonogatari (Kuro) (1-4)",
      "Nekomonogatari (Kuro) Recap",
      "Monogatari Series Second Season (1-11)",
      "Hanamonogatari (1-5)",
      "Monogatari Series Second Season (12-26)",
      "Koyomi History",
      "Tsukimonogatari (1-4)",
      "Koyomimonogatari (1-12)",
      "Owarimonogatari (1-12)",
      "Owarimonogatari - Owari ni Mukau Monogatari",
      "Owarimonogatari (1-4)",
      "Owarimonogatari - Araragi Koyomi no Monogatari",
      "Owarimonogatari (5-7)",
      "Zoku Owarimonogatari (1-6)",
      "Monogatari Series: Monster & Off Season (1-6)",
      "Monogatari Series: Monster & Off Season - Zankoku Douwa: Utsukushi-hime",
      "Monogatari Series: Monster & Off Season (7-14)"
    ]
  },
  {
    title: "Naku Koro ni",
    subs: [
      "Higurashi no Naku Koro ni (1-26)",
      "Higurashi no Naku Koro ni: Nekogoroshi-hen",
      "Higurashi no Naku Koro ni Kaku: Outbreak",
      "Higurashi no Naku Koro ni Kai (1-24)",
      "Higurashi no Naku Koro ni Kai: Specials (1-24)",
      "Higurashi no Naku Koro ni Rei (1-5)",
      "Higurashi no Naku Koro ni Kira (1-4)",
      "Umineko no Naku Koro ni (1-26)",
      "Umineko no Naku Koro ni: Specials (1-26)",
      "Higurashi no Naku Koro ni Gō (1-24)",
      "Higurashi no Naku Koro ni Sotsu (1-15)"
    ]
  },
  {
    title: "Rosario to Vampire",
    subs: [
      "Rosario to Vampire (1-13)",
      "Rosario to Vampire Capu2 (1-13)"
    ]
  },
  {
    title: "Sekirei",
    subs: [
      "Sekirei (1-12)",
      "Sekirei: Hajimete no Otsukai",
      "Sekirei Pure Engagement: Shindan/Yoka",
      "Sekirei Pure Engagement (1-13)"
    ]
  },
  {
    title: "Shimoneta to Iu Gainen ga Sonzai Shinai Taikutsu na Sekai",
    subs: [
      "Shimoneta to Iu Gainen ga Sonzai Shinai Taikutsu na Sekai (1-12)"
    ]
  },
  {
    title: "Sora no Otoshimono",
    subs: [
      "Sora no Otoshimono (1-13)",
      "Sora no Otoshimono: Project Pink",
      "Sora no Otoshimono Forte (1-12)",
      "Gekijōban Sora no Otoshimono: Tokeijikake no Angeloid",
      "Sora no Otoshimono Final: Eternal My Master"
    ]
  },
  {
    title: "Soul Eater",
    subs: [
      "Soul Eater (1-51)",
      "Soul Eater: Late Night Show (1-51)",
      "Soul Eater Not! (1-12)"
    ]
  },
  {
    title: "To Love Ru -Trouble-",
    subs: [
      "To Love Ru -Trouble- (1-26)",
      "To Love Ru -Trouble- OVA (1-6)",
      "Motto To Love Ru -Trouble- (1-12)",
      "To Love Ru -Trouble- Darkness OVA (1)",
      "To Love Ru -Trouble- Darkness (1-10)",
      "To Love Ru -Trouble- Darkness OVA (2-3)",
      "To Love Ru -Trouble- Darkness (11-12)",
      "To Love Ru -Trouble- Darkness OVA (4-6)",
      "To Love Ru -Trouble- Darkness 2nd (1-10)",
      "To Love Ru -Trouble- Darkness 2nd OVA (1)",
      "To Love Ru -Trouble- Darkness 2nd (11-12)",
      "To Love Ru -Trouble- Darkness 2nd Specials (1-2)",
      "To Love Ru -Trouble- Darkness 2nd OVA (2-3)",
      "To Love Ru -Trouble- Multiplication: Mae kara Ushiro kara"
    ]
  },
  {
    title: "Tsuki ga Michibiku Isekai Dōchū",
    subs: [
      "Tsuki ga Michibiku Isekai Dōchū (1-12)",
      "Tsuki ga Michibiku Isekai Dōchū Dainimaku (1-25)"
    ]
  },
  {
    title: "Urusei Yatsura",
    subs: [
      "Urusei Yatsura (1-21)",
      "Urusei Yatsura: Haru da, Tobidase!",
      "Urusei Yatsura (22-58)",
      "Urusei Yatsura: Only You",
      "Urusei Yatsura (59-99)",
      "Urusei Yatsura 2: Beautiful Dreamer",
      "Urusei Yatsura (100-140)",
      "Urusei Yatsura 3: Remember My Love",
      "Urusei Yatsura (141-151)",
      "Urusei Yatsura Memorial Album: I'm the Owari-chan",
      "Urusei Yatsura (152-165)",
      "Urusei Yatsura: The Shougaibutsu Suieitaikai",
      "Urusei Yatsura (166-174)",
      "Urusei Yatsura: Ryōko no Kugatsu no Ochakai",
      "Urusei Yatsura (175-191)",
      "Urusei Yatsura 4: Lum the Forever",
      "Urusei Yatsura (192-195)",
      "Urusei Yatsura: Denki Jikake no Oniwaban",
      "Urusei Yatsura: Reikon to Date",
      "Urusei Yatsura: Yume no Shikakenin, Inaba-kun Toujou! Lum no Mirai wa Dounaruccha!?",
      "Urusei Yatsura: Nagisa no Fiancé",
      "Urusei Yatsura: Ikare!! Sherbet",
      "Urusei Yatsura: Otome Bashika no Kyoufu",
      "Urusei Yatsura: Yagi-san to Cheese",
      "Urusei Yatsura: Tsuki ni Hoeru",
      "Urusei Yatsura: Heart wo Tsukame",
      "Urusei Yatsura: Itsudatte My Darling",
      "Urusei Yatsura: Kanketsuhen",
      "Urusei Yatsura (1-23)",
      "Urusei Yatsura (1-23)"
    ]
  },
  {
    title: "Violet Evergarden",
    subs: [
      "Violet Evergarden (1-4)",
      "Violet Evergarden: Kitto \"Ai\" wo Shiru Hi ga Kuru no Darō",
      "Violet Evergarden (5-10)",
      "Violet Evergarden: Tokubetsu Sōshū-ban",
      "Violet Evergarden (11-13)",
      "Violet Evergarden Gaiden: Eien to Jidō Shuki Ningyū",
      "Gekijōban Violet Evergarden"
    ]
  },
  {
    title: "Yōkoso Jitsuryoku Shijō Shugi no Kyōshitsu e",
    subs: [
      "Yōkoso Jitsuryoku Shijō Shugi no Kyōshitsu e (1-12)",
      "Yōkoso Jitsuryoku Shijō Shugi no Kyōshitsu e 2nd Season (1-13)",
      "Yōkoso Jitsuryoku Shijō Shugi no Kyōshitsu e 3rd Season (1-13)"
    ]
  },
  {
    title: "Zero no Tsukaima",
    subs: [
      "Zero no Tsukaima (1-13)",
      "Zero no Tsukaima Futatsuki no Kishi (1-12)",
      "Zero no Tsukaima Princesses no Rondo (1-6)",
      "Zero no Tsukaima Princesses no Rondo: Yuuwaku no Sunahama",
      "Zero no Tsukaima Princesses no Rondo (7-12)",
      "Zero no Tsukaima Princesses no Rondo: Picture Drama (1-7)",
      "Zero no Tsukaima F (1-12)"
    ]
  }
];

const mainColor = "#4285f4";
const bgColor = "#f8fafc";
const cardColor = "#fff";
const borderRadius = 18;
const shadow = "0 6px 32px rgba(60,72,98,0.11)";
const font = `Roboto, Arial, "Segoe UI", sans-serif`;

export default function AnimeList() {
  const [open, setOpen] = useState({});

  const toggle = (idx) => {
    setOpen((prev) => ({
      ...prev,
      [idx]: !prev[idx],
    }));
  };

  return (
    <div style={{
      minHeight: "100vh",
      background: bgColor,
      fontFamily: font,
      padding: 0,
      margin: 0,
      boxSizing: "border-box"
    }}>
      <header style={{
        textAlign: "center",
        padding: "60px 0 36px 0",
        letterSpacing: 2
      }}>
        <h1 style={{
          color: mainColor,
          fontSize: "clamp(2.2rem, 4vw, 3.5rem)",
          fontWeight: 800,
          margin: 0,
          textShadow: "0 2px 8px rgba(66,133,244,0.08)"
        }}>
          My Anime List
        </h1>
      </header>
      <main style={{
        maxWidth: 520,
        margin: "0 auto",
        padding: "0 12px"
      }}>
        {animeList.map(({ title, subs }, idx) => (
          <section key={title} style={{
            marginBottom: 16,
            transition: "all 0.2s"
          }}>
            <button
              onClick={() => toggle(idx)}
              aria-expanded={!!open[idx]}
              style={{
                width: "100%",
                textAlign: "left",
                background: cardColor,
                border: `1.5px solid ${mainColor}33`,
                borderRadius,
                boxShadow: open[idx] ? shadow : "0 2px 8px rgba(60,72,98,0.08)",
                padding: "18px 24px",
                fontSize: "clamp(1.1rem, 2vw, 1.35rem)",
                fontWeight: 600,
                color: "#292929",
                cursor: "pointer",
                outline: "none",
                display: "flex",
                alignItems: "center",
                gap: 14,
                transition: "all 0.22s"
              }}
            >
              <span style={{
                flexGrow: 1,
                letterSpacing: 1
              }}>
                {title}
              </span>
              <span style={{
                color: mainColor,
                fontSize: "clamp(1.3rem, 2vw, 1.6rem)",
                fontWeight: 400,
                lineHeight: 1
              }}>
                {open[idx] ? "▲" : "▼"}
              </span>
            </button>
            <div
              style={{
                maxHeight: open[idx] ? 520 : 0,
                overflow: "hidden",
                transition: "max-height 0.35s cubic-bezier(.6,1.2,.45,1)",
                background: cardColor,
                borderRadius: `${borderRadius}px`,
                borderTopLeftRadius: open[idx] ? 0 : borderRadius,
                borderTopRightRadius: open[idx] ? 0 : borderRadius,
                marginTop: open[idx] ? 0 : "-12px",
                boxShadow: open[idx] ? shadow : "none"
              }}
            >
              {open[idx] && (
                <ul style={{
                  margin: 0,
                  padding: "10px 32px 18px 32px",
                  listStyle: "disc",
                  color: "#505050",
                  fontSize: "clamp(0.97rem, 1.7vw, 1.08rem)",
                  lineHeight: 1.7
                }}>
                  {subs.map((sub, subIdx) => (
                    <li key={subIdx} style={{
                      marginBottom: 4,
                      wordBreak: "break-word"
                    }}>
                      {sub}
                    </li>
                  ))}
                </ul>
              )}
            </div>
          </section>
        ))}
      </main>
      <link
        rel="stylesheet"
        href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;600;700;800&display=swap"
      />
    </div>
  );
}
