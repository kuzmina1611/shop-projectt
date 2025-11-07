<template>
  <div class="complete-look">
    <h2 class="section-title">Complete the Look</h2>
    
    <div class="cards-container">
      
      <div class="product-card" 
           @mouseenter="hoveredCard = 1" 
           @mouseleave="hoveredCard = null">
        <div class="main-image">
          <img src="/1.jpg" alt="Main Product" class="main-img">
          
          <div class="product-dot" style="top: 39%; left: 42%;" 
               @mouseenter="activeDot = 1" @mouseleave="activeDot = null">
            <div class="dot-circle" :class="{ 'dot-visible': hoveredCard === 1 }"></div>
          </div>
          
          <div class="product-dot" style="top: 74%; left: 14%;" 
               @mouseenter="activeDot = 3" @mouseleave="activeDot = null">
            <div class="dot-circle" :class="{ 'dot-visible': hoveredCard === 1 }"></div>
          </div>
          
          <div class="product-dot" style="top: 83%; left: 95%;" 
               @mouseenter="activeDot = 4" @mouseleave="activeDot = null">
            <div class="dot-circle" :class="{ 'dot-visible': hoveredCard === 1 }"></div>
          </div>
          
          <div class="product-info" v-if="activeDot === 1" style="top: 59%; left: 62%;">
            <div class="info-content">
              <div class="brand">NOCTA</div>
              <div class="name">Fleece CS Hoodie 2</div>
              <div class="price">$120</div>
            </div>
          </div>
        
          <div class="product-info" v-if="activeDot === 3" style="top: 71%; left: 40%;">
            <div class="info-content">
              <div class="brand">Nike Everyday Plus Cushioned</div>
              <div class="name">Training Ankle Socks (6 Pairs)</div>
              <div class="price">$21.97</div>
            </div>
          </div>
          
          <div class="product-info" v-if="activeDot === 4" style="top: 80%; left: 76%;">
            <div class="info-content">
              <div class="brand">NOCTA Zoom Drive</div>
              <div class="name">Men's Shoes</div>
              <div class="price">$107.97</div>
            </div>
          </div>
          
          <div class="view-details-button">
            <div class="view-details">
              <div class="view-details-icon">
                <img src="/eye.jpg" alt="View Details" class="eye-icon">
                <div class="eye-open-indicator" :class="{ 'visible': hoveredCard === 1 }"></div>
              </div>
              <span class="view-items-text">View Entire Look</span>
            </div>
          </div>
        </div>
      </div>

      <div class="product-card" 
           @mouseenter="hoveredCard = 2" 
           @mouseleave="hoveredCard = null">
        <div class="main-image">
          <img src="/2.jpg" alt="Main Product" class="main-img">
          
          <div class="product-dot" style="top: 13%; left: 20%;" 
               @mouseenter="activeDot = 5" @mouseleave="activeDot = null">
            <div class="dot-circle" :class="{ 'dot-visible': hoveredCard === 2 }"></div>
          </div>
          
          <div class="product-dot" style="top: 18%; left: 88%;" 
               @mouseenter="activeDot = 6" @mouseleave="activeDot = null">
            <div class="dot-circle" :class="{ 'dot-visible': hoveredCard === 2 }"></div>
          </div>
          
          <div class="product-dot" style="top: 70%; left: 23%;" 
               @mouseenter="activeDot = 7" @mouseleave="activeDot = null">
            <div class="dot-circle" :class="{ 'dot-visible': hoveredCard === 2 }"></div>
          </div>
          
          <div class="product-dot" style="top: 81%; left: 93%;" 
               @mouseenter="activeDot = 9" @mouseleave="activeDot = null">
            <div class="dot-circle" :class="{ 'dot-visible': hoveredCard === 2 }"></div>
          </div>
          
          <div class="product-info" v-if="activeDot === 5" style="top: 34%; left: 40%;">
            <div class="info-content">
              <div class="brand">Nike Life</div>
              <div class="name">Men's Wilderness Sweater</div>
              <div class="price">$157.97</div>
            </div>
          </div>
          
          <div class="product-info" v-if="activeDot === 6" style="top: 39%; left: 69%;">
            <div class="info-content">
              <div class="brand">Nike Club</div>
              <div class="name">Unstructured Cap</div>
              <div class="price">$18.97</div>
            </div>
          </div>
          
          <div class="product-info" v-if="activeDot === 7" style="top: 67%; left: 43%;">
            <div class="info-content">
              <div class="brand">Nike Recharge</div>
              <div class="name">Tritan Chug Bottle (24 oz)</div>
              <div class="price">$26</div>
            </div>
          </div>
          
          <div class="product-info" v-if="activeDot === 9" style="top: 78%; left: 74%;">
            <div class="info-content">
              <div class="brand">Nike Court Vision Low Next Nature</div>
              <div class="name">Men's Shoes</div>
              <div class="price">$85</div>
            </div>
          </div>
          
          <div class="view-details-button">
            <div class="view-details">
              <div class="view-details-icon">
                <img src="/eye.jpg" alt="View Details" class="eye-icon">
                <div class="eye-open-indicator" :class="{ 'visible': hoveredCard === 2 }"></div>
              </div>
              <span class="view-items-text">View Entire Look</span>
            </div>
          </div>
        </div>
      </div>

      <div class="product-card" 
           @mouseenter="hoveredCard = 3" 
           @mouseleave="hoveredCard = null">
        <div class="main-image">
          <img src="/3.jpg" alt="Main Product" class="main-img">
          
          <div class="product-dot" style="top: 13%; left: 19%;" 
               @mouseenter="activeDot = 10" @mouseleave="activeDot = null">
            <div class="dot-circle" :class="{ 'dot-visible': hoveredCard === 3 }"></div>
          </div>
          
          <div class="product-dot" style="top: 22%; left: 86%;" 
               @mouseenter="activeDot = 11" @mouseleave="activeDot = null">
            <div class="dot-circle" :class="{ 'dot-visible': hoveredCard === 3 }"></div>
          </div>
          
          <div class="product-dot" style="top: 74%; left: 11%;" 
               @mouseenter="activeDot = 12" @mouseleave="activeDot = null">
            <div class="dot-circle" :class="{ 'dot-visible': hoveredCard === 3 }"></div>
          </div>
          
          <div class="product-dot" style="top: 81%; left: 93%;" 
               @mouseenter="activeDot = 14" @mouseleave="activeDot = null">
            <div class="dot-circle" :class="{ 'dot-visible': hoveredCard === 3 }"></div>
          </div>
          
          <div class="product-info" v-if="activeDot === 10" style="top: 34%; left: 40%;">
            <div class="info-content">
              <div class="brand">Nike</div>
              <div class="name">Men's Max90 Fitness T-Shirt</div>
              <div class="price">$27.97</div>
            </div>
          </div>
          
          <div class="product-info" v-if="activeDot === 11" style="top: 47%; left: 66%;">
            <div class="info-content">
              <div class="brand">Nike Victory Road Tint</div>
              <div class="name">Sunglasses</div>
              <div class="price">$175</div>
            </div>
          </div>
          
          <div class="product-info" v-if="activeDot === 12" style="top: 71%; left: 34%;">
            <div class="info-content">
              <div class="brand">Nike Everyday Essential</div>
              <div class="name">Ankle Socks (3 Pairs)</div>
              <div class="price">$22</div>
            </div>
          </div>
          
          <div class="product-info" v-if="activeDot === 14" style="top: 78%; left: 73%;">
            <div class="info-content">
              <div class="brand">Nike Court Vision Low Next Nature</div>
              <div class="name">Men's Shoes</div>
              <div class="price">$85</div>
            </div>
          </div>
          
          <div class="view-details-button">
            <div class="view-details">
              <div class="view-details-icon">
                <img src="/eye.jpg" alt="View Details" class="eye-icon">
                <div class="eye-open-indicator" :class="{ 'visible': hoveredCard === 3 }"></div>
              </div>
              <span class="view-items-text">View Entire Look</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const activeDot = ref(null)
const hoveredCard = ref(null)
</script>

<style scoped>
.complete-look {
  width: 100%;
  margin: 0;
  padding: 60px 10px 20px;
  background: white;
}

.section-title {
  font-size: 28px;
  font-weight: 600;
  margin-bottom: 20px;
  color: #000;
  text-align: left;
  padding-left: 10px;
}

.cards-container {
  display: flex;
  gap: 10px;
  justify-content: center;
  flex-wrap: nowrap;
  overflow-x: auto;
  padding: 10px 2px;
}

.product-card {
  width: 400px;
  height: 495px;
  background: white;
  border: 1px solid #f0f0f0;
  flex-shrink: 0;
  position: relative;
}

.main-image {
  position: relative;
  width: 100%;
  height: 495px;
  overflow: hidden;
  background: #cec0c0ff;
}

.main-img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.product-dot {
  position: absolute;
  width: 24px;
  height: 24px;
  cursor: pointer;
  transform: translate(-50%, -50%);
  z-index: 10;
}

.dot-circle {
  width: 15px;
  height: 15px;
  background: #fff;
  border: 2px solid #929292af;
  border-radius: 1300%;
  transition: all 0.2s ease;
  opacity: 0;
}

.dot-visible {
  opacity: 1;
}

.product-dot:hover .dot-circle {
  background: #979797da;
  transform: scale(1.2);
}

.product-info {
  position: absolute;
  transform: translate(-50%, -100%);
  z-index: 20;
}

.info-content {
  background: white;
  padding: 16px;
  border-radius: 8px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.15);
  min-width: 160px;
  border: 1px solid #f0f0f0;
}

.brand {
  font-size: 13px;
  font-weight: 600;
  color: #000;
  margin-bottom: 4px;
  text-transform: uppercase;
}

.name {
  font-size: 13px;
  font-weight: 500;
  color: #646464;
  margin-top: -4px;
}

.price {
  font-size: 14px;
  font-weight: 600;
  color: #000;
}

.view-details-button {
  position: absolute;
  bottom: 12px;
  left: 12px;
  cursor: pointer;
  z-index: 5;
}

.view-details {
  display: flex;
  align-items: center;
  background: #fff;
  border-radius: 30px;
  padding: 0 8px;
  min-height: 36px;
  height: 36px;
  width: 36px;
  transition: width 0.2s ease-in-out;
  overflow: hidden;
  box-shadow: 0 2px 8px rgba(0,0,0,0.1);
  justify-content: flex-start;
}

.view-details-icon {
  width: 20px;
  height: 20px;
  border-radius: 50%;
  overflow: hidden;
  flex-shrink: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  background: transparent;
  margin-left: 2px;
  position: relative;
}

.eye-icon {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 50%;
}

.eye-open-indicator {
  position: absolute;
  top: 50%;
  left: 50%;
  width: 8px;
  height: 8px;
  border-radius: 50%;
  transform: translate(-50%, -50%);
  opacity: 0;
  transition: opacity 0.2s ease;
}

.eye-open-indicator.visible {
  opacity: 1;
}

.view-items-text {
  font-size: 13px;
  font-weight: 500;
  color: #212121;
  white-space: nowrap;
  margin-left: 8px;
  opacity: 0;
  transition: opacity 0.1s ease-in-out 0.05s;
  display: flex;
  align-items: center;
}

.view-details-button:hover .view-details {
  width: 150px;
  padding: 0 12px;
}

.view-details-button:hover .view-details-icon {
  margin-left: 0;
}

.view-details-button:hover .view-items-text {
  opacity: 1;
}
</style>