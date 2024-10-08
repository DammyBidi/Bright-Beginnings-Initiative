<template>
  <div class="body">
    <nav>
      <div class="logo">
        <img src="../src/assets/images/Frame 26085726.png" alt="" />
        <h4>
          Bright <br />
          Beginnings <br />
          Initiative
        </h4>
      </div>
      <div class="nav-link">
        <p>Who we are</p>
        <p>What we do</p>
        <p>Research Blog</p>
        <p>Contact a Volunteer</p>
      </div>
      <div>
        <button>Donate</button>
      </div>
      <div class="menu-icon" @click="toggleMenu">
        <img
          v-if="!menuOpen"
          src="../src/assets/images/nav-icon.svg"
          alt="nav-icon"
        />
        <img
          v-if="menuOpen"
          src="../src/assets/images/cancel.svg"
          alt="Cancel Icon"
        />
      </div>
      <ul :class="{ 'nav-items': true, open: menuOpen }">
        <li>
          <p>Who we are</p>
        </li>
        <li>
          <p>What we do</p>
        </li>
        <li>
          <p>Research Blog</p>
        </li>
        <li>
          <p>Contact a Volunteer</p>
        </li>
        <li>
          <button>Donate</button>
        </li>
      </ul>
    </nav>

    <div :class="{'content': true, 'blurred': menuOpen}">
      <!-- Hero -->
      <div class="hero">
        <div class="hero-text">
          <h1>
            Igniting Hope, <br />
            Inspiring Chance
          </h1>
          <p>
            At Bright Beginning Initiative, we are committed to transforming the
            lives of children through dedicated support and innovative programs.
            Our mission is to provide every child with access to quality
            education, healthcare, and a nurturing community
          </p>
          <button>Donate</button>
        </div>
      </div>

      <!-- Meet-section -->

      <div class="Meet-section">
        <h2>Meet Us</h2>
        <p>
          At Bright Beginning Initiative, we are dedicated to transforming the
          lives of children through comprehensive welfare programs. Our mission
          is to ensure every child has access to education, healthcare, and a
          supportive community. We believe in nurturing potential and creating a
          brighter future for the next generation. Join us in making a
          difference, one child at a time.
        </p>
        <button>Learn More</button>
      </div>

      <!-- News Section-->

      <div class="news-section">
        <h2>News</h2>
        <div class="news-one">
          <div class="news-image">
            <img src="../src/assets/images/News1.svg" alt="" />
          </div>
          <div class="news-text">
            <div>
              <h4>Conflict</h4>
              <img src="../src/assets/images/line.svg" alt="" />
            </div>
            <h3>War On Gaza</h3>
            <p>
              The ongoing conflict in Gaza has devastating effects on children,
              stripping them of safety, education, and basic necessities.
              Innocent lives are lost, and countless children are left
              traumatized. Our mission is to provide essential support and hope
              for a peaceful future
            </p>
            <div class="more">
              <p>Read more</p>
              <img src="../src/assets/images/arrow.svg" alt="arrow" />
            </div>
          </div>
        </div>
        <div class="news-two">
          <div class="news-image">
            <img src="../src/assets/images/News2.png" alt="" />
          </div>
          <div class="news-text">
            <div>
              <h4>Digest</h4>
              <img src="../src/assets/images/line.svg" alt="" />
            </div>
            <h3>War Against Child Solider</h3>
            <p>
              Child soldiers are robbed of their childhood and forced into
              unimaginable situations. This practice not only endangers their
              lives but also leaves deep psychological scars. At Bright
              Beginning Initative, we are committed to ending this grave
              injustice and helping these children reclaim their futures. Join
              us in the fight to protect and restore the lives of vulnerable
              children.
            </p>
            <div class="more">
              <p>Read more</p>
              <img src="../src/assets/images/arrow.svg" alt="arrow" />
            </div>
          </div>
        </div>
        <div class="news-three">
          <div class="news-image">
            <img src="../src/assets/images/News3.png" alt="" />
          </div>
          <div class="news-text">
            <div>
              <h4>Insight</h4>
              <img src="../src/assets/images/line.svg" alt="" />
            </div>
            <h3>Child Labour</h3>
            <p>
              Child labor is a global crisis that robs children of their
              childhood, education, and future. It exposes them to dangerous
              conditions, stunts their development, and perpetuates the cycle of
              poverty. Ending child labor is crucial to ensuring every child can
              grow up in a safe, healthy, and nurturing environment. Together,
              we can fight this injustice and protect our children's rights and
              futures.
            </p>
            <div class="more">
              <p>Read more</p>
              <img src="../src/assets/images/arrow.svg" alt="arrow" />
            </div>
          </div>
        </div>
      </div>

      <!-- Project -->
      <div class="project-section">
        <h2>Project</h2>
        <div class="project-container">
          <div class="project-text">
            <h4>Vision 2025</h4>
            <h1>
              Empowering <br />
              2Milion children <br />
              around the world
            </h1>
            <p>
              We're excited to announce a $200 million initiative dedicated to
              empowering children. This funding will provide vital resources for
              education, healthcare, and community support, helping to build a
              brighter future for our youth.
            </p>
            <button>Learn More</button>
          </div>
          <div class="project-image">
            <img src="../src/assets/images/Project.svg" alt="project-image" />
          </div>
          <div class="mobile-projectImage">
            <img
              src="../src/assets/images/mobile-project.svg"
              alt="project-image"
            />
          </div>
        </div>
      </div>

      <!-- Blog -->

      <div class="blog-section">
        <h1>Blog</h1>
        <div class="blog-top">
          <div class="blog-left">
            <div class="blog-image">
              <img
                src="../src/assets/images/Blog-image1.svg"
                alt="blog-image"
              />
            </div>
            <div class="blog-text">
              <h3>War on Gaza</h3>
              <p>
                The ongoing conflict in Gaza has devastating effects on
                children, stripping them of safety, education, and basic
                necessities. Innocent lives are lost, and countless children are
                left traumatized. Our mission is to provide essential support
                and hope for a peaceful future
              </p>
              <div class="more">
                <p>Read more</p>
                <img src="../src/assets/images/arrow.svg" alt="arrow" />
              </div>
            </div>
          </div>
          <div class="blog-right">
            <div class="blog-image">
              <img
                src="../src/assets/images/Blog-image1.svg"
                alt="blog-image"
              />
            </div>
            <div class="blog-text">
              <h3>War on Gaza</h3>
              <p>
                The ongoing conflict in Gaza has devastating effects on
                children, stripping them of safety, education, and basic
                necessities. Innocent lives are lost, and countless children are
                left traumatized. Our mission is to provide essential support
                and hope for a peaceful future
              </p>
              <div class="more">
                <p>Read more</p>
                <img src="../src/assets/images/arrow.svg" alt="arrow" />
              </div>
            </div>
          </div>
        </div>

        <div class="blog-bottom">
          <div class="blog-left">
            <div class="blog-image">
              <img
                src="../src/assets/images/Blog-image1.svg"
                alt="blog-image"
              />
            </div>
            <div class="blog-text">
              <h3>War on Gaza</h3>
              <p>
                The ongoing conflict in Gaza has devastating effects on
                children, stripping them of safety, education, and basic
                necessities. Innocent lives are lost, and countless children are
                left traumatized. Our mission is to provide essential support
                and hope for a peaceful future
              </p>
              <div class="more">
                <p>Read more</p>
                <img src="../src/assets/images/arrow.svg" alt="arrow" />
              </div>
            </div>
          </div>
          <div class="blog-right">
            <div class="blog-image">
              <img
                src="../src/assets/images/Blog-image1.svg"
                alt="blog-image"
              />
            </div>
            <div class="blog-text">
              <h3>War on Gaza</h3>
              <p>
                The ongoing conflict in Gaza has devastating effects on
                children, stripping them of safety, education, and basic
                necessities. Innocent lives are lost, and countless children are
                left traumatized. Our mission is to provide essential support
                and hope for a peaceful future
              </p>
              <div class="more">
                <p>Read more</p>
                <img src="../src/assets/images/arrow.svg" alt="arrow" />
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- Our Reach -->

      <div class="reach-section">
        <h1>Our Reach</h1>
        <p>
          We're reaching out today to share our passion for improving children's
          lives around the world through the [Your Foundation Name] initiative.
          We believe that every child deserves the opportunity to thrive,
          regardless of their background or location our reach extends far
          beyond borders. We have active programs and partnerships in numerous
          countries, making a tangible difference in the lives of children
          across the globe
        </p>
        <div class="reach-image">
          <img src="../src/assets/images/map-base.svg" alt="reach-image" />
        </div>
        <button class="reach-button">
          <img src="../src/assets/images/copy-image.svg" alt="" />
          <p>View out report</p>
        </button>
      </div>

      <!-- Impact Section -->

      <div class="impact-section">
        <h1>See Your Impact</h1>
        <p>
          Documenting our Impact, Ensuring <br />
          Transparency and Accountability
        </p>
        <div class="button">
          <p>Show all</p>
          <img src="../src/assets/images/Arrow2.svg" alt="arrow" />
        </div>
      </div>

      <!-- Our partners -->

      <div class="partner-section">
        <h1>Our Partners</h1>
        <div class="partner-container"  ref="PartnerContainer">
          <div class="partner-image">
            <img
              src="../src/assets/images/ubongo_logo.png.svg"
              alt="partner-image"
            />
          </div>
          <div class="partner-image">
            <img
              src="../src/assets/images/ubongo_logo.png.svg"
              alt="partner-image"
            />
          </div>
          <div class="partner-image">
            <img
              src="../src/assets/images/ubongo_logo.png.svg"
              alt="partner-image"
            />
          </div>
        </div>
      </div>

      <!-- Footer -->
      <footer>
        <div class="footer-left">
          <h1>
            Subscribe to our <br />
            newsletter
          </h1>
          <div>
            <input type="email" placeholder="name@gmail.com" />
            <button>Subscribe</button>
          </div>
        </div>
        <div class="footer-right">
          <div class="footer-links">
            <h4>Menu</h4>
            <p>Who we are</p>
            <p>What we do</p>
            <p>Research Blog</p>
            <p>Contact a Volunteer</p>
          </div>
          <div class="footer-links">
            <h4>Follow Us</h4>
            <p>x/Twitter</p>
            <p>Linkedin</p>
            <p>Instagram</p>
          </div>
        </div>
      </footer>

      <hr />

      <div class="footer-bottom">
        <p>© 2024 Bright Beginnings Initiative. All rights reserved</p>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref, watch, onMounted } from "vue";


const menuOpen = ref(false);

const toggleMenu = () => {
  menuOpen.value = !menuOpen.value;
};

const PartnerContainer = ref<HTMLElement | null>(null);

const startContinuousScrolling = (
  container: HTMLElement,
  direction: "left" 
) => {
  const scrollSpeed = 3;

  const content = container.innerHTML;
  container.innerHTML += content;

  const scroll = () => {
    if (direction === "left") {
      container.scrollLeft += scrollSpeed;
      if (container.scrollLeft >= container.scrollWidth / 2) {
        container.scrollLeft = 0;
      }
    }

    requestAnimationFrame(scroll);
  };

  scroll();
};

onMounted(() => {
  if (PartnerContainer.value) {
    startContinuousScrolling(PartnerContainer.value, "left");
  }
});


</script>

<style scoped>


</style>
