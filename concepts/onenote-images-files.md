---
title: Adicione imagens, vídeos e arquivos às páginas do OneNote usando a API do OneNote
description: Use os elementos img, object e iframe para adicionar imagens, vídeos e arquivos à página do OneNote quando você criar ou atualizar a página.
author: jewan-microsoft
ms.localizationpriority: high
ms.prod: onenote
ms.openlocfilehash: a9edfd96275e2ce9516fd937ad02e721aa526462
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444387"
---
# <a name="add-images-videos-and-files-to-onenote-pages"></a>Adicionar imagens, vídeos e arquivos a páginas do OneNote

**Aplica-se a** Notebooks de consumidores no OneDrive | Notebooks corporativos no Microsoft 365

Você pode usar os elementos **img**, **object** e **iframe** para adicionar imagens, vídeos e arquivos à página do OneNote quando você [criar](onenote-create-page.md) ou [atualizar](onenote-update-page.md) a página. 

- Use **img** para renderizar uma imagem na página.
- Use **iframe** para inserir um vídeo na página.
- Use **object** para adicionar um anexo de arquivo na página.


<a name="images"></a>

## <a name="adding-images"></a>Adicionar imagens

Imagens podem ser adicionadas por referência de URL ou enviando dados brutos. Os seguintes métodos de adição de imagens, logotipos e fotos para páginas do OneNote são compatíveis com o Microsoft Graph. 

[Adicionar uma imagem pública da Web](#add-a-public-image-from-the-web)

Use `img` com `src="https://image-url"` e especifique a URL de uma imagem acessível ao público. Renderiza a imagem na página do OneNote.

[Adicionar uma imagem usando dados binários](#add-an-image-using-binary-data)

Use `img` com `src="name:image-block-name"` e envie o arquivo de imagem em uma parte de dados de uma solicitação de várias partes. Renderiza a imagem na página do OneNote.

[Adicionar um instantâneo de página da Web](#add-a-webpage-snapshot)

Use `img` com `data-render-src="https://webpage-url"` e especifique a URL de uma página da Web. Renderiza um instantâneo da página da Web inteira na página do OneNote.

[Adicionar uma imagem renderizada de HTML](#add-an-image-rendered-from-html)

Use `img` com `data-render-src="name:html-block-name"` e envie HTML na parte de dados de uma solicitação de várias partes. Renderiza o HTML como uma imagem na página do OneNote.

[Adicionar imagens de conteúdos de arquivo PDF](#add-images-of-pdf-file-contents)

Use `<img data-render-src="name:part-name" />` e envie o arquivo PDF na parte de dados de uma solicitação de várias partes. Renderiza cada página do PDF como uma imagem separada na página do OneNote.

[Adicionar um arquivo de imagem como um anexo de arquivo](#add-an-image-file-as-an-attachment)

Use `object` com `data="name:file-block-name" data-attachment="file-name.file-ext" type="media-type"` e envie um arquivo de imagem em uma parte de dados de uma solicitação de várias partes. Adiciona um anexo de arquivo à página do OneNote e exibe um ícone de arquivo.

> [!NOTE]
> Para inserir imagens em uma página do OneNote, primeiro envie uma [solicitação GET para o conteúdo da página](onenote-get-content.md#page-html-content). Isso retornará as URLs para recursos de imagem na página. Em seguida, separe as [solicitações GET dos recursos de imagem](onenote-get-content.md#image-or-other-file-resource).


#### <a name="image-attributes"></a>Atributos de imagem 

Um elemento **img** pode incluir opcionalmente atributos **alt**, **height** e **width** e os atributos de estilo **max-width** e **max-height**.

#### <a name="image-media-types"></a>Tipos de mídia de imagem

O Microsoft Graph é compatível com os tipos de imagem TIFF, PNG, GIF, JPEG e BMP. Para capturar uma imagem que usa um formato diferente que você não quer converter, [envie dados binários](#add-an-image-using-binary-data) em uma solicitação de várias partes. Não é necessário usar Base64 ou codificar os dados binários que você enviar.

> [!NOTE]
> A API detecta o tipo de imagem de entrada e o retorna como o atributo **data-fullres-src-type** no [HTML de saída](onenote-input-output-html.md#output-html). A API também retorna o tipo de imagem da imagem otimizada em **data-src-type**.
 
Ver [limitações](#size-limitations-for-post-pages-requests) que se aplicam ao criar páginas que contém mídia.


<a name="image-img-url-src"></a>

### <a name="add-a-public-image-from-the-web"></a>Adicionar uma imagem pública da Web

No HTML de entrada da sua solicitação, inclua `<img src="https://..." />` e especifique a URL de uma imagem publicamente acessível para o atributo **src**.

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Public URL</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays an image from the web.</p>
    <img src="https://..." width="300"/>
  </body>
</html>

--MyAppPartBoundary--  
```

<a name="image-img-binary-src"></a>

### <a name="add-an-image-using-binary-data"></a>Adicionar uma imagem usando dados binários

No HTML de entrada da parte de **Apresentação** da sua solicitação, inclua `<img src="name:part-name" />`, em que *part-name* é o identificador exclusivo para a parte de dados na sua [solicitação de várias partes](onenote-create-page.md#example-request) que contém os dados de imagem binária. Basta enviar dados binários, não use Base64 ou codifique.

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Image binary data</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays the uploaded image.</p>
    <img src="name:image-block-name" alt="a cool image" width="500"/>
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="MyAppPictureId"
Content-Type: image/jpeg

... image binary data ...

--MyAppPartBoundary--  
```


<a name="image-img-url-data-render-src"></a>

### <a name="add-a-webpage-snapshot"></a>Adicionar um instantâneo de página da Web

Você pode usar o Microsoft Graph para fazer instantâneos inteiros de páginas da Web e inseri-los em novas páginas. Esse método é útil para arquivar páginas da Web ou capturar páginas da Web complexas que possuem recursos não compatíveis com o OneNote (como algumas CSS).  

No HTML de entrada da sua solicitação, inclua `<img src="https://..." />` e especifique a URL de uma página da Web que você quer inserir para o atributo **src**.

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Webpage capture</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays an image of the webpage.</p>
    <img data-render-src="https://www.onenote.com" width="200"/>
  </body>
</html>

--MyAppPartBoundary--  
```


<a name="image-img-binary-data-render-src"></a>

### <a name="add-an-image-rendered-from-html"></a>Adicionar uma imagem renderizada de HTML

Quando você passar o HTML como um bloco de dados, certifique-se de que não haja conteúdo ativo que exija credenciais de usuário ou um plug-in de navegador pré-carregado. O mecanismo que o Microsoft Graph usa para renderizar a página HTML em uma imagem não tem a capacidade de fazer logon de um usuário e não inclui plug-ins como Adobe Flash, Apple QuickTime entre outros. Isso também significa que o conteúdo carregado dinamicamente, que pode vir com um script AJAX, não será exibido se a obtenção dos dados exigir credenciais de logon do usuário ou cookies.

No HTML de entrada da parte de **Apresentação** da sua solicitação, inclua `<img data-render-src="name:part-name" />`, em que *part-name* é o identificador exclusivo para a parte de dados na sua [solicitação de várias partes](onenote-create-page.md#example-request) que contém o HTML.


```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: HTML block</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays the block of HTML as an image.</p>
    <img data-render-src="name:html-block-name" alt="a cool image" width="500"/>
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="html-block-name"
Content-Type: text/html

<html>
<body>
<h1>This HTML will render as an image</h1>
<p><b>Don't</b> try to embed another <i>data-render-src</i> type-image inside the HTML part--
it won't work. Instead, use URL-based real images like this:</p>
<img src="https://cdn.onenote.net/1664161560_Images/OneNote.ico" />
</body>
</html>

--MyAppPartBoundary--  
```


<a name="image-object"></a>

### <a name="add-an-image-file-as-an-attachment"></a>Adicionar um arquivo de imagem como um anexo

No HTML de entrada da parte de **Apresentação** da sua solicitação, inclua `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, em que *part-name* é o identificador exclusivo para a parte de dados na sua [solicitação de várias partes](onenote-create-page.md#example-request) que contém os dados de imagem binária. Basta enviar dados binários, não use Base64 ou codifique.

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Binary image data as file attachment</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page contains the image as a file attachment.</p>
    <object data-attachment="image-file.jpg" data="name:image-block-name" type="image/jpeg" />
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="logo1-file"
Content-Type: image/jpeg

... binary file data ...

--MyAppPartBoundary--
```

Saiba mais sobre [tipos de mídia de arquivos](#file-media-types).



<a name="adding-videos"></a>

## <a name="adding-videos"></a>Adicionar vídeos

Você pode inserir vídeos em páginas do OneNote usando `<iframe data-original-src="https://..." />` no HTML de entrada. 

### <a name="supported-video-sites"></a>Sites de vídeo compatíveis

- Dailymotion
- Office Mix
- Sway
- Sketchfab
- TED
- YouTube
- Vimeo
- Vine

### <a name="iframe-attributes"></a>atributos de iframe

#### <a name="data-original-src"></a>data-original-src

Necessário. A URL do vídeo.

Exemplo: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`

#### <a name="width"></a>width

Opcional. A largura do iframe que contém o vídeo. O padrão é 480.

Exemplo: `width="300"`

#### <a name="height"></a>height

Opcional. A altura do iframe que contém o vídeo. O padrão é 360.

Exemplo: `height="300"`

### <a name="example"></a>Exemplo

No HTML de entrada da sua solicitação, inclua `<iframe data-original-src="https://..." />` e especifique a URL do vídeo para o atributo **data-original-src**.

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
    <head>
        <title>A page with an embedded video</title>
    </head>
    <body>
        <iframe data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8" width="340" height="280"/>
    </body>
</html>

--MyAppPartBoundary--
```


<a name="adding-files"></a>

## <a name="adding-files"></a>Adicionar arquivos

Você pode adicionar anexos de arquivo a páginas do OneNote usando um elemento **object** de HTML de entrada. Se você estiver adicionando um arquivo PDF, você pode usar um elemento de **img** para renderizar as páginas de PDF como imagens. 

[Adicionar um anexo de arquivo](#add-a-file-attachment)

Use `<object .../>` e envie o arquivo na parte de dados de uma solicitação de várias partes. Adiciona um anexo de arquivo que exibe um ícone de arquivo na página do OneNote.

[Adicionar imagens de conteúdos de arquivo PDF](#add-images-of-pdf-file-contents)

Use `<img data-render-src="name:part-name" />` e envie um arquivo PDF na parte de dados de uma solicitação de várias partes. Renderiza cada página do PDF como uma imagem separada na página do OneNote.

#### <a name="file-attributes"></a>Atributos de arquivo

O elemento **object** requer os seguintes atributos.

**data-attachment**

O nome e a extensão do arquivo para exibir na página do OneNote.

Exemplo: `data-attachment="filename.docx"`

**data**

O nome da parte do corpo na solicitação de várias partes que contém os dados de arquivo binário. O Microsoft Graph não é compatível com a passagem de uma referência de URL aqui.

Exemplo: `data="name:part-name"`

**type**

O tipo de mídia de arquivo, usado para determinar o ícone de arquivo a ser usado na página e qual aplicativo é iniciado quando o usuário ativa o arquivo no dispositivo a partir do OneNote.

Exemplo: `type="application/pdf"`


<a name="file-media-types"></a>

#### <a name="file-media-types"></a>Tipos de mídia de arquivo  

O Microsoft Graph usa o ícone de tipos de arquivo predefinido para arquivos anexos ou um ícone genérico quando a API não reconhece o tipo de arquivo. A tabela a seguir mostra alguns tipos de arquivos comuns reconhecidos pela API.

- application/pdf  
- application/vnd.openxmlformats-officedocument.wordprocessingml.document  
- application/vnd.openxmlformats-officedocument.presentationml.presentation
- application/vnd.openxmlformats-officedocument.spreadsheetml.sheet
- image/png
- image/jpeg
- image/gif
- audio/wav
- video/mp4
- application/msword
- application/mspowerpoint
- application/excel

Ver [limitações](#size-limitations-for-post-pages-requests) que se aplicam ao criar páginas que contém mídia.


<a name="file-object"></a>

### <a name="add-a-file-attachment"></a>Adicionar um anexo de arquivo

No HTML de entrada da parte de **Apresentação** da sua solicitação, inclua `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, em que *part-name* é o identificador exclusivo para a parte de dados na sua [solicitação de várias partes](onenote-create-page.md#example-request) que contém os dados de arquivo binário. Basta enviar dados binários, não use Base64 ou codifique.

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image file attachment</title>
  </head>
  <body>
    <p>This is an image file attachment.</p>
    <object data-attachment="Logo.jpg" data="name:logo1-file" type="image/jpeg" />
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="logo1-file"
Content-Type: image/jpeg

... binary file data ...

--MyAppPartBoundary--
```


<a name="file-binary-data-render-src"></a>

### <a name="add-images-of-pdf-file-contents"></a>Adicionar imagens de conteúdos de arquivo PDF

No HTML de entrada da parte de **Apresentação** da sua solicitação, inclua `<img data-render-src="name:part-name" ... />`, em que *part-name* é o identificador exclusivo para a parte de dados na sua [solicitação de várias partes](onenote-create-page.md#example-request) que contém os dados de arquivo binário. Basta enviar dados binários, não use Base64 ou codifique.

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with images of the pages of a PDF file</title>
  </head>
  <body>
    <p>The pages of this PDF file render as images.</p>
    <img data-render-src="name:file-part" alt="PDF file as images" width="500"/>
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="file-part"
Content-Type: application/pdf

... binary file data ...

--MyAppPartBoundary--  
```


<a name="size-limits"></a>

## <a name="size-limitations-for-post-pages-requests"></a>Limitações de tamanho para solicitações de páginas de POSTAGEM

Ao enviar a imagem e arquivo de dados, esteja ciente dessas limitações: <!--TODO: check these-->

- A API REST do Microsoft Graph tem um limite de solicitação de 4 MB. Qualquer item maior que isso falhará com a mensagem de erro "solicitação muito grande (413)". 

- O limite de solicitação da subjacentes API REST do OneNote é maior, mas não pode ser acessada usando a API do Microsoft Graph. 
  - O limite de tamanho da POSTAGEM total é de aproximadamente 70 MB, incluindo imagens, arquivos e outros dados. O limite real é afetado pela codificação downstream, portanto, não há um limite de número de bytes fixo. As solicitações que excederem o limite podem gerar resultados não confiáveis.
  - O limite de cada parte de dados é de 25 MB, incluindo os cabeçalhos das partes. Partes de dados que excedem o limite são rejeitadas pelo Microsoft Graph. 

- O número máximo de imagens por página é 150. Ao usar o atributo `src="https://..."`, a API ignora rótulos **img** que ultrapassam o limite.

- O número máximo de partes de dados é 6 por POSTAGEM, incluindo a parte obrigatória **Apresentação**.

- Cada pedido pode conter até cinco elementos **img** que usam **data-render-src** um elemento **object** que usa **data-render-src**. Outras referências de imagem e arquivo são ignoradas.

- O número máximo de imagens em uma POSTAGEM única é 30, não importa qual o método usado para enviá-las para a API. Imagens adicionais são ignoradas. Se quiser capturar uma página da Web que contém muitas imagens, considere [capturar toda a página como um instantâneo](#add-a-webpage-snapshot).


## <a name="when-to-use-html-versus-data-render-src"></a>Quando usar HTML ou data-render-src 

Para decidir entre colocar HTML diretamente na página do OneNote em vez de usar o atributo **data-render-src**, considere o seguinte:

- Provavelmente, a melhor maneira de enviar HTML complexo para o mecanismo de renderização é por meio de **data-render-src**, em vez de tentar modificar o HTML para caber naquilo que o Microsoft Graph aceita. Isso também ocorre quando o HTML inclui rótulos sem suporte.

- Provavelmente, a melhor maneira de fazer a renderização de página com precisão para preservar o layout e a aparência da página é com o mecanismo de renderização por meio do **data-render-src**.

- Geralmente, a melhor maneira de acrescentar texto diretamente editável é inserindo HTML diretamente na página. As imagens renderizadas são examinadas por um sistema de reconhecimento óptico de caracteres (OCR), mas não é a mesma coisa.

- Normalmente, a melhor maneira de fazer um instantâneo no tempo para fins de histórico ou arquivamento é com o método **data-render-src**.

- O **data-render-src** realmente se destaca pela funcionalidade de marcação do design da página da Web para revisões. Com as funcionalidades de escrita à tinta do OneNote, é possível desenhar na imagem para indicar alterações ou destacar áreas importantes. Com a página da Web como uma imagem fica muito mais fácil.

- As imagens muito grandes ou as imagens nos formatos que o OneNote não aceita diretamente podem, às vezes, ser transformadas em miniaturas e convertidas com o atributo **data-render-src** mais facilmente do que se isso for feito em seu próprio código. Mesmo que a imagem também esteja disponível online, inserir os dados em sua POSTAGEM pode às vezes disponibilizar antes a página selecionada para os usuários do OneNote, reduzindo o número total de procedimentos necessários para criar a página do OneNote.

Às vezes, a melhor maneira para determinar qual método funciona melhor para os usuários é experimentar as duas formas conforme você desenvolve seu aplicativo.


<a name="permissions"></a>

## <a name="permissions"></a>Permissões

Para criar ou atualizar páginas do OneNote, solicite permissões apropriadas. Escolha o nível mais baixo que seu aplicativo precisa para realizar o trabalho.

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

- [Integrar com o OneNote](integrate-with-onenote.md)
- [Blog de desenvolvedor do OneNote](https://go.microsoft.com/fwlink/?LinkID=390183)
- [Perguntas de desenvolvimento do OneNote no Microsoft Q&A](/answers/topics/microsoft-graph-notes.html)
- [Repositórios do OneNote no GitHub](https://go.microsoft.com/fwlink/?LinkID=390178)
