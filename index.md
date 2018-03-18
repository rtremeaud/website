## My r code / graphics



### graphic I

[![ IIII ](https://rtremeaud.github.io/website/Capture d’écran 2018-03-12 à 00.24.34.png)](https://rtremeaud.github.io/website/graphics1.html)

```markdown
library("highcharter")

hchart(dd, "scatter", 
  hcaes(x = Review.Date, 
        y = Rating,   
        group = Company.Location))
```

### graphic II

[![ IIII ](https://rtremeaud.github.io/website/Capture d’écran 2018-03-18 à 17.23.33.png)](https://rtremeaud.github.io/website/graphic2.html)

```markdown
library("highcharter")

highchart() %>% hc_title(text = "Evolution des coûts MNT") %>% 
  hc_subtitle(text = "Source: OFS") %>% hc_yAxis(title = list(text = "en %")) %>% 
  hc_xAxis(title = list(text = "année")) %>% hc_xAxis(categories = dd$X) %>% 
  hc_add_series(name = "Coût.du.système.de.santé.Valeur.nominale..en.mio.de.francs", data = dd$Coût.du.système.de.santé.Valeur.nominale..en.mio.de.francs) %>% 
  hc_add_series(name = "PIB.Valeur.nominale..en.mio.de.francs", data = dd$PIB.Valeur.nominale..en.mio.de.francs)
}
```
### graphic III
Différentes variations des coûts de santé en lien avec le PIB et la population
[![ IIII ](https://rtremeaud.github.io/website/visualize.png)]
### Jekyll Themes


