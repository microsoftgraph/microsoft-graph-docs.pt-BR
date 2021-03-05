---
title: Criar elementos posicionados absolutos nas páginas do OneNote
description: O corpo de uma página do OneNote pode conter vários elementos filhos diretos `div`, `img` e `object` que podem ser posicionados de forma independente na página.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: e21ad3fb97b807bc91ecf6a993483f3bb83c82b8
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472836"
---
# <a name="create-absolute-positioned-elements-in-onenote-pages"></a>Criar elementos posicionados absolutos nas páginas do OneNote

O corpo de uma página do OneNote pode conter vários elementos filhos diretos `div`, `img` e `object` que podem ser posicionados de forma independente na página.

<a name="attributes"></a>

## <a name="attributes-and-positioning-behavior"></a>Atributos e comportamento de posicionamento

Use os atributos `data-absolute-enabled` e [`style`](#supported-css-style-attributes) para criar elementos posicionados absolutos em uma página, da seguinte maneira:

- O elemento do corpo deve especificar `data-absolute-enabled="true"`. Se omitido ou definido como `false`, todo o conteúdo do corpo será processado dentro de um div posicionado absoluto `_default` que a API cria e todas as configurações de posição serão ignoradas.

- Apenas os elementos `div`, `img` e `object` podem incluir elementos posicionados absolutos. 

- Os elementos posicionados absolutos devem especificar `style="position:absolute"`.

- Os elementos posicionados absolutos devem ser filhos diretos do elemento `body`. Quaisquer filhos diretos do corpo que não sejam elementos posicionados absolutos `div`, `img` ou `object` serão processados como conteúdo estático no div posicionado absoluto `_default`.

- Os elementos posicionados absolutos são colocados nas coordenadas especificadas superiores e esquerdas, relativas à posição inicial 0:0 no canto superior esquerdo da página, acima da área de título.

- Quando um elemento com posicionamento absoluto omite coordenada esquerda ou superior, a coordenada ausente está definida com o valor padrão: `top:120px` ou `left:48px`. Essas coordenadas padrão especificam uma posição abaixo da área de título. Lembre-se de que omitir coordenadas pode resultar em elementos empilhados.

- Os elementos posicionados absolutos não podem ser aninhados, nem conter elementos posicionados. A API ignora as configurações de posição especificadas em elementos aninhados dentro do div posicionado absoluto, processa o conteúdo aninhado dentro do div pai posicionado absoluto e retorna um aviso na propriedade **api.diagnostics** na resposta.


### <a name="example"></a>Exemplo

O exemplo a seguir contém um filho `p` direto, um div posicionado absoluto e um div posicionado não absoluto.

#### <a name="input-html"></a>HTML de entrada  

   ```html 
   <body data-absolute-enabled="true">
       <p>This content will appear in the _default div.</p>
       <div style="position:absolute;top:175px;left:100px" data-id="div1">
         <p>This content will appear in an absolute positioned div.</p>
       </div>
       <div>
           <p>This content will also appear in the _default div.</p>
       </div>
   </body>
   ```

A API processa o div posicionado não absoluto no div padrão. Observe que as marcas aninhadas `<div>` são descartadas porque não definem informações semânticas (como `data-id`).

#### <a name="output-html"></a>HTML de saída 

   ```html 
   <body data-absolute-enabled="true" style="font-family:Calibri;font-size:11pt">
       <div data-id="_default" style="position:absolute;left:48px;top:120px;width:624px">
           <p>This content will appear in the _default div.</p>
           <p>This content will also appear in the _default div.</p>
       </div>
       <div data-id="div1" style="position:absolute;left:99px;top:174px;width:624px">
           <p>This content will appear in an absolute positioned div.</p>
       </div>
   </body>
   ```

### <a name="example"></a>Exemplo

O exemplo a seguir cria uma página que contém um div posicionado absoluto e uma imagem posicionada absoluta.


#### <a name="input-html"></a>HTML de entrada  

```html 
<html>
    <head>
        <title>Page Title</title>
    </head>
    <body data-absolute-enabled="true">
        <div style="position:absolute;width:280px;top:120px;left:68px">
            <p>Some text</p>
            <img style="width:120px" src="https://officeimg.vo.msecnd.net/files/018/949/ZA103278226.png" />
            <div>
                <p>More text inside a regular, nested div</p>
            </div>
        </div>
        <img style="position:absolute;width:360px;top:350px;left:300px" src="https://officeimg.vo.msecnd.net/files/018/949/ZA103278226.png" />
    </body>
</html>
```
 
A API do OneNote avalia o HTML de entrada e preserva todo o conteúdo semântico e qualquer informação estrutural compatível com o OneNote. A página resultante processa conforme mostrado na imagem a seguir, mas sem as bordas visíveis do div e da imagem. 

![A página resultante com o div posicionado absoluto e a imagem](images/abs-pos.png)

Observe as alterações no div aninhado não contribuidor do HTML de entrada. A API preserva o conteúdo do div, mas descarta as marcas `<div>` porque o div não define informações semânticas (como `data-id`).

Saiba mais sobre como a API do OneNote lida com HTML de entrada e saída em [HTML de entrada e de saída para páginas do OneNote](onenote-input-output-html.md).

<a name="style-attributes"></a>

## <a name="supported-css-style-attributes"></a>Atributos de estilos CSS compatíveis

Todos os elementos posicionados absolutos podem especificar as posições superiores e esquerdas. Divs e imagens podem especificar a largura e as imagens também podem especificar a altura. Por exemplo:

```html
<img style="position:absolute;top:140px;left:95px;width:480px;height:665px" src="..." />
```

| Atributo | Elemento compatível | Descrição |  
|:------|:------|:------|  
| top | div, img, object | A coordenada do eixo Y da borda superior do elemento, somente em pixels. O padrão é 120 pixels.<br/><br/>Exemplo: `top:140px` |  
| left |  div, img, object  | A coordenada do eixo X da borda esquerda do elemento, somente em pixels. O padrão é 48 pixels.<br/><br/>Exemplo: `left:95px` |  
| width |  div, img  | A largura do elemento, somente em pixels.<br/><br/>Exemplo: `width:480px` |  
| height | img | A altura do elemento, somente em pixels. Para divs, a altura é calculada no tempo de execução e qualquer valor de altura especificado será ignorado.<br/><br/>Exemplo: `height:665px` |  
 
Outros atributos de posição, como `z-index`, são ignorados. As imagens posicionadas absolutas podem usar o atributo `data-render-src` ou `src`.


<a name="request-response-info"></a>

## <a name="response-information"></a>Informações de resposta

A API do OneNote retorna as seguintes informações na resposta.

| Dados de resposta | Descrição |  
|:------|:------|  
| Código de êxito | Um código de status HTTP 201 para uma solicitação POST bem-sucedida e um código de status HTTP 204 para uma solicitação PATCH bem-sucedida. |  
| Erros | Leia [Códigos de erro para APIs do OneNote no Microsoft Graph](onenote-error-codes.md) para saber mais sobre erros do OneNote que poderão ser retornados pelo Microsoft Graph. |  
  


<a name="permissions"></a>

## <a name="permissions"></a>Permissões

Para criar ou atualizar páginas do OneNote, solicite permissões apropriadas. Escolha o nível mais baixo de permissões que seu aplicativo precisa para realizar o trabalho.

#### <a name="permissions-for-post-pages"></a>Permissões para páginas POST 

- Notes.Create
- Notes.ReadWrite
- Notes.ReadWrite.All  


#### <a name="permissions-for-patch-pages"></a>Permissões para páginas PATCH 

- Notes.ReadWrite
- Notes.ReadWrite.All

Para saber mais sobre escopos de permissão e como eles funcionam, confira [Escopos de permissão do OneNote](permissions-reference.md#notes-permissions).


<a name="see-also"></a>

## <a name="see-also"></a>Confira também

- [Criar páginas do OneNote](onenote-create-page.md)
- [Atualizar o conteúdo da página do OneNote](onenote-update-page.md)
- [Integrar com o OneNote](integrate-with-onenote.md)
- [Blog de desenvolvedor do OneNote](https://go.microsoft.com/fwlink/?LinkID=390183)
- [Perguntas sobre desenvolvimento do OneNote no Microsoft Q&A](https://docs.microsoft.com/answers/topics/microsoft-graph-notes.html)
- [Repositórios do OneNote no GitHub](https://go.microsoft.com/fwlink/?LinkID=390178)  

