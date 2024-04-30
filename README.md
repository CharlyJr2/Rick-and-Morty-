# Rick-and-Morty-
const API_URL = 'https://rickandmortyapi.com/api';

const searchCharacters = async (name) => {
  const response = await fetch(`${API_URL}/character/?name=${name}`);
  const data = await response.json();
  return data.results;
};
