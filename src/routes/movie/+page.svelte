<style>
    :root {
    --primary-color: rgb(75, 19, 28);
    --secodary-color: rgb(38, 6, 7);
}

* {
    box-sizing:  border-box;
}

main {
    display: flex;
    flex-wrap: wrap;
}

body{
    background-color:  var(--primary-color);
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    margin: 0;
}

header {
    padding: 10px;
    display: flex;
    justify-content: flex-end;
    background-color: var(--secodary-color);
}

.search {
    background-color: transparent;
    border: 2px solid var(--primary-color);
    border-radius: 50px;
    font-family: inherit;
    font-size: 14px;
    padding: 20px 10px;
}

.search::placeholder {
    color: rgb(164, 82, 101);
}

.search.search:focus{
    outline: none;
    background-color: rgb(214, 180, 180);
}

.movie {
    width: 300px;
    margin: 10px;
    background-color: var(--secodary-color);
    box-shadow: 0 4px 5px rgba(0, 0, 0, 0.2);
    position: relative;
    overflow: hidden;
    border-radius: 3px;
}

.movie img{
    width: 100%;
}

.movie-info {
    color: rgb(240, 215, 215);
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 20px 30px 30px;
    letter-spacing: 0.5px;
}

.movie-info h3{
    margin-top: 0;
}

.movie-info span{
    background-color: var(--primary-color);
    padding: 25px 5px;
    border-radius: 3px;
    font-weight: bold;
}

.movie-info span.green{
    color: rgb(238, 144, 155);
}

.overview {
    background-color: rgb(246, 198, 216);
    padding: 20px;
    position: absolute;
    left: 0;
    bottom: 0;
    right: 0;
    max-width: 100%;
    transform: translateY(101%);
    transition: transform 0.3s ease-in;
}

.movie:hover .overview{
    transform: translateY(0)
}
</style>

<main id="main">
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Гравити фолз</h3>
            <span class="green">9.0</span>
        </div>
        <div class="overview">
            <h3 id="Description">американский анимационный телевизионный сериал, созданный Алексом Хиршем и компанией Disney Television Animation для телеканалов Disney Channel и Disney XD</h3>
        </div>
    </div>
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Леди баг</h3>
            <span class="green">9.3</span>
        </div>
        <div class="overview">
            <h3 id="Description">французский мультсериал производства Zagtoon и Method Animation для детей раннего подросткового возраста</h3>
        </div>
    </div>
    
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Маша и медведь</h3>
            <span class="green">7.9</span>
        </div>
        <div class="overview">
            <h3 id="Description">О дружбе и приключениях маленькой озорной девочки Маши и ее заботливого друга Медведя.</h3>
        </div>
    </div>
    
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Сказочный патруль</h3>
            <span class="green">7.8</span>
        </div>
        <div class="overview">
            <h3 id="Description"> российский анимационный детский мультсериал студии «Паровоз». Повествует о приключениях четырёх девочек-волшебниц, приехавших в город Мышкин. </h3>
        </div>
    </div>
    
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Удивительный мир гамбола</h3>
            <span class="green">9.9</span>
        </div>
        <div class="overview">
            <h3 id="Description">англо-американский мультсериал производства телеканала Cartoon Network, выпущенный в эфир 3 мая 2011 года в Великобритании, 9 мая того же года — в США</h3>
        </div>
    </div>
</main>