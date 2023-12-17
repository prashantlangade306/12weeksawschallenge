[tracks_list.json](https://github.com/prashantlangade306/12weeksawschallenge/files/13694281/tracks_list.json)1. Overview of the AWS analytics architecture

![1](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/9cbf1eaf-bc8e-4896-bc10-512f6255a7a8)

2. Create S3 bucket as below 
![2](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/6d1f0efc-d218-4f72-9151-daabf73175eb)

3. Create a folder named "data" inside that S3 bucket
![3](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/33d2d697-16c8-40c4-80bb-91bc54ef319d)

4. Create a folder named "reference_data" inside that folder
![4](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/89780e29-8f54-4197-aec8-74313528f97a)

5. Upload the tracks_list.json file to the bucket
[Uploa{"track_id" : "1" , "track_name" : "God's Plan" , "artist_name" : "Drake"}
{"track_id" : "2" , "track_name" : "Meant To Be" , "artist_name" : "Bebe Rexha & Florida Georgia Line"}
{"track_id" : "3" , "track_name" : "Perfect" , "artist_name" : "Ed Sheeran"}
{"track_id" : "4" , "track_name" : "Finesse" , "artist_name" : "Bruno Mars & Cardi B"}
{"track_id" : "5" , "track_name" : "Psycho" , "artist_name" : "Post Malone Featuring Ty Dolla $ign"}
{"track_id" : "6" , "track_name" : "The Middle" , "artist_name" : "Zedd, Maren Morris & Grey"}
{"track_id" : "7" , "track_name" : "Sad!" , "artist_name" : "XXXTentacion"}
{"track_id" : "8" , "track_name" : "Havana" , "artist_name" : "Camila Cabello Featuring Young Thug"}
{"track_id" : "9" , "track_name" : "Freaky Friday" , "artist_name" : "Lil Dicky Featuring Chris Brown"}
{"track_id" : "10" , "track_name" : "Pray For Me" , "artist_name" : "The Weeknd & Kendrick Lamar"}
{"track_id" : "11" , "track_name" : "Look Alive" , "artist_name" : "BlocBoy JB Featuring Drake"}
{"track_id" : "12" , "track_name" : "Stir Fry" , "artist_name" : "Migos"}
{"track_id" : "13" , "track_name" : "Ric Flair Drip" , "artist_name" : "Offset & Metro Boomin"}
{"track_id" : "14" , "track_name" : "All The Stars" , "artist_name" : "Kendrick Lamar & SZA"}
{"track_id" : "15" , "track_name" : "Mine" , "artist_name" : "Bazzi"}
{"track_id" : "16" , "track_name" : "New Rules" , "artist_name" : "Dua Lipa"}
{"track_id" : "17" , "track_name" : "Let You Down" , "artist_name" : "NF"}
{"track_id" : "18" , "track_name" : "Rockstar" , "artist_name" : "Post Malone Featuring 21 Savage"}
{"track_id" : "19" , "track_name" : "Never Be The Same" , "artist_name" : "Camila Cabello"}
{"track_id" : "20" , "track_name" : "Walk It Talk It" , "artist_name" : "Migos Featuring Drake"}
{"track_id" : "21" , "track_name" : "Him & I" , "artist_name" : "G-Eazy & Halsey"}
{"track_id" : "22" , "track_name" : "Thunder" , "artist_name" : "Imagine Dragons"}
{"track_id" : "23" , "track_name" : "Plug Walk" , "artist_name" : "Rich The Kid"}
{"track_id" : "24" , "track_name" : "Whatever It Takes" , "artist_name" : "Imagine Dragons"}
{"track_id" : "25" , "track_name" : "I Fall Apart" , "artist_name" : "Post Malone"}
{"track_id" : "26" , "track_name" : "Lights Down Low" , "artist_name" : "MAX Featuring gnash"}
{"track_id" : "27" , "track_name" : "King's Dead" , "artist_name" : "Jay Rock, Kendrick Lamar, Future & James Blake"}
{"track_id" : "28" , "track_name" : "Friends" , "artist_name" : "Marshmello & Anne-Marie"}
{"track_id" : "29" , "track_name" : "Wait" , "artist_name" : "Maroon 5"}
{"track_id" : "30" , "track_name" : "Heaven" , "artist_name" : "Kane Brown"}
{"track_id" : "31" , "track_name" : "Marry Me" , "artist_name" : "Thomas Rhett"}
{"track_id" : "32" , "track_name" : "Say Something" , "artist_name" : "Justin Timberlake Featuring Chris Stapleton"}
{"track_id" : "33" , "track_name" : "Bad At Love" , "artist_name" : "Halsey"}
{"track_id" : "34" , "track_name" : "Feel It Still" , "artist_name" : "Portugal. The Man"}
{"track_id" : "35" , "track_name" : "Moonlight" , "artist_name" : "XXXTentacion"}
{"track_id" : "36" , "track_name" : "You Make It Easy" , "artist_name" : "Jason Aldean"}
{"track_id" : "37" , "track_name" : "Changes" , "artist_name" : "XXXTentacion"}
{"track_id" : "38" , "track_name" : "Bartier Cardi" , "artist_name" : "Cardi B Featuring 21 Savage"}
{"track_id" : "39" , "track_name" : "Outside Today" , "artist_name" : "YoungBoy Never Broke Again"}
{"track_id" : "40" , "track_name" : "Lemon" , "artist_name" : "NERD & Rihanna"}
{"track_id" : "41" , "track_name" : "Wolves" , "artist_name" : "Selena Gomez X Marshmello"}
{"track_id" : "42" , "track_name" : "Love." , "artist_name" : "Kendrick Lamar Featuring Zacari"}
{"track_id" : "43" , "track_name" : "MotorSport" , "artist_name" : "Migos, Nicki Minaj & Cardi B"}
{"track_id" : "44" , "track_name" : "No Limit" , "artist_name" : "G-Eazy Featuring A$AP Rocky & Cardi B"}
{"track_id" : "45" , "track_name" : "New Freezer" , "artist_name" : "Rich The Kid Featuring Kendrick Lamar"}
{"track_id" : "46" , "track_name" : "Young Dumb & Broke" , "artist_name" : "Khalid"}
{"track_id" : "47" , "track_name" : "Most People Are Good" , "artist_name" : "Luke Bryan"}
{"track_id" : "48" , "track_name" : "How Long" , "artist_name" : "Charlie Puth"}
{"track_id" : "49" , "track_name" : "Found / Tonight" , "artist_name" : "Lin-Manuel Miranda & Ben Platt"}
{"track_id" : "50" , "track_name" : "Sky Walker" , "artist_name" : "Miguel Featuring Travis Scott"}
{"track_id" : "51" , "track_name" : "Powerglide" , "artist_name" : "Rae Sremmurd & Juicy J"}
{"track_id" : "52" , "track_name" : "All On Me" , "artist_name" : "Devin Dawson"}
{"track_id" : "53" , "track_name" : "Love Lies" , "artist_name" : "Khalid & Normani"}
{"track_id" : "54" , "track_name" : "Dura" , "artist_name" : "Daddy Yankee"}
{"track_id" : "55" , "track_name" : "Broken Halos" , "artist_name" : "Chris Stapleton"}
{"track_id" : "56" , "track_name" : "Everyday" , "artist_name" : "Logic & Marshmello"}
{"track_id" : "57" , "track_name" : "Singles You Up" , "artist_name" : "Jordan Davis"}
{"track_id" : "58" , "track_name" : "IDGAF" , "artist_name" : "Dua Lipa"}
{"track_id" : "59" , "track_name" : "X" , "artist_name" : "Nicky Jam x J Balvin"}
{"track_id" : "60" , "track_name" : "Five More Minutes" , "artist_name" : "Scotty McCreery"}
{"track_id" : "61" , "track_name" : "Billy" , "artist_name" : "6ix9ine"}
{"track_id" : "62" , "track_name" : "Top Off" , "artist_name" : "DJ Khaled Featuring JAY Z, Future & B"}
{"track_id" : "63" , "track_name" : "Gummo" , "artist_name" : "6ix9ine"}
{"track_id" : "64" , "track_name" : "No Excuses" , "artist_name" : "Meghan Trainor"}
{"track_id" : "65" , "track_name" : "Hardaway" , "artist_name" : "Derez De'Shon"}
{"track_id" : "66" , "track_name" : "Delicate" , "artist_name" : "Taylor Swift"}
{"track_id" : "67" , "track_name" : "The Remedy For A Broke Heart (Why Am I So In Love)" , "artist_name" : "XXXTentacion"}
{"track_id" : "68" , "track_name" : "Zombie" , "artist_name" : "Bad Wolves"}
{"track_id" : "69" , "track_name" : "El Farsante" , "artist_name" : "Ozuna & Romeo Santos"}
{"track_id" : "70" , "track_name" : "44 More" , "artist_name" : "Logic"}
{"track_id" : "71" , "track_name" : "Pick It Up" , "artist_name" : "Famous Dex Featuring A$AP Rocky "}
{"track_id" : "72" , "track_name" : "In My Blood" , "artist_name" : "Shawn Mendes"}
{"track_id" : "73" , "track_name" : "Tell Me You Love Me" , "artist_name" : "Demi Lovato"}
{"track_id" : "74" , "track_name" : "The Long Way" , "artist_name" : "Brett Eldredge"}
{"track_id" : "75" , "track_name" : "Red Roses" , "artist_name" : "Lil Skies Featuring Landon Cube"}
{"track_id" : "76" , "track_name" : "Betrayed" , "artist_name" : "Lil Xan"}
{"track_id" : "77" , "track_name" : "NBAYoungboat" , "artist_name" : "Lil Yachty Featuring NBA YoungBoy"}
{"track_id" : "78" , "track_name" : "When We" , "artist_name" : "Tank"}
{"track_id" : "79" , "track_name" : "No Smoke" , "artist_name" : "YoungBoy Never Broke Again"}
{"track_id" : "80" , "track_name" : "I Like Me Better" , "artist_name" : "Lauv"}
{"track_id" : "81" , "track_name" : "Nowadays" , "artist_name" : "Lil Skies Featuring Landon Cube"}
{"track_id" : "82" , "track_name" : "Numb" , "artist_name" : "XXXTentacion"}
{"track_id" : "83" , "track_name" : "Infinity (888)" , "artist_name" : "XXXtentacion Featuring Joey Bada$$"}
{"track_id" : "84" , "track_name" : "One Number Away" , "artist_name" : "Luke Combs"}
{"track_id" : "85" , "track_name" : "I Lived It" , "artist_name" : "Blake Shelton"}
{"track_id" : "86" , "track_name" : "Sit Next To Me" , "artist_name" : "Foster The People"}
{"track_id" : "87" , "track_name" : "Tequila" , "artist_name" : "Dan + Shay"}
{"track_id" : "88" , "track_name" : "Narcos" , "artist_name" : "Migos"}
{"track_id" : "89" , "track_name" : "Booty" , "artist_name" : "Blac Youngsta"}
{"track_id" : "90" , "track_name" : "She's With Me" , "artist_name" : "High Valley"}
{"track_id" : "91" , "track_name" : "Sativa" , "artist_name" : "Jhene Aiko Featuring Swae Lee Or Rae Sremmurd"}
{"track_id" : "92" , "track_name" : "Written In The Sand" , "artist_name" : "Old Dominion"}
{"track_id" : "93" , "track_name" : "Beautiful Trauma" , "artist_name" : "P!nk"}
{"track_id" : "94" , "track_name" : "Tempo" , "artist_name" : "Chris Brown"}
{"track_id" : "95" , "track_name" : "Going Down!" , "artist_name" : "XXXTentacion"}
{"track_id" : "96" , "track_name" : "At The Club" , "artist_name" : "Jacquees X Dej Loaf"}
{"track_id" : "97" , "track_name" : "Echame La Culpa" , "artist_name" : "Luis Fonsi & Demi Lovato"}
{"track_id" : "98" , "track_name" : "La Modelo" , "artist_name" : "Ozuna x Cardi B"}
{"track_id" : "99" , "track_name" : "Dark Knight Dummo" , "artist_name" : "Trippie Redd Featuring Travis Scott"}
{"track_id" : "100" , "track_name" : "Everybody Hates Me" , "artist_name" : "The Chainsmokers"}ding tracks_list.json…]()

![5](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/205f9772-9266-4266-8095-864662555a81)

![6E](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/80feff9e-fcf4-4884-bd99-90bb27ad66a6)

![7](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/50f8b401-79a1-43a9-92af-d476289b843e)
![8](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/da832aa1-ef34-4d4b-8353-7055b39f6478)
![9](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/201a0ff0-77f1-4d68-b19b-feb8d58e443d)
![10](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/febfda23-9e63-4900-9b5f-9d1435002845)
![11](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/79ba4acd-d5ce-4efc-8dc0-4542c863bdde)
![12](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/c002748b-0e82-4a5b-aa49-e0b54af89b5e)
![13](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/d473865a-66ea-4928-92d4-f396e3411429)
![14](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/ecf45f4d-3355-4ce5-a571-c54c362406d2)
![15](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/0bd8c0b9-71f7-4cc5-96bb-78b313d81510)
![16](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/2e33d58b-e057-4bda-ab11-508ea7d8aab8)
![17](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/909daa8d-a86c-4414-969c-23c18a3637e4)
![18](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/1558fe62-4398-4422-a242-150332ab0fd6)
![19](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/dd1d8897-af2e-4181-858a-55ac3bfe59dd)
![20](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/ace59e66-769c-45a8-b19d-6722c558a9f8)
![21](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/a0ae256e-acbc-471e-9973-15b0106b8b90)
![22](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/0216cf25-ae2c-4c39-9226-6afe79d07b5d)
![23](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/eddd52b3-686a-45ad-a9fb-9ec1e9e12b49)
![24](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/837a6fd0-e689-40a1-9468-06b68afd11db)
![25](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/005631e3-9905-4014-9c83-0114f869f4cd)
![26](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/a7464d6c-ad5d-47ba-84d7-eade09981f64)
![27](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/2671e530-d2d0-4c07-a454-196135848651)

![28E](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/6a7f7996-ffd9-46a5-9beb-de63379cd33c)


![29](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/7e5808ec-391d-418a-9674-561139210061)
![30](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/ed57b44f-fbeb-4f9e-9773-6f595d124574)
![31](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/cf8da5e8-f54d-457b-b623-0da7f58a7fa8)
![32](https://github.com/prashantlangade306/12weeksawschallenge/assets/57378421/e7477300-cb85-4fc5-bd75-94aeef7387e7)
