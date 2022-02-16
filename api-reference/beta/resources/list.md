---
author: JeremyKelley
description: O recurso de lista representa uma lista em um site.
title: Recurso List
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: c2f0fd3fe48eaebbf7f730d0e52e964aab2e057b
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854470"
---
# <a name="list-resource"></a>Recurso List

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **list** representa uma lista em um [site][].
Este recurso contém as propriedades de nível superior da lista, incluindo definições de modelo e campo.

## <a name="tasks-on-a-list"></a>Tarefas em list

As tarefas a seguir estão disponíveis para os recursos list.
**Observação:** esta versão beta só permite navegar por listas, não criar ou atualizá-las.
Você pode, no entanto, criar ou atualizar [itens de lista][listItem].

Todos os exemplos abaixo são relativos a um site, por exemplo, `https://graph.microsoft.com/beta/sites/{site-id}`.

| Tarefa comum               | Método HTTP
|:--------------------------|:------------------------------
| [Obter listas em um site][]   | GET /sites/{site-id}/lists
| [Criar lista][]           | POSTAR/listas
| [Obter lista][]              | GET /lists/{list-id}
| [Enumerar itens de lista][]  | GET /lists/{list-id}/items
| [Atualizar item de lista][]      | PATCH /lists/{list-id}/items/{item-id}
| [Excluir item de lista][]      | DELETE /lists/{list-id}/items/{item-id}
| [Criar item de lista][]      | POST /lists/{list-id}
| [Obter atividades recentes][] | GET /lists/{list-id}/activities
| [Obter canal WebSocket][] | GET /lists/{list-id}/subscriptions/socketIo
|[Tipos de conteúdo de lista][]          | GET /lists/{list-id}/contentTypes
|[Adicionar cópia do tipo de conteúdo do site][] | POST /lists/{list-id}/contentTypes/addCopy
|[Colunas de lista][]               | GET /lists/{list-id}/columns
|[Criar coluna][]              | POST /lists/{list-id}/columns
|[Listar operações](../api/list-list-operations.md)|GET /lists/{list-id}/operations

[Obter listas em um site]: ../api/list-list.md
[Obter lista]: ../api/list-get.md
[Criar lista]: ../api/list-create.md
[Enumerar itens de lista]: ../api/listitem-list.md
[Atualizar item de lista]: ../api/listitem-update.md
[Excluir item de lista]: ../api/listitem-delete.md
[Criar item de lista]: ../api/listitem-create.md
[Obter atividades recentes]: ../api/activities-list.md
[Obter canal WebSocket]: ../api/subscriptions-socketio.md
[Tipos de conteúdo de lista]: ../api/list-list-contenttypes.md
[Adicionar cópia do tipo de conteúdo do site]: ../api/contenttype-addCopy.md
[Colunas de lista]: ../api/list-list-columns.md
[Criar coluna]: ../api/list-post-columns.md

## <a name="properties"></a>Propriedades

O recurso **list** tem as seguintes propriedades.

| Nome da propriedade    | Tipo                             | Descrição
|:-----------------|:---------------------------------|:---------------------------
| **columns**      | Collection([columnDefinition][]) | A coleção de definições de campo para esta lista.
| **contentTypes** | Collection([contentType][])      | A coleção de tipos de conteúdo presentes nesta lista.
| **displayName**  | string                           | O título em exibição da lista.
| **list**         | [listInfo][]                     | Fornece mais detalhes sobre a lista.
| **system**       | [systemFacet][]                  | Se presente, indica que esta é uma lista gerenciada pelo sistema. Somente leitura.

As propriedades a seguir são herdadas do **[baseItem][]**.

| Nome da propriedade            | Tipo             | Descrição
|:-------------------------|:-----------------|:-------------------------------
| **id**                   | string           | O identificador exclusivo do item. Somente leitura.
| **name**                 | string           | O nome do item.
| **createdBy**            | [identitySet][]  | Identidade do criador deste item. Somente leitura.
| **createdDateTime**      | DateTimeOffset   | A data e a hora da criação do item. Somente leitura.
| **description**          | string           | O texto descritivo do item.
| **lastModifiedBy**       | [identitySet][]  | Identidade do último modificador deste item. Somente leitura.
| **lastModifiedDateTime** | DateTimeOffset   | A data e a hora que o item foi modificado pela última vez. Somente leitura.
| **webUrl**               | string (url)     | A URL que exibe o item no navegador. Somente leitura.

## <a name="relationships"></a>Relações

O recurso **list** tem as seguintes relações com outros recursos.

| Nome da relação | Tipo                        | Descrição
|:------------------|:----------------------------|:------------------------------
| **activities**    | Conjunto [itemActivity][] | As atividades recentes que ocorreram nesta lista.
| **drive**         | [drive][]                   | Presente apenas em bibliotecas de documentos. Permite o acesso à lista como um recurso [drive][] com [driveItems][driveItem].
| **items**         | Collection([listItem][])    | Todos os itens contidos na lista.
| assinaturas      | conjunto de [assinaturas][] | O conjunto de assinaturas na lista.
|**operations**|Coleção [richLongRunningOperation](../resources/richlongrunningoperation.md)| A coleção de operações em execução longa para a lista.

[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[driveItem]: driveitem.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[site]: site.md
[systemFacet]: systemfacet.md
[assinatura]: subscription.md

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.list",
       "keyProperty": "id", 
       "optionalProperties": [ "items", "drive"] } -->

```json
{
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "displayName": "title of list",
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "items": [ { "@odata.type": "microsoft.graph.listItem" } ],
  "list": {
    "@odata.type": "microsoft.graph.listInfo",
    "hidden": false,
    "template&quot;: &quot;documentLibrary | genericList | survey | links | announcements | contacts ..."
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
  "webUrl&quot;: &quot;url to visit the list in a browser"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Lists",
  "tocBookmarks": {
    "Lists&quot;: &quot;#"
  },
  "suppressions": []
}
-->


