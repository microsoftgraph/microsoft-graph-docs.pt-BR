---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: SitePage
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 7b1634e79214f1cece85a78af29db6422ac03a81
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640655"
---
# <a name="sitepage-resource"></a>recurso de sitePage

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Esse recurso representa uma página na [lista][]SitePages.
Ele contém uma coleção de [Web Part][]s, layout e o título.

## <a name="tasks-on-a-page"></a>Tarefas em uma página

As tarefas a seguir estão disponíveis para os recursos de **sitePage** .
Todos os exemplos a seguir são em relação um [site][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.

| Tarefa comum                     | Método HTTP
|:--------------------------------|:------------------------------
| [Listar páginas][]                  | OBTER /pages
| [Get page][]                    | OBTER /pages/ {id page}
| [Create][]                      | /Pages POST
| [Delete][]                      | Excluir /pages/ {id page}
| [Publish][]                     | POSTAR /pages/ {id page} / publicar

[Listar páginas]: ../api/sitepage-list.md
[Get page]: ../api/sitepage-get.md
[Create]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON de um recurso de **sitePage** .

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.sitePage"
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },

  /* page content */
  "title": "string",
  "pageLayout": "Article",
  "webParts": [{ "@odata.type": "microsoft.graph.sitePageWebParts" }],

  /* authoring metadata */
  "publishingState": { "@odata.type": "microsoft.graph.publicationFacet" },

  /* inherited from baseItem */
  "id": "string",
  "name": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "datetime",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "webUrl": "url"
}
```

## <a name="properties"></a>Propriedades

O recurso de **sitePage** possui as seguintes propriedades.

| Nome da propriedade    | Tipo                         | Descrição
|:-----------------|:-----------------------------|:---------------------------
| contentType      | [contentTypeInfo][]          | O tipo de conteúdo da página.

## <a name="page-content"></a>Conteúdo da página

O recurso de **sitePage** tem os seguintes campos de conteúdo.

| Nome da propriedade      | Tipo                       | Descrição
|:-------------------|:---------------------------|:---------------------------
| title              | string                     | O título da página.
| pageLayout         | string                     | O nome do layout de página da página.
| Web Parts           | [Web Part][]                | As web parts na página.

## <a name="authoring-metadata"></a>Criação de metadados

O recurso de **sitePage** tem os seguintes metadados relacionados a criação. A propriedade publishingState irão refletir a estado como check-out ou publicada de criação de páginas.

| Nome da propriedade          | Tipo                   | Descrição
|:-----------------------|:-----------------------|:---------------------------
| publishingState        | [publicationFacet][]   | O status de publicação e a versão de MM.mm da página.

As propriedades a seguir são herdadas do **[baseItem][]**.

| Nome da propriedade        | Tipo              | Descrição
|:---------------------|:------------------|:----------------------------------
| id                   | string            | O identificador exclusivo do item. Somente leitura.
| name                 | string            | O nome/título do item.
| createdBy            | [identitySet][]   | Identidade do criador desse item. Somente leitura.
| eTag                 | string            | ETag do item. Somente leitura.
| lastModifiedBy       | [identitySet][]   | Identidade da última pessoa que alterou esse item. Somente leitura.
| lastModifiedDateTime | DateTimeOffset    | A data e a hora que o item foi modificado pela última vez. Somente leitura.
| parentReference      | [itemReference][] | A data e a hora que o item foi modificado pela última vez. Somente leitura.
| webUrl               | string (url)      | A URL que exibe o item no navegador. Somente leitura.

## <a name="relationships"></a>Relações

O recurso de **sitePage** não tem relações para outros recursos.

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
[Web Part]: webpart.md

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
  "suppressions": [
    "Error: /api-reference/beta/resources/sitepage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
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
