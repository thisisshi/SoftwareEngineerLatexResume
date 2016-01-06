# Software Engineer Latex Resume
A Resume in LaTeX!

![Preview](http://i.imgur.com/kehekD1.png)

Resumes are boring. They're hard to design well because they're so utilitarian. 

This LaTeX project is a fork of [Awesome-CV](https://github.com/posquit0/Awesome-CV). I've cut away a lot of the CV-ish features from the default resume, but they can be easily added back. At its core the resume includes sections for: Experience, Other Projects, Education, and Skills. From that, a large amount of use cases should be covered. 

To start using this template, begin by editing the `resume.tex` file in the root folder. Fill in your own name, location, phone number, etc. You can center the header section by uncommenting the `\begin{center}` and `\end{center}` lines in the `awesome-cv.cls` file in the `\makecvheader` section.

To change the accent color, use: `\colorlet{<some-color>}{<some-color>}` where `<some-color>` can be `awesome`, `white`, `black`, `darkgray`, `gray`, `lightgray`, `green`, `orange`, `purple`, `red`, `blue`, `darktext`, `darkgray`, `darktext`, `lighttext`, `awesome-emerald`, `awesome-skyblue`, `awesome-red`, `awesome-pink`, `awesome-orange`, `awesome-nephritis`, `awesome-concrete`, `awesome-darknight`. You can add additoinal colors in `awesome-cv.cls` using `\definecolor`.

From there, fill in the rest of sections accordingly. A `\cvsection` is called by using the following:

```
\cvsection{<Section Name>}
  \begin{cventries}
    \cventry
    {<Title>}
    {<Section Header>}
    {<Location>}
    {<Date>}
    {
      \begin{cvitems}
        \item{<bullet point 1>}
        \item{<bullet point 2>}
      \end{cvitems}
    }
  \end{cventries}
```

Skills are a bit different:
```
\cvsection{Skills}
\begin{cvskills}
    \cvskill{Languages}{Java, C, Ruby, Javascript, C\#, Visual Basic}
    \cvskill{Frameworks}{Ruby on Rails, Bootstrap, Skeleton, Flexbox, ASP.NET}
    \cvskill{Database}{MSSQL, MySQL, PostgreSQL}
    \cvskill{Markup}{HTML, XML, Markdown, LaTeX}
    \cvskill{Design}{Adobe Photoshop, Adobe InDesign, Adobe Illustrator}
    \cvskill{Other}{English, Chinese (conversational), Spanish (limited)}
\end{cvskills}
```

That's basically all you need to know to get started. More documentation can be found at [Awesome-CV](https://github.com/posquit0/Awesome-CV)'s repo
