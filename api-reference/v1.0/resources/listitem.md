---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListItem
ms.openlocfilehash: 0f5afaeff29da6f3a6330975adece44731e014bc
ms.sourcegitcommit: 4bdff5fdaea824c7c1204ec7dd641abc282d32a1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2018
---
# <a name="listitem-resource"></a>Recurso ListItem

Este recurso representa um item em uma **[list][]** do SharePoint.
Os valores de coluna na lista estão disponíveis por meio do dicionário `fieldValueSet`.

## <a name="tasks-on-a-listitem"></a>Tarefas em um listItem

As tarefas a seguir estão disponíveis para recursos **listItem**.
Todos os exemplos a seguir referem-se a uma **[list][]**, por exemplo: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.

| Tarefa comum                    | Método HTTP
|:-------------------------------|:------------------------
| [Get][]                        | GET /items/{item-id}
| [Obter valores de coluna][Get]       | GET /items/{item-id}?expand=fields
| [Create][]                     | POST /items
| [Delete][]                     | DELETE /items/{item-id}
| [Update][]                     | PATCH /items/{item-id}
| [Atualizar valores de coluna][Update] | PATCH /items/{item-id}/fields

[Get]: ../api/listItem_get.md
[Create]: ../api/listItem_create.md
[Delete]: ../api/listItem_delete.md
[Update]: ../api/listItem_update.md

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON de um recurso **listItem**.

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.listItem",
       "keyProperty": "id" } -->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentType" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },

  /* relationships */
  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },

  /* inherited from baseItem */
  "id": "string",
  "name": "name of resource",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of resource",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "webUrl": "url"
}
```

## <a name="properties"></a>Propriedades

O recurso **listItem** tem as seguintes propriedades.

| Nome da propriedade | Tipo                | Descrição
|:--------------|:--------------------|:-------------------------------
| contentType   | [contentTypeInfo][] | O tipo de conteúdo deste item de lista
| campos        | [fieldValueSet][]   | Os valores das colunas definidos neste item de lista.

As propriedades a seguir são herdadas do **[baseItem][]**.

| Nome da propriedade        | Tipo             | Descrição
|:---------------------|:-----------------|:-----------------------------------
| id                   | string           | O identificador exclusivo do item. Somente leitura.
| name                 | string           | O nome/título do item.
| createdBy            | [identitySet][]  | Identidade do criador desse item. Somente leitura.
| createdDateTime      | DateTimeOffset   | A data e a hora da criação do item. Somente leitura.
| description          | string           | O texto descritivo do item.
| lastModifiedBy       | [identitySet][]  | Identidade da última pessoa que alterou esse item. Somente leitura.
| lastModifiedDateTime | DateTimeOffset   | A data e a hora que o item foi modificado pela última vez. Somente leitura.
| webUrl               | string (url)     | A URL que exibe o item no navegador. Somente leitura.

## <a name="relationships"></a>Relações

 O recurso **listItem** tem as seguintes relações com outros recursos.

| Nome da relação | Tipo                        | Descrição
|:------------------|:----------------------------|:-------------------------------
| driveItem         | [driveItem][]               | Para bibliotecas de documentos, a relação **driveItem** expõe listItem como um **[driveItem][]**

[baseItem]: baseItem.md
[contentTypeInfo]: contentTypeInfo.md
[driveItem]: driveItem.md
[fieldValueSet]: fieldValueSet.md
[identitySet]: identitySet.md
[list]: list.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ListItem",
  "tocBookmarks": {
    "ListItem": "#"
  }
} -->
