<template>
  <div id="app">
    <single-image :img-src="firstImage.src" :img-alt="firstImage.alt"></single-image>
    <single-section :title="firstSection.title" :paragraphs="firstSection.paragraphs"></single-section>
    <single-section :title="secondSection.title" :paragraphs="firstSection.paragraphs"></single-section>
    <single-image :img-src="secondImage.src" :img-alt="secondImage.alt"></single-image>
    <single-section :title="thirdSection.title" :paragraphs="thirdSection.paragraphs"></single-section>
    <single-section :title="fourthSection.title" :paragraphs="fourthSection.paragraphs"></single-section>
    <single-image :img-src="thirdImage.src" :img-alt="thirdImage.alt"></single-image>
    <single-section :title="fifthSection.title" :paragraphs="fifthSection.paragraphs"></single-section>
    <single-section :title="sixthSection.title" :paragraphs="sixthSection.paragraphs"></single-section>
    <single-image :img-src="fourthImage.src" :img-alt="fourthImage.alt"></single-image>
  </div>
</template>

<script>
import singleSection from "./components/shared/singleSection";
import singleImage from "./components/shared/singleImage";

export default {
  name: 'App',
  components: {
    singleSection,
    singleImage
  },
  data() {
    return {
      firstImage: {
        src: 'laptop_2.png',
        alt: 'Opis obrazka'
      },
      secondImage: {
        src: 'laptop_3.png',
        alt: 'Opis obrazka'
      },
      thirdImage: {
        src: 'laptop_4.png',
        alt: 'Opis obrazka'
      },
      fourthImage: {
        src: 'laptop_5.png',
        alt: 'Opis obrazka'
      },
      sixthImage: {
        src: 'laptop_6.png',
        alt: 'Opis obrazka'
      },
      seventhImage: {
        src: 'laptop_7.png',
        alt: 'Opis obrazka'
      },
      firstSection: {
        title: 'Pomysłowe technologie dla wszystkich',
        paragraphs: [
          'Lenovo poszerza zakres możliwości w nowych laptopach Yoga opracowanych wspólnie z firmą Intel® i wyposażonych w funkcje sztucznej inteligencji. Teraz możesz mówić do urządzenia i nim sterować z drugiego końca pokoju. Oglądać wideo o podwyższonej jakości w programie Windows Media Player. Unikać zmęczenia oczu dzięki wyświetlaczowi, który automatycznie zmniejsza natężenie światła niebieskiego odpowiednio do pory dnia. A to jeszcze nie wszystko.',
        ]
      },
      secondSection: {
        title: 'Sztuczna inteligencja i zdrowy rozsądek',
        paragraphs: [
          'Zaawansowany procesor Intel® Core™ 10. generacji do urządzeń mobilnych i utraprzenośny laptop Yoga S740 dostosowują się do Twoich potrzeb i stylu użytkowania. Razem tworzą rozwiązanie bardziej intuicyjne i osobiste, którego sztuczna inteligencja dynamicznie reaguje na Twoje działania i optymalizuje żywotność baterii.'
        ]
      },
      thirdSection: {
        title: 'Potrzebujesz czegoś? Wystarczy poprosić.',
        paragraphs: [
          'Yoga S740 ma mikrofony dalekiego zasięgu i inteligentne asystentki głosowe Alexę oraz Cortanę. Pomogą Ci złożyć zamówienie, ustawić przypomnienie czy odtworzyć muzykę — wystarczy poprosić z odległości do 4 metrów. To kolejny przykład przewagi, jaką daje Ci Yoga S740.',
          'Aby uzyskać więcej informacji o Cortanie, kliknij tutaj , a w celu uzyskania dodatkowych informacji o Alexie, kliknij tutaj.'
        ]
      },
      fourthSection: {
        title: 'Mobilne kino',
        paragraphs: [
          'Wyświetlacz o przekątnej 14 cali w wąskiej jak brzytwa ramce prezentuje imponującą gamę kolorów i szczegółów. Ekran do poziomu 4K VESA400 HDR z jasnością 500 nitów i spektakularną technologią Dolby Vision™ oraz bogaty, wielowarstwowy dźwięk 3D z głośników z Dolby Atmos® oferują niezwykle realistyczną i wciągającą rozrywkę.'
        ]
      },
      fifthSection: {
        title: 'Nie ma gniazdka? Nie ma problemu.',
        paragraphs: [
          'Niezależnie od tego, czy pracujesz w terenie, czy też urządzasz sobie serialową noc na sofie, bateria eleganckiego i smukłego Yoga S740 ma w sobie wystarczająco dużo energii — na nawet 15 godzin działania.'
        ]
      },
      sixthSection: {
        title: 'Nowy poziom wydajności',
        paragraphs: [
          'Opcjonalna dedykowana karta graficzna NVIDIA® GeForce® MX250 zwiększa dodatkowo możliwości laptopa w zastosowaniach służbowych i rozrywkowych. Korzystaj z nawet 3,5-krotnie większej wydajności w porównaniu ze zintegrowaną kartą graficzną w aplikacjach do edycji zdjęć i wideo, a także z szybszej i płynniejszej gry.'
        ]
      }
    }
  }
}
</script>

<style>
  .container {
    max-width: 1321px;
    width: 100%;
    margin: 0 auto;
  }
</style>
