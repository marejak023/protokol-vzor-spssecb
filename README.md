# protokol-vzor-spssecb
Předloha vytvořená v LaTeXu pro ty, co nechtějí psát protokoly ve Wordu.

## Jak šablonu použít?

compiler: pdfLaTeX (já osobně používám OverLeaf editor, kde je automaticky nastaven jako výchozí https://www.overleaf.com).
Nepoužívají se zde klasické sections (kapitoly, části) ale je zde struktura

  \fakesection{} (zvýší hodnotu section counteru +1 bez text)
  výchozí hodnota section counter je 0 (0.1 je první kapitola)
  místo \section{} se používají rovnou \subsection{}, struktura může vypadat například takto:
  
    \fakesection{}
    \subsection{Zadání úlohy}
    \par Zde je nějaké zadání úlohy.

    \subsection{Řešení úlohy}
    \par Zde je nějaké řešení úlohy.

    \fakesection{}
    \subsection{Závěr}
    \par Zde je nějaký shrnujicí text.
  
  Tato struktura by poté vypadala následovně:
  
    0.1 Zadání úlohy
    Zde je nějaké zadání úlohy.

    0.2 Řešení úlohy
    Zde je nějaké řešení úlohy.

    1.1 Závěr
    Zde je nějaký shrnujicí text.

Vždy dole ponechte watermark v podobě rámečku s odkazem. Jednotky se snažte psát písmem typu roman (v math modu pomocí \mathrm{}), kvůli mezinárodní konvenci (https://information-technology.web.cern.ch/book/e-publishing-handbooks/preparing-your-contribution/using-latex-writing-your-document-0). Proměnné pak zase stylem písma italic (v math modu výcozí).
Pro grafy používejte pgfplots a pro schémata obvodů circuitikz. Vždy používejte nejnovější verzi.

## changelog:

* v0.1 - První vzor
  
