---
author: rahmit
description: Esse recurso representa uma página na lista SitePages.
ms.date: 03/15/2018
title: SitePage
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: d92a78ff73854d465ba8363b7bddff66be6bffc4
ms.sourcegitcommit: 1a84f80798692fc0381b1acecfe023b3ce6ab02c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2020
ms.locfileid: "41953610"
---
# <a name="sitepage-resource"></a>recurso sitePage

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Esse recurso representa uma página na [lista][]SitePages.
Ele contém o título, o layout e uma coleção de [WebPart][]s.

## <a name="tasks-on-a-page"></a>Tarefas em uma página

As tarefas a seguir estão disponíveis para recursos do **sitePage** .
Todos os exemplos abaixo são relativos a um [site][], por `https://graph.microsoft.com/{api-version}/sites/{site-id}`exemplo:.

| Tarefa comum                     | Método HTTP
|:--------------------------------|:------------------------------
| [List pages][]                  | OBTER/Pages
| [Obter página][]                    | OBTER/Pages/{Page-ID}
| [Create][]                      | POSTAR/Pages
| [Delete][]                      | EXCLUIR/Pages/{Page-ID}
| [Publish][]                     | POSTAR/Pages/{Page-ID}/Publish

[List pages]: ../api/sitepage-list.md
[Obter página]: ../api/sitepage-get.md
[Create]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON de um recurso **sitePage** .

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.sitePage",
  "openType": true
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },

  /* page content */
  "title": "string",
  "pageLayoutType": "String",
  "webParts": [{ "@odata.type": "microsoft.graph.webPart" }],

  /* authoring metadata */
  "publishingState": { "@odata.type": "microsoft.graph.publicationFacet" },

   /* inherited from baseItem */
  "id": "string (identifier)",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "String (timestamp)",
  "description": "string",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "webUrl": "url"
}
```

## <a name="properties"></a>Propriedades

O recurso **sitePage** tem as propriedades a seguir.

| Nome da propriedade    | Tipo                         | Descrição
|:-----------------|:-----------------------------|:---------------------------
| contentType      | [contentTypeInfo][]          | O tipo de conteúdo da página.

## <a name="page-content"></a>Conteúdo da página

O recurso **sitePage** tem os seguintes campos de conteúdo.

| Nome da propriedade      | Tipo                       | Descrição
|:-------------------|:---------------------------|:---------------------------
| title              | cadeia de caracteres                     | O título da página.
| pageLayout         | string                     | O nome do layout de página da página.
| webParts           | [webPart][]                | As Web Parts na página.

## <a name="authoring-metadata"></a>Criação de metadados

O recurso **sitePage** tem os seguintes metadados relacionados a criação. A propriedade publishingstate refletirá o estado de criação da página, como check-out ou publicada.

| Nome da propriedade          | Tipo                   | Descrição
|:-----------------------|:-----------------------|:---------------------------
| publishingState        | [publicationFacet][]   | O status de publicação e a versão do MM.mm da página.

As propriedades a seguir são herdadas do **[baseItem][]**.

| Nome da propriedade        | Tipo              | Descrição
|:---------------------|:------------------|:----------------------------------
| id                   | cadeia de caracteres            | O identificador exclusivo do item. Somente leitura.
| name                 | string            | O nome/título do item.
| createdBy            | [identitySet][]   | Identidade do criador desse item. Somente leitura.
| eTag                 | string            | ETag do item. Somente leitura.
| lastModifiedBy       | [identitySet][]   | Identidade da última pessoa que alterou esse item. Somente leitura.
| lastModifiedDateTime | DateTimeOffset    | A data e a hora que o item foi modificado pela última vez. Somente leitura.
| parentReference      | [itemReference][] | Informações do pai, se o item tiver um pai. Somente leitura.
| webUrl               | string (url)      | A URL que exibe o item no navegador. Somente leitura.

## <a name="relationships"></a>Relações

O recurso **sitePage** não tem relações com outros recursos.

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[list]: list.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[publicationFacet]: publicationfacet.md
[site]: site.md
[webPart]: webpart.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Page",
  "tocBookmarks": {
    "Page": "#"
  },
  "suppressions": []
}
-->

<!--
TODO:
* Define {page-id}
* Update examples
    * Be consistent with other URLs in the documentation.
    * Try to use the same site, library, etc.
    * Add the URL to the underlying list item resource in the API
* PATCH for list item patches /item/{item-id}/fields.
-->
