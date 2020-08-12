<style lang="scss">
h2 {
  padding: 1em 0 0;
}
.gallery {
  height: 65vh;
  overflow: scroll;
}
.img-link {
  max-width: 26em;
  padding:.25em .5em;
  display: inline-block;
}
a {
  cursor: pointer;
    img {
      width:25em;
    &:hover {
      width: 100%;
    }
  }
}
</style>

<script>
import Index from "./blog/index.svelte";

let imgs = [
  {
    filename: 'Aabal-Heating-Cooling.jpg',
    url: 'http://www.aabal.com/',
    alt: 'Aabal Heating and Cooling website',
  },
  {
    filename: 'Action-Fire-Equipment.jpg',
    url: 'http://action-fire.com/',
    alt: "Action Fire Equipment Inc website",
  },
  {
    filename: 'Alta-Ridge.jpg',
    url: 'http://altaridge.com/',
    alt: 'Alta Ridge communities website',
  },
  {
    filename: 'AM-PM-Movers.jpg',
    url: 'http://ampmmovers.com/',
    alt: 'AM PM movers Knoxville, Tennessee website',
  },
  {
    filename: 'Arlington-School-of-Music.jpg',
    url: 'http://arlingtonschoolofmusic.com/',
    alt: 'Arlington School of Music website',
  },
  {
    filename: 'Bell-Law.jpg',
    url: 'http://www.bell-law.com/',
    alt: 'Bell, Gould, and Scott P.C. website',
  },
  {
    filename: 'Christopher-John-Design.jpg',
    url: 'http://christopherjohndesigns.com/',
    alt: 'Christopher John Design website',
  },
  {
    filename: 'Collier-Podiatry.jpg',
    url: 'https://collierpodiatry.com/',
    alt: 'Collier Podiatry',
  },
  {
    filename: 'Gresham-Injury-Law.jpg',
    url: 'http://greshaminjurylaw.com/',
    alt: 'Gresham Injury Law',
  },
  {
    filename: 'JK-Landscape.jpg',
    url: 'https://web.archive.org/web/20150117075222/http://jklandscape.com/',
    alt: 'JK Landscape website',
  },
  {
    filename: 'Kreisler-Law.jpg',
    url: 'http://kreislerlaw.com/',
    alt: 'Kreisler Law website',
  },
  {
    filename: 'Latah-Creek.jpg',
    url: 'http://latahcreekfamilydentistry.com/',
    alt: 'Latah Creek website',
  },
  {
    filename: 'McCrea-PC.jpg',
    url: 'http://mccreapc.com/',
    alt: 'McCrea PC website',
  },
  {
    filename: 'Modern-Pump-Inc.jpg',
    url: 'http://modernpumpinc.com/',
    alt: 'Modern Pump Inc, website',
  },
  {
    filename: 'MS-Glass-Outlet.jpg',
    url: 'http://msglassoutlet.com/',
    alt: 'MS Glass Outlet website',
  },
  {
    filename: 'Mueller-Interiors.jpg',
    url: 'https://www.muellerinteriors.com/',
    alt: 'Mueller Interiors website',
  },
  {
    filename: 'O-L-Door.jpg',
    url: 'http://oandldoorsystems.com/',
    alt: 'O & L Door Systems website',
  },
  {
    filename: 'Reliable-Transportation.jpg',
    url: 'http://www.reliabletrans.com/',
    alt: 'Reliable Transportation website',
  },
  {
    filename: 'The-Safety-Team.jpg',
    url: 'http://thesafetyteaminc.com/',
    alt: 'The Safety Team Inc website',
  },
  {
    filename: 'Septic-Technologies.jpg',
    url: 'http://septictechnologies.com/',
    alt: 'Septic Technologies website',
  },
  {
    filename: 'SWFNA.jpg',
    url: 'http://swfna.com/',
    alt: 'Southwest Florida Nuerosurgical & Rehab Associations website',
  },
  {
    filename: 'Valley-Oak.jpg',
    url: 'http://valleyoakdentalgroup.com/',
    alt: 'Valley Oak Dental Group website',
  },
  {
    filename: 'Star-Brite.jpg',
    url: 'http://star-brite.com/',
    alt: 'Star Brite Learning program website',
  },

  {
    filename: 'Zobrist-Law.jpg',
    url: 'http://www.zoblaw.com/',
    alt: 'Zobrist Law website',
  },
  
]
</script>

<h1>Portfolio</h1>

<div class="gallery">
  {#each imgs as img}
  <a class="img-link" href={img.url} target="_blank">
      <img src="/images/{img.filename}" alt={img.alt} />
  </a>
  {/each}
</div>

<h2>Other projects</h2>
<p>While my major body of work is not suitable to show in galleries, I have done work for the following products/contracts:</p>
<ul>
  <li>Supply Chain tracker</li>
  <li>Foreign Aid tracking dashboards - USAID</li>
  <li>Provider enrollment for medicare - CMS</li>
  <li>Diplomat training resources library - State Department</li>
  <li>ShareAmerica.gov - State Department</li>
</ul>
