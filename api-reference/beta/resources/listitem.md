---
author: JeremyKelley
description: Este recurso representa um item em uma list do SharePoint.
ms.date: 09/11/2017
title: ListItem
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: e457840ee55206b47b035ae53127c5bf3e5130c6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055257"
---
# <a name="listitem-resource"></a>Recurso ListItem

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Este recurso representa um item em uma **[list][]** do SharePoint.
Os valores de coluna na lista estão disponíveis por meio do dicionário `fieldValueSet`.

## <a name="tasks-on-a-listitem"></a>Tarefas em um listItem

As tarefas a seguir estão disponíveis para recursos **listItem**.
Todos os exemplos a seguir referem-se a uma **[list][]**, por exemplo: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.

| Tarefa comum                    | Método HTTP
|:-------------------------------|:------------------------
| [Get][]                        | GET /items/{item-id}
| [Obter valores de coluna][Get]       | GET /items/{item-id}?expand=fields
| [Obter análises][]              | OBTER/Items/{Item-ID}/Analytics
| [Obter atividades por intervalo][] | OBTER/items/{item-id}/getActivitiesByInterval
| [Create][]                     | POST /items
| [Delete][]                     | DELETE /items/{item-id}
| [Update][]                     | PATCH /items/{item-id}
| [Atualizar valores de coluna][Update] | PATCH /items/{item-id}/fields

[Get]: ../api/listitem-get.md
[Obter análises]: ../api/itemanalytics-get.md
[Obter atividades por intervalo]: ../api/itemactivity-getbyinterval.md
[Create]: ../api/listitem-create.md
[Delete]: ../api/listitem-delete.md
[Update]: ../api/listitem-update.md

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON de um recurso **listItem**.

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.listItem"
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },

  /* relationships */
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "analytics": { "@odata.type": "microsoft.graph.itemAnalytics" },
  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
  "versions": [{"@odata.type": "microsoft.graph.listItemVersion"}],

  /* inherited from baseItem */
  "id": "string",
  "name": "name of resource",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of resource",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference"},
  "webUrl": "url"
}
```

## <a name="properties"></a>Propriedades

O recurso **listItem** tem as seguintes propriedades.

| Nome da propriedade | Tipo                | Descrição
|:--------------|:--------------------|:-------------------------------
| contentType   | [contentTypeInfo][] | O tipo de conteúdo deste item de lista

As propriedades a seguir são herdadas do **[baseItem][]**.

| Nome da propriedade        | Tipo              | Descrição
|:---------------------|:------------------|:----------------------------------
| id                   | string            | O identificador exclusivo do item. Somente leitura.
| name                 | string            | O nome/título do item.
| createdBy            | [identitySet][]   | Identidade do criador desse item. Somente leitura.
| createdDateTime      | DateTimeOffset    | A data e a hora da criação do item. Somente leitura.
| description          | string            | O texto descritivo do item.
| eTag                 | string            | ETag do item. Somente leitura.                                                          |
| lastModifiedBy       | [identitySet][]   | Identidade da última pessoa que alterou esse item. Somente leitura.
| lastModifiedDateTime | DateTimeOffset    | A data e a hora que o item foi modificado pela última vez. Somente leitura.
| parentReference      | [itemReference][] | Informações do pai, se o item tiver um pai. Leitura e gravação.
| sharepointIds        | [sharepointIds][] | Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.
| webUrl               | string (url)      | A URL que exibe o item no navegador. Somente leitura.

## <a name="relationships"></a>Relações

 O recurso **listItem** tem as seguintes relações com outros recursos.

| Nome da relação | Tipo                           | Descrição
|:------------------|:-------------------------------|:-------------------------------
| activities        | Conjunto [itemActivity][]    | A lista de atividades recentes que ocorreram neste item.
| análise         | recurso [itemAnalytics][]     | Análise sobre as atividades de visualização que ocorreram neste item.
| driveItem         | [driveItem][]                  | Para bibliotecas de documentos, a relação **driveItem** expõe listItem como um **[driveItem][]**
| campos            | [fieldValueSet][]              | Os valores das colunas definidos neste item de lista.
| versões          | coleção [listItemVersion][]  | A lista de versões anteriores do item de lista.

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[driveItem]: driveitem.md
[fieldValueSet]: fieldvalueset.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[list]: list.md
[listItemVersion]: listitemversion.md
[sharepointIds]: sharepointids.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ListItem",
  "tocBookmarks": {
    "ListItem": "#"
  },
  "suppressions": []
}
-->


