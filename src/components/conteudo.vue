<script setup>

import Corpo2 from '../components/corpo.vue'
import Cabecalho from '../components/Cabecalho.vue'
import img2 from '../assets/img1.jpg'
import img3 from '../assets/img2.jpg'
import img4 from '../assets/img3.jpg'
import gif1 from '../assets/gif1.gif'
import gif2 from '../assets/gif2.gif'
import gif3 from '../assets/gif3.gif'
</script>

<template>

  <header>

    
    
    <br>
    <Corpo2 :post="img2" 
      titulo="DETECTIVE CONAN COMPLETA 20 ANOS COM LANÇAMENTO DE SEU 20° FILME NOS CINEMAS"
      txt=" So, as to what Conan explained, it all adds up. Conan suddenly realizes what really happens, and says 
      So that's how it is. then Ayumi asks Conan-kun! Where are you going? 
      Conan ignores the question and rushes to the hospital and the room where the man is being kept under treatment.
       So, he spots the nurse and tells her and the police that she's the one who is also responsible for all of this happening.
        She then feels bad and starts to cry. The man then wakes up, and relief and tears of joy spreads throughout the room.
        And I was like Yay! A happy ending! :D." 
         
    />
   
    <br>
   
    <Corpo2 :post="img3" 
      titulo="o 20° filme da série, a misteriosa Organização Negra volta a dar as caras, com assassinatos ocorrendo pelo mundo inteiro." 
      txt=" The solution? Well, the doctor (excuse me for not being familiar with knowing their names.) 
      noticed the man from before, and the man had a knife and said that he promised he would operate for him, 
      but he said to him that he just lied, so yeah, he tried to attack him with the knife. But the doctor had self defense,
       so he struggled with the man, pushed him back, and the man hit the back of his head on the bench and his button
        from his jacket flew off on the ground. The paint was still fresh since it was near a site where things were still
         being constructed, so some of the paint went on the man's jacket. Apparently, the doctor went inside his car, 
         and drove off. Whereas the taxi part comes in afterwords, when he still has the urge to find him, and takes a cab,
          to go searching. Where one of the guys at first gets
       mistaken as the culprit, since he happens to run into the taxi on his way back from someplace.."
      
    /> 
    <br>
  
    <Corpo2 :post="img4" 
      titulo="filme da série, a misteriosa Organização"
      txt= "Ayumi has a big heart. She cares for one, even if one can seem cold hearted. I felt sympathy for her when she said she 
      felt sorry for the man who threatened to attack her. So, she really wanted to help him. And Conan and the others agreed, 
      and so that's how this mystery really started going. :D  What were my deductions during this case? Well, I was very concerned 
      about the paint on the man's jacket. It was obvious that there was blood on the back of this head, so I was assuming he hit his 
      head, and was soon later to fall to the ground after he grabbed Ayumi, and passed out because of the wound. At first, I thought 
      the paint came from the taxi, but it wasn't the same color. Then I saw the bench, and at first, I wasn't thinking much of it, 
      other than I saw blood on it, I didn't notice the threads on the bench until Haibara pointed it out. Then there was the button. 
      And I was assuming the the button fell off when he was in a struggle with someone. At the time, I didn't know that the doctor
       was the man who attacked him, but with his power of deduction, Conan revealed the truth! And that poster, well, I know it 
       was taped to the bench, and I noticed a red spot on the back of the paper when the wind blew it. Then Genta grabbed it,and
        noticed his most favorite food eel rice. And Mitsuhiko was like"
           
    /> 
   
    
    <br>
  
   
  </header>

  <RouterView />
</template>

<style scoped>

.teste{
  width: 100vh;
  
}
span{
  color: rgb(255, 255, 255);
 
}



</style>
