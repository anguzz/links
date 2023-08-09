<script>
    import { links } from './links.ts';
  </script>

  <div class="container">
    {#each links as link}
      <a class="box" href={link.link} target="_blank">
        {link.name}
      </a>
    {/each}
  </div>
  

  <style>
    .container {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: flex-start;
      margin-top: 50px;
      
    }
  
    .box {
      width: 60%;
      height: 2vw;
      background-color: #b1dfec;
      margin: 10px;
      display: flex;
      align-items: center;
      justify-content: center;
      cursor: pointer;
      transition: background-color 0.3s ease;
      border-radius: 10px;
      font-size: 2rem;
    }
  
    .box:hover {
      background-color: #7bffd5;
    }
  
    @media screen and (max-width: 600px) {
      .box {
        font-size: 1.5rem; /* mobile */
        height: 10%;

      }
    }

    a:link {
  text-decoration: none;
  color:#2e3541;
}

a:visited {
  text-decoration: none;
  color:#2e3541;

}

a:hover {
  text-decoration: none;
  color:#2e3541;

}

a:active {
  text-decoration: none;
  color:#2e3541;

}
  </style>
  
  