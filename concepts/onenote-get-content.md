---
title: Obter a estrutura e o conteúdo do OneNote com o Microsoft Graph
description: " Blocos de anotações empresariais no Microsoft 365"
author: jewan-microsoft
ms.localizationpriority: high
ms.prod: onenote
ms.openlocfilehash: 13a017ac30de19f978c21b1da549efefac985ae7
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64586867"
---
# <a name="get-onenote-content-and-structure-with-microsoft-graph"></a>Obter a estrutura e o conteúdo do OneNote com o Microsoft Graph

**Aplica-se a**: Blocos de anotações de consumidor no OneDrive | Blocos de anotações empresariais no Microsoft 365

Para obter a estrutura e o conteúdo do OneNote, você envia uma solicitação GET para o ponto de extremidade de destino. Por exemplo:

`GET ../onenote/pages/{id}`

Se a solicitação for bem-sucedida, o Microsoft Graph retornará um código de status HTTP `200 OK` e as entidades ou o conteúdo que você solicitou. As entidades do OneNote são retornadas como objetos JSON que estão em conformidade com a especificação OData versão 4.0.

Usando as opções de cadeia de caracteres de consulta, você pode filtrar as consultas e melhorar o desempenho.

> [!NOTE]
> Se você estiver criando uma solução que dê suporte a um dos cenários a seguir, atingirá as limitações da API do OneNote:
> - Seções do OneNote de Backup/restauração
> - Fazer backup/restaurar blocos de anotações do OneNote
> 
> Para operações de backup e restauração, consulte [Práticas recomendadas para descobrir arquivos e detectar alterações em escala](/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online).

<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a>Construir a URI de solicitação

Para construir a URI de solicitação, comece com a URL raiz do serviço:

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

Em seguida, acrescente o ponto de extremidade do recurso que você deseja recuperar. (Os [caminhos recurso](#resource-paths-for-get-requests) são mostrados na próxima seção).

Sua URI de solicitação completa parecerá com um dos seguintes exemplos:

- `https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/sections`
- `https://graph.microsoft.com/v1.0/me/onenote/notes/pages`
- `https://graph.microsoft.com/v1.0/me/onenote/pages?select=title,self`

> **Observação:** saiba mais sobre a [URL raiz de serviço](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).

<a name="resource-paths"></a>

## <a name="resource-paths-for-get-requests"></a>Caminhos de recursos para solicitações GET

Use os caminhos de recursos a seguir para obter páginas, seções, grupos de seções, blocos de anotações e recursos de arquivo ou imagem.

- [Coleção de páginas](#page-collection)
- [Entidade Page](#page-entity)
- [Visualização de página](#page-preview)
- [Conteúdo HTML da página](#page-html-content)
- [Coleção Section](#section-collection)
- [Entidade Section](#section-entity)
- [Coleção SectionGroup](#sectiongroup-collection)
- [Entidade SectionGroup](#sectiongroup-entity)
- [Coleção de blocos de anotações](#notebook-collection)
- [Entidade Notebook](#notebook-entity)
- [Imagem ou outro recurso de arquivo](#image-or-other-file-resource)

<a name="get-pages"></a>

### <a name="page-collection"></a>Coleção de páginas

Obter páginas (metadados) em todos os blocos de anotações.

`../pages[?filter,orderby,select,expand,top,skip,search,count]`

<br/>

Obter páginas (metadados) de uma seção específica.

`../sections/{section-id}/pages[?filter,orderby,select,expand,top,skip,search,count,pagelevel]`

<br/>
 
A opção de cadeia de caracteres de consulta `search` está disponível somente para blocos de anotações de consumidor.

A ordem de classificação padrão é `lastModifiedTime desc`.

A consulta padrão expande a seção pai e seleciona as propriedades `id`, `name` e `self` da seção.

Por padrão, somente as primeiras 20 entradas são retornadas para solicitações *GET pages*. Solicitações que não especificam uma opção **principal** de sequência de caracteres de consulta retornam um link `@odata.nextLink` na resposta que você pode usar para obter as próximas 20 entradas.

Para a coleção de páginas em uma seção, use **pagelevel** para retornar o nível de recuo de páginas e sua ordem dentro da seção. 

#### <a name="example"></a>Exemplo

`GET ../sections/{section-id}/pages?pagelevel=true`



<a name="get-page"></a> 

### <a name="page-entity"></a>Entidade Page

Obtenha os metadados de uma página específica. 

`../pages/{page-id}[?select,expand,pagelevel]` 

<br/>

As páginas podem expandir as propriedades **parentNotebook** e **parentSection**.

A consulta padrão expande a seção pai e seleciona as propriedades `id`, `name` e `self` da seção.

Use **pagelevel** para retornar o nível de recuo da página e sua ordem dentro da seção pai. 

#### <a name="example"></a>Exemplo

`GET ../pages/{page-id}?pagelevel=true`



<a name="get-page-preview"></a> 

### <a name="page-preview"></a>Visualização de página

Obtenha conteúdo de visualização de texto e imagem de uma página.

`../pages/{page-id}/preview`

<br/>


A resposta JSON contém conteúdo de visualização que você pode usar para ajudar os usuários a identificar o que está na página.

```json
{
  "@odata.context":"https://www.onenote.com/api/v1.0/$metadata#Microsoft.OneNote.Api.PagePreview",
  "previewText":"text-snippet",
  "links":{
    "previewImageUrl":{
      "href":"https://www.onenote.com/api/v1.0/resources/{id}/content?publicAuth=true&mimeType=image/png"
    }
  }
}
```

A propriedade **previewText** contém um trecho de texto proveniente da página. O Microsoft Graph retorna frases completas, no máximo de 300 caracteres. 

Se a página tiver uma imagem que possa ser usada para criar uma interface do usuário de visualização, a propriedade **href** no objeto **previewImageUrl** conterá um link para um recurso de [imagem pública](#image-or-other-file-resource). Você pode usar este link em HTML. Caso contrário, **href** retorna nulo.

#### <a name="example"></a>Exemplo 

`<img src="https://www.onenote.com/api/v1.0/resources/{id}/content?publicAuth=true&mimeType=image/png" />`


<a name="get-page-content"></a> 

### <a name="page-html-content"></a>Conteúdo HTML da página

Obtenha o conteúdo HTML da página.

`../pages/{page-id}/content[?includeIDs]`

(*saiba mais sobre [conteúdo HTML retornado](onenote-input-output-html.md)*) 

<br/>

Use a opção de cadeia de caracteres de consulta **includeIDs=true** para obter IDs gerados usados para [atualizar a página](onenote-update-page.md).



<a name="get-sections"></a>

### <a name="section-collection"></a>Conjunto da seção

Obtenha todas as seções de todos os blocos de anotações de propriedade de um usuário, incluindo seções em grupos de seções aninhadas.

`../sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

Obtenha todas as seções que estão diretamente em um grupo de seções específico.

`../sectionGroups/{sectiongroup-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

Obtenha todas as seções que estão diretamente em um bloco de anotações específico.

`../notebooks/{notebook-id}/sections[?filter,orderby,select,top,skip,expand,count]` 

<br/>

As seções podem expandir as propriedades **parentNotebook** e **parentSectionGroup**.

A ordem de classificação padrão para seções é `name asc`.

A consulta padrão expande o bloco de anotações pai e o grupo de seções pai e seleciona as propriedades `id`, `name` e `self`.



<a name="get-section"></a>

### <a name="section-entity"></a>Entidade Section

Obtenha uma seção específica.

`../sections/{section-id}[?select,expand]` 

<br/>

As seções podem expandir as propriedades **parentNotebook** e **parentSectionGroup**.

A consulta padrão expande o bloco de anotações pai e o grupo de seções pai e seleciona as propriedades `id`, `name` e `self`.



<a name="get-section-groups"></a>

### <a name="sectiongroup-collection"></a>Coleção SectionGroup

Obtenha todos os grupos de seções de todos os blocos de anotações que são de propriedade de um usuário, incluindo grupos de seções aninhadas.

`../sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<br/>

Obtenha todos os grupos de seções que estão diretamente em um bloco de anotações específico. 

`../notebooks/{notebook-id}/sectionGroups[?filter,orderby,select,top,skip,expand,count]` 

<br/>

Os grupos de seções podem expandir as propriedades **sections**, **sectionGroups**, **parentNotebook** e **parentSectionGroup**.

A ordem de classificação padrão para grupos de seções é `name asc`.

A consulta padrão expande o bloco de anotações pai e o grupo de seções pai e seleciona as propriedades `id`, `name` e `self`.



<a name="get-section-group"></a>

### <a name="sectiongroup-entity"></a>Entidade SectionGroup

Obtenha um grupo de seções específico.

`../sectionGroups/{sectiongroup-id}[?select,expand]` 

<br/>

Os grupos de seções podem expandir as propriedades **sections**, **sectionGroups**, **parentNotebook** e **parentSectionGroup**.

A consulta padrão expande o bloco de anotações pai e o grupo de seções pai e seleciona as propriedades `id`, `name` e `self`.



<a name="get-notebooks"></a>

### <a name="notebook-collection"></a>Coleção de blocos de anotações

Obtenha todos os blocos de anotações de propriedade do usuário. 

`../notebooks[?filter,orderby,select,top,skip,expand,count]` 

<br/>

Os blocos de anotações podem expandir as propriedades **sections** e **sectionGroups**.

A ordem de classificação padrão para blocos de anotações é `name asc`. 



<a name="get-notebook"></a>

### <a name="notebook-entity"></a>Entidade Notebook

Obtenha um bloco de anotações específico.

`../notebooks/{notebook-id}[?select,expand]` 

<br/>

Os blocos de anotações podem expandir as propriedades **sections** e **sectionGroups**.



<a name="get-resource"></a>

### <a name="image-or-other-file-resource"></a>Imagem ou outro recurso de arquivo

Obtenha os dados binários de um recurso específico. 

`../resources/{resource-id}/$value` 

<br/>

Você pode encontrar a URI do recurso do arquivo na página de [HTML de saída](onenote-input-output-html.md).

Por exemplo, um rótulo **img** inclui os pontos de extremidade para a imagem original no atributo **data-fullres-src** e a imagem otimizada no atributo **src**. 

#### <a name="example"></a>Exemplo

```html
<img 
    src="https://www.onenote.com/api/v1.0/me/notes/resources/{image-id}/$value"  
    data-src-type="image/png"
    data-fullres-src="https://www.onenote.com/api/v1.0/resources/{image-id}/$value"  
    data-fullres-src-type="image/png" ... />
```

E um rótulo **object** inclui o ponto de extremidade para o recurso do arquivo no atributo **data**. 

#### <a name="example"></a>Exemplo

```html
<object
    data="https://www.onenote.com/api/v1.0/me/notes/resources/{file-id}/$value"
    data-attachment="fileName.pdf" 
    type="application/pdf" ... />
```

> **Observação:** não há suporte para obter uma coleção de recursos. 

Quando um recurso de arquivo é obtido, não é necessário incluir um tipo de conteúdo **Accept** na solicitação.

Para obter mais informações sobre solicitações GET, confira os seguintes recursos na referência do Microsoft Graph API REST:

- [GET Pages](/graph/api/page-get?view=graph-rest-1.0)
- [GET Sections](/graph/api/section-get?view=graph-rest-1.0)
- [GET SectionGroups](/graph/api/sectiongroup-get?view=graph-rest-1.0)
- [GET Notebooks](/graph/api/notebook-get?view=graph-rest-1.0) 




<a name="example"></a>

## <a name="example-get-requests"></a>Exemplo de solicitações GET

Você pode consultar entidades do OneNote e o conteúdo de página de pesquisa para obter apenas as informações que você precisa. Os exemplos a seguir mostram algumas maneiras de usar [opções de cadeia de caracteres de consulta com suporte](#supported-odata-query-string-options) em solicitações GET para o Microsoft Graph. 

**Lembre-se:**

- Todas as solicitações GET começam com a [URL raiz de serviço raiz](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url). <br/><br/>**Exemplos**: `https://www.onenote.com/api/v1.0/me/notes` e `https://www.onenote.com/api/v1.0/myOrganization/siteCollections/{id}/sites/{id}/notes/`

- Os espaços na cadeia de caracteres de consulta da URL devem usar a codificação de %20.<br/><br/>**Exemplo**: `filter=title%20eq%20'biology'`

- Os nomes de propriedade e as comparações de cadeias de caracteres de OData diferenciam maiúsculas de minúsculas. É recomendável usar a função **tolower** do OData para comparações de cadeia de caracteres.<br/><br/>**Exemplo**: `filter=tolower(name) eq 'spring'`
 

### <a name="search--filter"></a>search e filter  

Obtenha todas as páginas que contêm o termo *recipe* que foram criadas por um aplicativo específico (`search` está disponível somente para blocos de anotações de consumidor).

```
[GET] ../pages?search=recipe&filter=createdByAppId eq 'WLID-000000004C12821A'
```
 
### <a name="search--select"></a>search e select  

Obtenha o título, links de cliente do OneNote e o link **contentUrl** para todas as páginas que contêm o termo *golgi app* (`search` está disponível somente para blocos de anotações de consumidor).

```
[GET] ../pages?search=golgi app&select=title,links,contentUrl
```
 
### <a name="expand"></a>expand 

Obtenha todos os blocos de anotações e expanda suas seções e grupos de seções.  

```
[GET] ../notebooks?expand=sections,sectionGroups
```

<br/>

Obtenha um grupo de seções específico e expanda suas seções e grupos de seções.  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections,sectionGroups
```

<br/>

Obtenha uma página e expanda sua seção pai e o bloco de anotações pai.

```
[GET] ../pages/{page-id}?expand=parentSection,parentNotebook
```

### <a name="expand-multiple-levels"></a>expand (vários níveis)  

Obtenha todos os blocos de anotações e expanda suas seções e grupos de seções, e expanda todas as seções em cada grupo de seções.  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections)
```
 
> **Observação:** expandir pais de entidades filho ou filhos de entidades pai cria uma referência circular e não tem suporte.

 
### <a name="expand--select-multiple-levels"></a>expand e select (vários níveis)  

Obtenha o nome e o link **self** para um grupo de seções específico, e obtenha o nome e os links **self** para todas as suas seções.  

```
[GET] ../sectionGroups/{sectiongroup-id}?expand=sections(select=name,self)&select=name,self
```

<br/>

Obtenha o nome e o link **self** para todas as seções e o nome e o tempo criados de cada bloco de anotações pai da seção.  

```
[GET] ../sections?expand=parentNotebook(select=name,createdTime)&select=name,self
```

<br/>
 
Obtenha o título e uma ID de todas as páginas, e o nome da seção pai e do bloco de anotações pai.

```
[GET] ../pages?select=id,title&expand=parentSection(select=name),parentNotebook(select=name)
```

### <a name="expand--levels-multiple-levels"></a>expand e levels (vários níveis)  

Obtenha todos os blocos de anotações, seções e grupos de seção.  

```
[GET] ../notebooks?expand=sections,sectionGroups(expand=sections,sectionGroups(levels=max;expand=sections))
```
 
### <a name="filter"></a>filter

Obtenha todas as seções que foram criadas em outubro de 2014.

```
[GET] ../sections?filter=createdTime ge 2014-10-01 and createdTime le 2014-10-31
```

<br/>

Obtenha as páginas que foram criadas por um aplicativo específico desde 1º de janeiro de 2015.

```
[GET] ../pages?filter=createdByAppId eq 'WLID-0000000048118631' and createdTime ge 2015-01-01
```

### <a name="filter--expand"></a>filter e expand  

Obtenha todas as páginas em um bloco de anotações específico. A API retorna 20 entradas por padrão.

```
[GET] ../pages?filter=parentNotebook/id eq '{notebook-id}'&expand=parentNotebook
```

<br/>

Obtenha o nome e o link **pagesUrl** para todas as seções do bloco de anotações *School*. Comparações de cadeias de caracteres de OData diferenciam maiúsculas de minúsculas, portanto, use a função **tolower** como uma prática recomendada.

```
[GET] ../notebooks?filter=tolower(name) eq 'school'&expand=sections(select=name,pagesUrl)
```

### <a name="filter--select--orderby"></a>filter, select e orderby   

Obtenha o link name e **pagesUrl** para todas as seções que contêm o termo *spring* no nome da seção. Ordene as seções pela data da última modificação.

```
[GET] ../sections?filter=contains(tolower(name),'spring')&select=name,pagesUrl&orderby=lastModifiedTime desc
```
 
### <a name="orderby"></a>orderby

Obtenha a ordem das primeiras 20 páginas pela **createdByAppId** e, em seguida, pela hora de criação mais recente. A API retorna 20 entradas por padrão.

```
[GET] ../pages?orderby=createdByAppId,createdTime desc
```

### <a name="search--filter--top"></a>search, filter e top 

Obtenha as cinco páginas mais recentemente criadas desde 1º de janeiro de 2015 com a frase *cell division*. A API retorna 20 entradas por padrão com um máximo de 100. A ordem de classificação padrão de páginas é `lastModifiedTime desc` (`search` está disponível somente para blocos de anotações de consumidor).

```
[GET] ../pages?search="cell division"&filter=createdTime ge 2015-01-01&top=5
```

### <a name="search--filter--top--skip"></a>search, filter, top e skip  

Obtenha as cinco próximas páginas do conjunto de resultados (`search` está disponível somente para blocos de anotações de consumidor).

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=5
```

<br/>

E as cinco seguintes (`search` está disponível somente para blocos de anotações de consumidor).

```
[GET] ../pages?search=biology&filter=createdTime ge 2015-01-01&top=5&skip=10
```

> **Observação:** se **search** e **filter** são aplicadas à mesma solicitação, os resultados incluem apenas as entidades que correspondem aos dois critérios.
 
### <a name="select"></a>select

Obtenha nome, hora de criação e link **self** de todas as seções nos blocos de anotações do usuário.

```
[GET] ../sections?select=name,createdTime,self
```

<br/>

Obtenha título, hora de criação e links do cliente do OneNote para uma página específica.

```
[GET] ../pages/{page-id}?select=title,createdTime,links
```

### <a name="select--expand--filter-multiple-levels"></a>select, expand e filter (vários níveis)  

Obtenha nome e link **pagesUrl** para todas as seções do bloco de anotações do usuário.

```
[GET] ../notebooks?select=name&expand=sections(select=name,pagesUrl)&filter=isDefault eq true
```

### <a name="top--select--orderby"></a>top, select e orderby 

Obtenha o título e o link **self** das 50 primeiras páginas, classificadas em ordem alfabética por título. A API retorna 20 entradas por padrão com um máximo de 100. A ordem de classificação padrão é `lastModifiedTime desc`.

```
[GET] ../pages?top=50&select=title,self&orderby=title
```

### <a name="skip--top--select--orderby"></a>skip, top, select e orderby  

Obtenha as páginas de 51 a 100. A API retorna 20 entradas por padrão com um máximo de 100.

```
[GET] ../pages?skip=50&top=50&select=title,self&orderby=title
```

> **Observação:** As solicitações GET para páginas que recuperam o número padrão de entradas (ou seja, elas não especificam uma expressão **top**) retornam um link **\@odata.nextLink** na resposta que você pode usar para obter as próximas 20 entradas.
 

<a name="supported-odata-query-string-options"></a>

## <a name="supported-odata-query-string-options"></a>Opções de cadeia de caracteres de consulta OData com suporte.

Quando enviar solicitações GET para Microsoft Graph, você pode usar as opções de cadeia de caracteres de consulta de OData para personalizar sua consulta e obter apenas as informações que você precisa. Também podem melhorar o desempenho, reduzindo o número de chamadas para o serviço e o tamanho da carga de resposta.

> **Observação:** para facilitar a leitura, os exemplos neste artigo não usam a codificação de %20 necessária para espaços na cadeia de caracteres de consulta da URL: `filter=isDefault%20eq%20true`
 
| Opção de consulta | Exemplo e descrição |  
|------|------|  
| count | <p>`count=true`</p><p>A contagem de entidades da coleção. O valor é retornado na propriedade **odata.coun\@** t na resposta.</p> |  
| expand | <p>`expand=sections,sectionGroups`</p><p>Propriedades de navegação para retornar embutidas na resposta. As propriedades a seguir têm suporte para expressões **expand**:<br /> – Páginas: **parentNotebook**, **parentSection**<br /> – Seções: **parentNotebook**, **parentSectionGroup**<br /> – Grupos de seções: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**<br /> – Blocos de anotações: **sections**, **sectionGroups**</p><p>Por padrão, as solicitações GET de páginas expandem **parentSection** e selecionam as propriedades **id**, **name** e **self**. Solicitações GET padrão de seções e grupos de seções expandem **parentNotebook** e **parentSectionGroup** e selecionam as propriedades pai **id**, **name** e **self**. </p><p>Pode ser usado para uma única entidade ou uma coleção.<br />Separar com vírgulas várias propriedades.<br />Os nomes de propriedades diferenciam maiúsculas de minúsculas.</p> |   
| filter | <p>`filter=isDefault eq true`</p><p>Uma expressão booliana para se deseja incluir uma entrada no conjunto de resultados. Compatível com os seguintes operadores e funções OData:<br /> – Operadores de comparação: **eq**, **ne**, **gt**, **ge**, **lt**, **le**<br /> – Operadores lógicos: **and**, **or**, **not**<br /> – Funções de cadeia de caracteres: **contains**, **endswith**, **startswith**, **length**, **indexof**, **substring**, **tolower**, **toupper**, **trim**, **concat**</p><p>Os nomes de [propriedade](#onenote-entity-properties) e as comparações de cadeias de caracteres de OData diferenciam maiúsculas de minúsculas. É recomendável usar a função **tolower** do OData para comparações de cadeia de caracteres.<br /><br />**Exemplo**: `filter=tolower(name) eq 'spring'`</p> |  
| orderby | <p>`orderby=title,createdTime desc`</p><p>As [propriedades](#onenote-entity-properties) para classificar por, com uma ordem de classificação opcional **asc** (padrão) ou **desc**. Você pode classificar por qualquer propriedade da entidade na coleção solicitada.</p><p>A ordem de classificação padrão para blocos de anotações, grupos de seções e seções é `name asc`, e para páginas é `lastModifiedTime desc` (última página modificada primeiro).</p><p>Separe várias propriedades com vírgulas e liste-as na ordem em que deseja que sejam aplicadas. Os nomes de propriedades diferenciam maiúsculas de minúsculas.</p> |  
| search | <p>`search=cell div`</p><p>Disponível somente para blocos de anotações de consumidor.</p><p>O termo ou frase a ser pesquisado no título da página, no corpo da página, no texto alt da imagem e no texto OCR da imagem. Por padrão, as consultas de pesquisa retornam com resultados classificados por relevância.</p><p>O OneNote usa a pesquisa de texto completo do Bing para oferecer suporte à pesquisa de frase, lematização, tolerância de ortografia, relevância e classificação, quebra de palavras, vários idiomas e outros recursos de pesquisa de texto completo. As cadeias de caracteres da pesquisa não diferenciam maiúsculas de minúsculas.</p><p>Aplica-se somente a páginas em blocos de anotações de propriedade do usuário. O conteúdo indexado é privado e só pode ser acessado pelo proprietário. As páginas protegidas por senha não são indexadas. Aplicável somente ao ponto de extremidade `pages`.</p> |  
| select | <p>`select=id,title`</p><p>As [propriedades](#onenote-entity-properties) a serem retornadas. Pode ser usado para uma única entidade ou para uma coleção. Separar com vírgulas várias propriedades. Os nomes de propriedades diferenciam maiúsculas de minúsculas.</p> |  
| skip | <p>`skip=10`</p><p>O número de entradas para ignorar no conjunto de resultados. Costumam ser usadas para resultados de paginação.</p> |  
| top | <p>`top=50`</p><p>O número de entradas a serem retornadas no conjunto de resultados, até um máximo de 100. O valor padrão é 20.</p> |  

O Microsoft Graph também fornece a opção de cadeia de caracteres de consulta `pagelevel` que você pode usar para obter o nível e ordem das páginas dentro da seção pai. Aplicam-se apenas às consultas de páginas em uma seção específica ou consultas para uma página específica. 

#### <a name="examples"></a>Exemplos 

- `GET ../sections/{section-id}/pages?pagelevel=true` 
- `GET ../pages/{page-id}?pagelevel=true` 

### <a name="supported-odata-operators-and-functions"></a>Funções e operadores de OData compatíveis

Microsoft Graph é compatível com os seguintes operadores e funções do OData nas expressões de **filter**. Ao usar expressões de OData, lembre-se:

- Os espaços na cadeia de caracteres de consulta da URL devem ser substituídos pela codificação `%20`.<br/><br/>**Exemplo:** `filter=isDefault%20eq%20true`

- Os nomes de propriedade e as comparações de cadeias de caracteres de OData diferenciam maiúsculas de minúsculas. É recomendável usar a função **tolower** do OData para comparações de cadeia de caracteres.<br/><br/>**Exemplo:** `filter=tolower(name) eq 'spring'`


| Operador de comparação | Exemplo |  
|------|------|  
| eq<br />(igual a) | `createdByAppId eq '{app-id}'` |  
| ne<br />(é diferente de) | `userRole ne 'Owner'` |  
| gt<br />(maior que) | `createdTime gt 2014-02-23` |  
| ge<br />(maior que ou igual a) | `lastModifiedTime ge 2014-05-05T07:00:00Z` |  
| lt<br />(menor que) | `createdTime lt 2014-02-23` |  
| le<br />(menor que ou igual a) | `lastModifiedTime le 2014-02-23` |  

<br/>

| Operador lógico | Exemplo |  
|------|------|  
| e | `createdTime le 2014-01-30 and createdTime gt 2014-01-23` |  
| or | `createdByAppId eq '{app-id}' or createdByAppId eq '{app-id}'` |  
| not | `not contains(tolower(title),'school')` |  

<br/>

| Função da cadeia de caracteres | Exemplo |  
|------|------|   
| contains | `contains(tolower(title),'spring')` |  
| endswith | `endswith(tolower(title),'spring')` |  
| startswith | `startswith(tolower(title),'spring')` |  
| length | `length(title) eq 19` |  
| indexof | `indexof(tolower(title),'spring') eq 1` |  
| substring | `substring(tolower(title),1) eq 'spring'` |  
| tolower | `tolower(title) eq 'spring'` |  
| toupper | `toupper(title) eq 'SPRING'` |  
| trim | `trim(tolower(title)) eq 'spring'` |  
| concat | `concat(title,'- by MyRecipesApp') eq 'Carrot Cake Recipe - by MyRecipesApp'` |  
 

<a name="properties"></a>

## <a name="onenote-entity-properties"></a>Propriedades de entidade do OneNote

As expressões de consulta **filter**, **select**, **expand** e **orderby** podem incluir propriedades de entidades do OneNote. 

#### <a name="example"></a>Exemplo

`../sections?filter=createdTime ge 2015-01-01&select=name,pagesUrl&orderby=lastModifiedTime desc` 

Os nomes de propriedades diferenciam maiúsculas de minúsculas em expressões de consulta.

Para obter a lista de propriedades e seus tipos, confira os seguintes recursos na referência do Microsoft Graph API REST:

- [GET Pages](/graph/api/page-get?view=graph-rest-1.0)
- [GET Sections](/graph/api/section-get?view=graph-rest-1.0)
- [GET SectionGroups](/graph/api/sectiongroup-get?view=graph-rest-1.0)
- [GET Notebooks](/graph/api/notebook-get?view=graph-rest-1.0) 



A opção de cadeia de caracteres de consulta **expand** pode ser usada com as seguintes propriedades de navegação:

- Páginas: **parentNotebook**, **parentSection**
- Seções: **parentNotebook**, **parentSectionGroup**
- Grupos de seções: **sections**, **sectionGroups**, **parentNotebook**, **parentSectionGroup**
- Blocos de anotações: **sections**, **sectionGroups**


<a name="request-response-info"></a>

## <a name="request-and-response-information-for-get-requests"></a>Informações de solicitação e resposta para solicitações de *GET*

| Dados da solicitação | Descrição |  
|------|------|  
| Protocolo | Todas as solicitações usam o protocolo HTTPS de SSL/TLS. |  
| Cabeçalho de autorização | <p>`Bearer {token}`, onde `{token}` é um token de acesso do OAuth 2.0 válido para o aplicativo registrado.</p><p>Se ausente ou inválido, a solicitação falha com um código de status 401. Consulte [Autenticação e permissões](permissions-reference.md).</p> |  
| Cabeçalho Accept | <p> `application/json` para entidades e conjuntos de entidades do OneNote</p><p> `text/html` para conteúdo de página</p> | 

<br/>

| Dados de resposta | Descrição |  
|------|------|  
| Código de êxito | Um código de status de HTTP 200. |  
| Corpo da resposta | Uma representação de OData da entidade ou conjunto de entidades no formato JSON, da página HTML ou dados binários do recurso de arquivo.  |  
| Erros | Se a solicitação falhar, a API retornará erros no objeto [errors](onenote-error-codes.md) no **\@@api.diagnostics** no corpo da resposta. |  
| Cabeçalho X-CorrelationId | Um GUID que identifica exclusivamente a solicitação. Você pode usar esse valor juntamente com o valor do cabeçalho Data ao trabalhar com o suporte da Microsoft para solucionar problemas. |  


<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-notes-service-root-url"></a>Criar a URL raiz do serviço de anotações do Microsoft Graph

A URL raiz do serviço de anotações do Microsoft Graph usa o formato a seguir para todas as chamadas para o Microsoft Graph:

`https://graph.microsoft.com/{version}/me/onenote/`  

O segmento `version` na URL representa a versão do Microsoft Graph que você deseja usar. Use `v1.0` para o código de produção estável. Use `beta` para experimentar um recurso que está em desenvolvimento. Os recursos e a funcionalidade na versão beta podem mudar, por isso, você não deve usá-la no código de produção. 

Use `me` para o conteúdo do OneNote que o usuário atual pode acessar (exclusivo e compartilhado). Use `users/{id}` para o conteúdo do OneNote que o usuário especificado (na URL) compartilhou com o usuário atual. Use o [Microsoft Graph](https://graph.microsoft.com/v1.0/users) para obter as IDs de usuário. 


<a name="permissions"></a>

## <a name="permissions-for-get-requests"></a>Permissões para solicitações GET

Para obter conteúdo ou estrutura do OneNote, você vai precisar solicitar as permissões adequadas. 

Os seguintes escopos permitem solicitações GET para Microsoft Graph. Escolha o nível mais baixo de permissões que seu aplicativo precisa para realizar o trabalho.

Escolha entre:

- Notes.read
- Notes.ReadWrite
- Notes.ReadWrite.All

Para saber mais sobre escopos de permissão e como eles funcionam, confira [Referência de permissões do Microsoft Graph](permissions-reference.md).

<a name="see-also"></a>

## <a name="see-also"></a>Confira também

- [HTML de entrada e saída para páginas do OneNote](onenote-input-output-html.md)
- [Integrar com o OneNote](integrate-with-onenote.md)
- [Blog de desenvolvedor do OneNote](https://go.microsoft.com/fwlink/?LinkID=390183)
- [Perguntas de desenvolvimento do OneNote no Microsoft Q&A](/answers/topics/microsoft-graph-notes.html)
- [Repositórios do OneNote no GitHub](https://go.microsoft.com/fwlink/?LinkID=390178)
