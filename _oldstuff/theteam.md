---
layout: default
title: The Team
permalink: /teampage
image: header-12.jpeg
---


{% include section_numbers.html title="The Team" content="Our team is as diverse as the audience we serve, consisting of members
    with different personalities, cultures and experiences. A strong commitment and a passion for social
    impact and effecting positive change is what has brought us together.<br><br>
    We combine all our skills and knowledge to come up with new and creative ways of communicating with our
    readers and instigating positive social change across the whole of Sub-Saharan Africa.<br><br>
    We believe that teamwork, a constant desire to improve, and humbleness to our cause are the key
    ingredients to achieving our goals. However, none of this would be possible without the countless
    experts from around the globe who donate their time and knowledge.<br><br>
    Working together, with an ever expanding community of dedicated men and women, we provide the necessary
    tools that can help change the world!"

  %}

{% include section_large_img.html image_path="img/RED/Czybik_Bansah_BridgeHohoe011.jpg" %}

  <div class="section">

  <div class="container">
  <div class="title-area">
      <h2>Management</h2>
      <div class="separator separator-danger"></div>
  </div>
      <div class="text-area">
          {% for entry in site.data.team %}
              <div class="row">
                  <div class="col-md-4">
                      <div class="title-area">
                          <h3 style="margin-top: 0px">{{ entry.name }}</h3>
                          <h4>{{ entry.title }}</h4>
                      </div>
                  </div>
                  <div class="col-md-8">
                      <div class="description">
                          <p class=" text-justify">{{ entry.info }}
                          </p>
                      </div>
                  </div>
              </div>
              <br><br>
              {% endfor %}
          </div>
        </div>
  </div>

  <div class="section section-gray">

  <div class="container">
  <div class="title-area">
      <h2>The Board</h2>
      <div class="separator separator-danger"></div>
  </div>
      <div class="text-area">
          {% for entry in site.data.board %}
              <div class="row">
                  <div class="col-md-4">
                      <div class="title-area">
                          <h3 style="margin-top: 0px">{{ entry.name }}</h3>
                          <h4>{{ entry.title }}</h4>
                      </div>
                  </div>
                  <div class="col-md-8">
                      <div class="description">
                          <p class="text-justify">{{ entry.info  }}
                          </p>
                      </div>
                  </div>
              </div>
              <br><br>
              {% endfor %}
          </div>
        </div>
  </div>
