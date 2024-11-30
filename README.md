const url = 'https://api.themoviedb.org/3/authentication';
const options = {
  method: 'GET',
  headers: {
    accept: 'application/json',
    Authorization: 'Bearer eyJhbGciOiJIUzI1NiJ9.eyJhdWQiOiI2MGM5OGMxZDhjYjlmMGU0MzZiZmJiZjA1OWE3YzAzOCIsIm5iZiI6MTQ2NjM1ODczNi41NTcsInN1YiI6IjU3NjZkYmQwYzNhMzY4MjNmMjAwMDFhOCIsInNjb3BlcyI6WyJhcGlfcmVhZCJdLCJ2ZXJzaW9uIjoxfQ.hxOUMko_eujG1cZf-ZYxoz4T9Q2B5LcKupBQwSIhlrA'
  }
};

fetch(url, options)
  .then(res => res.json())
  .then(json => console.log(json))
  .catch(err => console.error(err));# mobie
