---
layout: post
title: About
permalink: /about/
comments: true
---

## As a conversation Starter

Here are some places I have lived.

<comment>
Flags are made using Wikipedia images
</comment>

<style>
    /* Style looks pretty compact, 
       - grid-container and grid-item are referenced the code 
    */
    .grid-container {
        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(150px, 1fr)); /* Dynamic columns */
        gap: 10px;
    }
    .grid-item {
        text-align: center;
    }
    .grid-item img {
        width: 100%;
        height: 100px; /* Fixed height for uniformity */
        object-fit: contain; /* Ensure the image fits within the fixed height */
    }
    .grid-item p {
        margin: 5px 0; /* Add some margin for spacing */
    }

    .image-gallery {
        display: flex;
        flex-wrap: nowrap;
        overflow-x: auto;
        gap: 10px;
        }

    .image-gallery img {
        max-height: 150px;
        object-fit: cover;
        border-radius: 5px;
    }
</style>

<!-- This grid_container class is used by CSS styling and the id is used by JavaScript connection -->
<div 
    class="grid-container" id="grid_container">
    <!-- content will be added here by JavaScript -->
</div>

<script>
   // Get the output element
    const outputElement = document.getElementById('grid_container');
    
    // Clear the output
    outputElement.innerHTML = '';

    // Data array
    const living_in_the_world = [
    {flag: "https://upload.wikimedia.org/wikipedia/commons/0/01/Flag_of_California.svg", greeting: "Hey", description: "California - forever"},
    {flag: "https://upload.wikimedia.org/wikipedia/commons/thumb/4/47/Flag_of_Virginia.svg/960px-Flag_of_Virginia.svg.png?20250807185748", greeting: "Hi", description: "Virginia"},
    {flag: "https://upload.wikimedia.org/wikipedia/commons/thumb/1/19/Flag_of_San_Diego%2C_California.svg/960px-Flag_of_San_Diego%2C_California.svg.png?20220727153107", greeting: "Hey man", description: "San Diego"},
    {flag: "https://upload.wikimedia.org/wikipedia/commons/thumb/5/55/Flag_of_San_Francisco%2C_California.svg/960px-Flag_of_San_Francisco%2C_California.svg.png?20220809152454", greeting: "Hello", description: "San Fransicos"}
    ];

    // Use the existing container
    const container = outputElement;
    container.style.border = '2px solid';
    container.style.padding = '10px';

    // Loop through data and create grid items
    for (const location of living_in_the_world) {
    // Create grid item
    const gridItem = document.createElement('div');
    gridItem.style.textAlign = 'center';
    
    // Create a flag image
    const img = document.createElement('img');
    img.src = location.flag;
    img.alt = location.description + ' Flag';
    img.style.width = '100%';
    img.style.height = '100px';
    img.style.objectFit = 'contain';
    
    // Create a description
    const description = document.createElement('p');
    description.textContent = location.description;
    description.style.margin = '5px 0';
    description.style.fontWeight = 'bold';
    
    // Create a greeting
    const greeting = document.createElement('p');
    greeting.textContent = location.greeting;
    greeting.style.margin = '5px 0';
    greeting.style.fontStyle = 'italic';
    greeting.style.opacity = '0.7';
    
    // Add all elements to grid item
    gridItem.appendChild(img);
    gridItem.appendChild(description);
    gridItem.appendChild(greeting);
    
    // Add grid item to container
    container.appendChild(gridItem);
    }
</script>


### Journey through Life

Here is what I did at those places
-  Born In Virginia
- 🏫 Moved to San Fransciso, went to  most of elementry school there
- 🏫 4th grade, 5th grade, middle school and highschool in San Deigo 
- 🎓 Oak valley middle school was my middle school 
- 🎓 Student at Del Norte 

### Culture, Family, and Fun

Everything for me, as for many others, revolves around family.

- I am mainly of German and English desent  [family tree]({{site.baseurl}}/images/about/familytree.png)
- I have 2 siblings along with my mom and dad
- The gallery of pics has some of my family, fun, culture memories.

<comment>
Gallery of Pics, scroll to the right for more ...
</comment>
<div class="image-gallery">
  <img src="https://cdn1.parksmedia.wdprapps.disney.com/resize/mwImage/1/1260/711/75/vision-dam/digital/parks-platform/parks-global-assets/disneyland/events/70th-anniversary/attraction/0237_DLR_70_Environmentals_05212025_JS_B-SUPERMOD-16x9.jpg?2025-06-04T20:48:29+00:00" alt="Image 1">
  <img src="https://www.travelmanagers.com.au/wp-content/uploads/2018/03/AdobeStock_116567811-kauai-hawaii-1-scaled.jpeg" alt="Image 2">
  <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTW_6h9l2IPUP9b-MveZR1kCwoBqoKDWjWNYQ&s" alt="Image 3">
  <img src="{{site.baseurl}}/images/about/surf.jpg" alt="Image 4">
  <img src="{{site.baseurl}}/images/about/john_lora.jpg" alt="Image 5">
  <img src="{{site.baseurl}}/images/about/lora_fam.jpg" alt="Image 6">
  <img src="{{site.baseurl}}/images/about/lora_fam2.jpg" alt="Image 7">
  <img src="{{site.baseurl}}/images/about/pj_party.jpg" alt="Image 8">
  <img src="{{site.baseurl}}/images/about/trent_family.png" alt="Image 9">
  <img src="{{site.baseurl}}/images/about/claire.jpg" alt="Image 10">
  <img src="{{site.baseurl}}/images/about/grandkids.jpg" alt="Image 11">
  <img src="{{site.baseurl}}/images/about/farm.jpg" alt="Image 12">
</div>