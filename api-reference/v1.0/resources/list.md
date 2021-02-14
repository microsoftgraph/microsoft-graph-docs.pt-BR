---
author: JeremyKelley
ms.date: 09/11/2017
title: Listar
localization_priority: Priority
ms.prod: sharepoint
description: O recurso de lista representa uma lista em um site.
doc_type: resourcePageType
ms.openlocfilehash: 4079320ef785dbdb3c1367fad92cda46eab0b4fa
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239363"
---
# <a name="list-resource"></a>Recurso List

Namespace: microsoft.graph

O recurso **list** representa uma lista em um [site][].
Este recurso contém as propriedades de nível superior da lista, incluindo definições de modelo e campo.

## <a name="tasks-on-a-list"></a>Tarefas em list

As tarefas a seguir estão disponíveis para os recursos list.
**Observação:** esta versão beta só permite navegar por listas, não criar ou atualizá-las.
Você pode, no entanto, criar ou atualizar [itens de lista][listItem].

Todos os exemplos a seguir referem-se a um site: `https://graph.microsoft.com/v1.0/sites/{site-id}`.

| Tarefa comum               | Método HTTP
|:--------------------------|:------------------------------
| [Obter lista][]              | GET /lists/{list-id}
| [Criar lista][]           | POSTAR/listas
| [Enumerar itens de lista][]  | GET /lists/{list-id}/items
| [Atualizar item de lista][]      | PATCH /lists/{list-id}/items/{item-id}
| [Excluir item de lista][]      | DELETE /lists/{list-id}/items/{item-id}
| [Criar item de lista][]      | POST /lists/{list-id}
| [Obter canal WebSocket][] | GET /lists/{list-id}/subscriptions/socketIo

[Obter lista]: ../api/list-get.md
[Criar lista]: ../api/list-create.md
[Enumerar itens de lista]: ../api/listitem-list.md
[Atualizar item de lista]: ../api/listitem-update.md
[Excluir item de lista]: ../api/listitem-delete.md
[Criar item de lista]: ../api/listitem-create.md
[Obter canal WebSocket]: ../api/subscriptions-socketio.md

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON de um recurso **list**.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "items",
    "drive"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.list"
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
    "template": "documentLibrary | genericList | survey | links | announcements | contacts | accessRequest ..."
  },
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
  "webUrl": "url to visit the list in a browser"
}
```

## <a name="properties"></a>Propriedades

O recurso **list** tem as seguintes propriedades.

| Nome da propriedade    | Tipo                             | Descrição
|:-----------------|:---------------------------------|:---------------------------
| **displayName**  | string                           | O título em exibição da lista.
| **list**         | [listInfo][]                     | Fornece mais detalhes sobre a lista.
| **system**       | [systemFacet][]                  | Se estiver presente, indica que se trata de uma lista gerenciada pelo sistema. Somente leitura.

As propriedades a seguir são herdadas do **[baseItem][]**.

| Nome da propriedade            | Tipo              | Descrição
|:-------------------------|:------------------|:------------------------------
| **id**                   | string            | O identificador exclusivo do item. Somente leitura.
| **name**                 | string            | O nome do item.
| **createdBy**            | [identitySet][]   | Identidade do criador desse item. Somente leitura.
| **createdDateTime**      | DateTimeOffset    | A data e a hora da criação do item. Somente leitura.
| **description**          | string            | O texto descritivo do item.
| **eTag**                 | string            | ETag do item. Somente leitura.                                                          |
| **lastModifiedBy**       | [identitySet][]   | Identidade da última pessoa que alterou esse item. Somente leitura.
| **lastModifiedDateTime** | DateTimeOffset    | A data e a hora que o item foi modificado pela última vez. Somente leitura.
| **parentReference**      | [itemReference][] | Informações do pai, se o item tiver um pai. Leitura e gravação.
| **sharepointIds**        | [sharepointIds][] | Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.
| **webUrl**               | string (url)      | A URL que exibe o item no navegador. Somente leitura.

## <a name="relationships"></a>Relações

O recurso **list** tem as seguintes relações com outros recursos.

| Nome da relação | Tipo                             | Descrição
|:------------------|:---------------------------------|:----------------------
| **drive**         | [drive][]                        | Presente somente em bibliotecas de documentos. Permite o acesso à lista como um recurso de [unidade][] com [driveItems][driveItem].
| **items**         | Collection([listItem][])         | Todos os itens contidos na lista.
| **columns**       | Collection([columnDefinition][]) | A coleção de definições de campo para esta lista.
| **contentTypes**  | Collection([contentType][])      | A coleção de tipos de conteúdo presentes nesta lista.
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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Lists",
  "tocBookmarks": {
    "Lists": "#"
  }
} -->

