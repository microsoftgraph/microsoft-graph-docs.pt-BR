---
author: JeremyKelley
title: Recurso List
ms.localizationpriority: high
ms.prod: sharepoint
description: O recurso de lista representa uma lista em um site.
doc_type: resourcePageType
ms.openlocfilehash: 8372127f2fc54444f66893331bc49cc1fd0e2428
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577564"
---
# <a name="list-resource"></a>Recurso List

Namespace: microsoft.graph

O recurso **list** representa uma lista em um [site][].
Este recurso contém as propriedades de nível superior da lista, incluindo definições de modelo e campo.

## <a name="tasks-on-a-list"></a>Tarefas em list

As tarefas a seguir estão disponíveis para os recursos list.

Todos os exemplos abaixo são relativos a um site, por exemplo, `https://graph.microsoft.com/v1.0/sites/{site-id}`.

| Tarefa comum               | Método HTTP
|:--------------------------|:------------------------------
| [Obter lista][]              | GET /lists/{list-id}
| [Criar lista][]           | POSTAR/listas
| [Enumerar itens de lista][]  | GET /lists/{list-id}/items
| [Atualizar item de lista][]      | PATCH /lists/{list-id}/items/{item-id}
| [Excluir item de lista][]      | DELETE /lists/{list-id}/items/{item-id}
| [Criar item de lista][]      | POST /lists/{list-id}
| [Obter canal WebSocket][] | GET /lists/{list-id}/subscriptions/socketIo
| [Listar operações](../api/list-list-operations.md)| GET /lists/{list-id}/operations

[Obter lista]: ../api/list-get.md
[Criar lista]: ../api/list-create.md
[Enumerar itens de lista]: ../api/listitem-list.md
[Atualizar item de lista]: ../api/listitem-update.md
[Excluir item de lista]: ../api/listitem-delete.md
[Criar item de lista]: ../api/listitem-create.md
[Obter canal WebSocket]: ../api/subscriptions-socketio.md

## <a name="properties"></a>Propriedades

O recurso **list** tem as seguintes propriedades.

| Nome da propriedade    | Tipo                             | Descrição
|:-----------------|:---------------------------------|:---------------------------
| **displayName**  | string                           | O título em exibição da lista.
| **list**         | [listInfo][]                     | Fornece mais detalhes sobre a lista.
| **system**       | [systemFacet][]                  | Se presente, indica que esta é uma lista gerenciada pelo sistema. Somente leitura.

As propriedades a seguir são herdadas do **[baseItem][]**.

| Nome da propriedade            | Tipo              | Descrição
|:-------------------------|:------------------|:------------------------------
| **id**                   | string            | O identificador exclusivo do item. Somente leitura.
| **name**                 | string            | O nome do item.
| **createdBy**            | [identitySet][]   | Identidade do criador deste item. Somente leitura.
| **createdDateTime**      | DateTimeOffset    | A data e a hora da criação do item. Somente leitura.
| **description**          | string            | O texto descritivo do item.
| **eTag**                 | string            | ETag do item. Somente leitura.                                                          |
| **lastModifiedBy**       | [identitySet][]   | Identidade do último modificador deste item. Somente leitura.
| **lastModifiedDateTime** | DateTimeOffset    | A data e a hora que o item foi modificado pela última vez. Somente leitura.
| **parentReference**      | [itemReference][] | Informações do pai, se o item tiver um pai. Leitura e gravação.
| **sharepointIds**        | [sharepointIds][] | Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.
| **webUrl**               | string (url)      | A URL que exibe o item no navegador. Somente leitura.

## <a name="relationships"></a>Relações

O recurso **list** tem as seguintes relações com outros recursos.

| Nome da relação | Tipo                             | Descrição
|:------------------|:---------------------------------|:----------------------
| **drive**         | [drive][]                        | Presente apenas em bibliotecas de documentos. Permite o acesso à lista como um recurso [drive][] com [driveItems][driveItem].
| **items**         | Collection([listItem][])         | Todos os itens contidos na lista.
| **columns**       | Collection([columnDefinition][]) | A coleção de definições de campo para esta lista.
| **contentTypes**  | Collection([contentType][])      | A coleção de tipos de conteúdo presentes nesta lista.
| **operations** | Coleção [richLongRunningOperation](../resources/richlongrunningoperation.md) | A coleção de operações de execução longa na lista. 
| **assinaturas** | Conjunto([assinatura][])     | O conjunto de assinaturas na lista.

[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[driveItem]: driveitem.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[sharepointIds]: sharepointids.md
[site]: site.md
[systemFacet]: systemfacet.md
[assinatura]: subscription.md

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "items",
    "drive"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type&quot;: &quot;microsoft.graph.list"
}-->

```json
{
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "displayName": "title of list",
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "items": [ { "@odata.type": "microsoft.graph.listItem" } ],
  "list": {
    "@odata.type": "microsoft.graph.listInfo",
    "hidden": false,
    "template&quot;: &quot;documentLibrary | genericList | survey | links | announcements | contacts | accessRequest ..."
  },
  "operations": [ { "@odata.type": "microsoft.graph.richLongRunningOperation" }],
  "system": false,
  "subscriptions": [ {"@odata.type": "microsoft.graph.subscription"} ],

  /* inherited from baseItem */
  "id": "string",
  "name": "name of list",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of list",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "webUrl&quot;: &quot;url to visit the list in a browser"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Lists",
  "tocBookmarks": {
    "Lists&quot;: &quot;#"
  }
} -->

