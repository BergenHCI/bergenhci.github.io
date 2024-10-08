---
title: Members

members:
    - name: "Miroslav Bachinski"
      photo: "https://profile.uib.no/sites/default/files/pictures/picture-404154-1684426021.jpg"
      desc: "I am an Associate Professor in Human-Computer Interaction at the University of Bergen. My research focuses on developing and applying data-driven methods for HCI tasks. Novel interaction methods such as full-body gestural or touch interaction offer immense design space. It is impossible to compare all design alternatives experimentally, and pure intuition can be misleading. I want to improve interaction methods by capturing the entire design space and formalising its performance and ergonomics properties in a simulation which integrates human biomechanics with motor control models. I adopt optical motion capture and biomechanical simulation besides standard performance measurement methods for the HCI experiments to achieve the goal."
      link: "https://bachinskim.github.io/"
    - name: "Frode Guribye"
      photo: "https://profile.uib.no/sites/default/files/pictures/picture-9765-1557248244.jpg"
      desc: "Frode Guribye is a Professor of Information Science focusing on human-computer interaction and the social implications of information and communication technologies. His research spans different application areas such as technology enhanced learning, computing and mental health and mobile journalism. Across these areas he is doing research through design and empirical investigations aiming to critically and constructively understand the potential and limitations of emerging technologies."
      link: "https://www4.uib.no/en/find-employees/Frode.Guribye"
      scholar: "https://scholar.google.com/citations?user=R8yaWs0AAAAJ&hl=en"
    - name: "Morten Fjeld"
      photo: "https://profile.uib.no/sites/default/files/pictures/picture-23358-1625046497.jpg"
      desc: "Morten Fjeld is a professor of Human-Computer Interaction at the University of Bergen (Norway) and Chalmers University of Technology (Sweden). His research activities are situated in the field of Human-Computer Interaction with a focus on tangible and tabletop user computing. In 2005, he founded the t2i Interaction Lab at Chalmers, Sweden. He holds a dual MSc degree in applied mathematics from NTNU (Trondheim, Norway) and ENSIMAG (Grenoble, France), and a PhD from ETH (Zurich, Switzerland). In 2002, Morten Fjeld received the ETH Medal for his PhD titled 'Designing for Tangible Interaction'. In 2011, he was a visiting professor at NUS Singapore, in 2016 and 2017 at Tohoku University, Japan, and in 2019 to 2020 at ETH Zurich. Morten Fjeld also has extensive industrial experience in the areas of fluid mechanics, simulators, and user interface design."
      link: "https://www4.uib.no/en/find-employees/Morten.Fjeld"
    - name: "Pavel Okopnyi"
      photo: "https://profile.uib.no/sites/default/files/pictures/picture-383591-1517235439.jpg"
      desc: "I'm a postdoctoral fellow at UiB, interested in tools, processes and practices for media production, including writing, video editing, music production and other forms of media; complex software, software and game development tools and systems; remote work and automation, including AI-assisted instruments."
      link: "https://www4.uib.no/en/find-employees/Pavel.Okopnyi"
      scholar: "https://scholar.google.com/citations?user=k6DCzvcAAAAJ&hl=en"
    - name: "Oda Elise Nordberg"
      photo: "https://profile.uib.no/sites/default/files/pictures/picture-384606-1603790347.jpg"
      desc: "In my Ph.D. studies, I am exploring the potential of conversational user interfaces (CUIs), such as chatbots and digital assistants, for engaging with news content. I am focused on future-oriented research methods, like co-speculation, to investigate the opportunities and implications of news interaction through conversational interfaces. Beyond my primary research, I have an interest in universal design, privacy, and mental health."
      link: "https://www4.uib.no/en/find-employees/Oda.Elise.Nordberg"
      scholar: "https://scholar.google.com/citations?hl=en&user=slMD2EUAAAAJ"
    - name: "Arngeir Berge"
      photo: "https://www.uib.no/sites/w3.uib.no/files/styles/content_main/public/media/arbe.jpg?itok=XdQf4aXC"
      desc: "I'm doing a PhD on collaboration between humans and artificial intelligence. More specifically, I'm looking at how artificial intelligence can assist call handlers during emergency calls with situational awareness, documentation, decisions, and more."
      link: "https://www4.uib.no/finn-ansatte/Arngeir.Berge"
      scholar: "https://scholar.google.com/citations?user=5promGYAAAAJ&hl=en"
    - name: "Fredrik Håland Jensen"
      photo: "https://www.uib.no/sites/w3.uib.no/files/styles/content_main/public/media/2020-02-06_12.42.00_0.jpg"
      desc: "Fredrik Håland Jensen is a PhD candidate at the University of Bergen. His project is related to TekLab, a network for research, education, and innovation within the media and communication sector. He researches media and interaction design, innovation theory, technology theory, innovation pedagogy, emerging technologies, prototypes, and University-Industry collaboration."
      link: "https://www4.uib.no/finn-ansatte/Fredrik.Håland.Jensen"
---

# Group members

{% if page.members %}
<div class="card-columns">
{% for member in page.members %}

<div class="card">
    <img src="{{member.photo}}" class="card-img-top" alt="{{member.name}}">
    <div class="card-body">
      <h5 class="card-title">{{member.name}}</h5>
      <p class="card-text">{{member.desc}}</p>
      <p class="card-text"><small class="text-muted">
        {% if member.private_link %}<a href="{{member.private_link}}" target="_blank">Personal Website</a>{% endif %}
        {% if member.link %}<a href="{{member.link}}" target="_blank">UiB page</a>{% endif %}
        {% if member.scholar %}<a href="{{member.scholar}}" target="_blank">Google Scholar</a>{% endif %}
        {% if member.linkedin %}<a href="{{member.linkedin}}" target="_blank">Linkdin</a>{% endif %}
        {% if member.twitter %}<a href="{{member.twitter}}" target="_blank">Twitter</a>{% endif %}
      </small></p>
    </div>
</div>

{% endfor %}
</div>
{% endif %}
