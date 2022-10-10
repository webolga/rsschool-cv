# Olga Kulczycka

## Contact info

- **Telephone number:** +48664112683
- **Email:** ok.supergirl@ukr.net
- **Telegram:** @olgakulczycka

## Summary

I am a beginner web developer from Szczecin, Poland. I design web products and bring them to life. I create modern design and correct layout of sites. I also adapt each site for tablets and mobile devices. In my work I use Git, Gulp, Sass and Scss preprocessors to optimize my work and get the work done as early as possible. Also I work with bootstrap if needed in the project. I try to please every client.

## Skills

- **Languages:** JavaScript, HTML5, CSS3, Scss, Sass
- **Other:** Git/Github, Figma

## Code examples

```
const personalMovieDB = {
  count: 0,
  movies: {},
  actors: {},
  genre: [],
  privat: false,
  start: function() {
    personalMovieDB.count = +prompt("Сколько фильмов вы уже посмотрели?", "");

    while (personalMovieDB.count == "" || personalMovieDB.count == null || isNaN(personalMovieDB.count)) {
      personalMovieDB.count = +prompt("Сколько фильмов вы уже посмотрели?", "");
    }
  },
  rememberMyFilms: function() {
  for (let i = 0; i < 2; i++) {
    const a = prompt("Один из поcледних просмотренных фильмов?", ""),
          b = prompt("На сколько оцените его?", "");

    if (a != null && b != null && a != "" && b != "" && a.lenght < 50) {
      personalMovieDB.movies[a] = b;
      console.log('done');
    } else {
      console.log('error');
      i--;
    }
  }
  },
  detectPersonalLevel: function() {
  if (personalMovieDB.count < 10) {
    console.log("Просмотрено довольно мало фильмов");
  } else if (personalMovieDB.count >= 10 && personalMovieDB.count < 30) {
    console.log("Вы классический зриетель");
  } else if (personalMovieDB.count >=30) {
    console.log("Вы киноман");
  } else {
    console.log("Произошла ошибка");
  }
  },
  showMyDB: function(hidden) {
  if (!hidden) {
    console.log(personalMovieDB);
  }
  },
  toggleVisibleMyDB: function() {
    if (personalMovieDB.privat) {
      personalMovieDB.privat = false;
    } else {
      personalMovieDB.privat = true;
    }
  },
  writeYourGenre: function() {
    for (let i = 1; i < 2; i++) {

      let genre = prompt(`Введите ваши любимые жанры через запятую `).toLowerCase();

      if (genre === '' || genre == null) {
        console.log('Вы ввели некоректные данные или не ввели их совсем');
        i--;
      } else {
        personalMovieDB.genre = genre.split(', ');
        personalMovieDB.genre.sort();
      }
    }

    personalMovieDB.genre.forEach((item, i) => {
      console.log(`Любимый жанр ${i + 1} - это ${item}`);
    });
  }
};

```

##  Experience

Here you can see my projects [GitHub Pages - Olga Kulczycka](https://yakolga.github.io/portfolio/).

##  Education

- Maritime University of Szczecin, Engineering degree Szczecin, Poland
- Web - developer 2020, Udemy
- JavaScript + React course, Udemy
- PHP for beginners: How to Biuld an Ecommerce Store, Udemy

##  Languages

- **English** - B2, certificate by English Cert
- **Polish** - C1
- **Russian** - native
- **Ukrainian** - native
