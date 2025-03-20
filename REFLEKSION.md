# Kort refleksion

1. Reflekter kort men fagligt over din løsning med henblik på udfordringerne og successerne ved opgaven.

1.a Jeg startede med at danne et overblik over alle Custom Proporties med de mange variabler. Dette hjalp med at kunne mindske koden på alle mine pages og components. Heri havde jeg samlet alle farver, fonte, text-størrelser, line-heigt osv. så de basale ting ikke skulle gentages. Disse Custom Proporties var klart en successfyldt del af opgaven, som formindskede en del kode for mig.

1.b En udfordring med opgaven var at få layout med en samlet margin / screen size til at fungere funktionelt. Denne udfordring blev til dels løst med en Wrapper layout, hvori jeg Wrappede alle mine components, så havde et ens layout og dermed ville flugtes med hinanden. En udfordring i denne løsning var, at få udvalgte components til IKKE at have samme layout...

2. Fremhæv specifikke kodestumper, der illustrerer brugen af forskellige teknikker og principper (gerne fra undervisningen).

2.a Her ses en specifik kodestump, der illustrerer brugen af Custom Proporties:

--yellow-dark: #ffcc4a;
--yellow-light: #ffe5a2;

--green-primary: #4eaf4e;
--white-primary: #ffffff;
--black-primary: #181818;

--black-background: rgba(27, 27, 27, 0.91);
--grey-light: #f5f5f5;
--grey-dark: #ebebeb;

2.b Her ses en specifik kodestump fra "Layout.astro" der illustrerer brugen af CSS-Selector. Her benyttes > :not(&)

footer {
grid-column: 1 / -1;
display: grid;
grid-template-columns: subgrid; > :not(&) {
grid-column: content;
}
}

3. Forklar, hvordan du har organiseret din CSS; hvornår er det globalt, og hvornår er det komponent-specifikt.
