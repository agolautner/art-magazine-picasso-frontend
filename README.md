# React Art Magazine / Team Project

This project was created by me and four classmates at Codecool, in collaboration with teams from the backend, sysadmin and manual testing courses. The main idea was to create a webapp which, after basic authentication, allows the user to search for artworks using the Art Institute Chicago API, save any of the results to their own collection, append tags and comments to the individual pieces of art, as well as rate them with stars. Saved artworks and any data added by the user should then be sent to a backend server.

## Design and Wireframing

The design of the page, as well as initial sketches and a high-fidelity wireframe, were done by me personally, using Figma and Photoshop. In choosing the color scheme for the original design, I took inspiration from a random painting by Picasso, and added a couple more matching colors using an online color picker tool. The idea was that search results would be rendered as cards, and arranged in a single row. This would later change into a responsive, grid-like layout.

![desktop wireframe](https://github.com/agolautner/react-art-magazine-frontend/blob/main/wireframe/picasso-desktop-1.png?raw=true)

## API call & Rendering results

Any search query longer than 2 characters is sent to the Artic API. Additionally, the search function accepts other parameters specifying the type of data we wish to get back from the API, such as 'thumbnail' or 'place_of_origin'. If the response contains no data, or the request fails, the error is caught. Otherwise, the results are saved into a state, then individual cards are rendered out by mapping through the results. 

![search results layout](https://github.com/agolautner/react-art-magazine-frontend/blob/main/wireframe/search-results.png?raw=true)
