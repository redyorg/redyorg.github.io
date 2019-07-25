---
layout: default
title: Our Partners
subtitle: Some subtitle
permalink: /partnerino
image: header-12.jpeg
---
{% include section_numbers.html
  title="Our Partners"
  content="Our partners form the pillars of our success. Outstanding organisations and individuals from all over the world, along with our community on the ground in Ghana, continue to provide their unwavering support for our mission. Our unified resolve to improve the lives of others guarantees Right For Education’s place at the forefront of social change in Sub-Saharan Africa."
%}



{% include section_img_right_text.html
  title="African Partners"
  subtitle="A short message from Ewefiaga Togbui  AGBOLI K. F. AGOKOLI  IV"
  content=" \"As the king of the Ewe in Togo and a member of the National Human Rights Commission, I work with many NGOs in Togo, particularly in the field of education, because I strongly believe in all the possibilities that education can enable a person to fulfil. These possibilities are endless and we should devote time and effort to educating children as well as adults, now for a better and stronger future.\"<br><br>
  Togbui endorses R:Ed for its unique esteem for culture, traditions and African values: \"I support the Right for Education project founded by Dr. Susann Dattenberg-Doyle, Nana Ngoryisi Dziwornu of Gbi Kpoeta (Ghana) for the promotion of education in Africa.”.<br><br>Ewefiaga Togbui  AGBOLI K. F. AGOKOLI  IV<br>
  Chef canton de Notsé<br>
  Président du Conseil des Chefs Traditionnels du Togo (CNCTT)<br>
  Membre de la Commission Nationale des Droits de l\’Homme (CNDH)"
  image_path="/img/RED/king.png"
  text-width="6"
  img-width="6"
%}



<div class="section">

<div class="container">
    <div class="text-area">
        {% for entry in site.data.partners %}
        {% assign partner = entry.partner %}

            <div class="row">
                <div class="col-md-4">
                    <div class="title-area">
                        <h2 style="margin-top: 0px">{{ entry.type }}</h2>
                        <h4>{{ entry.title }}</h4>
                    </div>
                </div>
                <div class="col-md-8">
                    <div class="description">
                        <p class=" text-justify">{{ entry.desc }}</p>
                        {% for item in partner %}
                        <strong class=" text-justify"><a href="{{ item.link }}">{{ item.name }}</a></strong><br>
                        {% endfor %}


                    </div>
                </div>
            </div>
            <br><br>
            {% endfor %}
        </div>
      </div>
</div>

{% include section_parallax.html
 title="To learn more about how you can partner with us, please email: "
 button-text="hello@rightforeducation.org"
 image_path="img/RED/Czybik-Accra-Fisher-Col039.jpg"
%}
