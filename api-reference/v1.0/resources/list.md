---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Listar
ms.openlocfilehash: ba0c01ce1887a32bd8b671cf511104e9128b5efb
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="list-resource"></a>Recurso List

O recurso **list** representa uma lista em um [site][].
Este recurso contém as propriedades de nível superior da lista, incluindo definições de modelo e campo.

## <a name="tasks-on-a-list"></a>Tarefas em list

As tarefas a seguir estão disponíveis para os recursos list.
**Observação:** esta versão beta só permite navegar por listas, não criar ou atualizá-las.
Você pode, no entanto, criar ou atualizar [itens de lista][listItem].

Todos os exemplos a seguir referem-se a um site: `https://graph.microsoft.com/beta/sites/{site-id}`.

| Tarefa comum               | Método HTTP
|:--------------------------|:------------------------------
| [Obter lista][]              | GET /lists/{list-id}
| [Enumerar itens de lista][]  | GET /lists/{list-id}/items
| [Atualizar item de lista][]      | PATCH /lists/{list-id}/items/{item-id}
| [Excluir item de lista][]      | DELETE /lists/{list-id}/items/{item-id}
| [Criar item de lista][]      | POST /lists/{list-id}

[Obter lista]: ../api/list_get.md
[Enumerar itens de lista]: ../api/listitem_list.md
[Atualizar item de lista]: ../api/listItem_update.md
[Excluir item de lista]: ../api/listItem_delete.md
[Criar item de lista]: ../api/listItem_create.md

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON de um recurso **list**.

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.list",
       "keyProperty": "id", 
       "optionalProperties": [ "items", "drive"] } -->

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
    "template": "documentLibrary | genericList | survey | links | announcements | contacts ..."
  },
  "system": false,

  /* inherited from baseItem */
  "id": "string",
  "name": "name of list",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of list",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "webUrl": "url to visit the list in a browser"
}
```

## <a name="properties"></a>Propriedades

O recurso **list** tem as seguintes propriedades.

| Nome da propriedade    | Tipo                             | Descrição
|:-----------------|:---------------------------------|:---------------------------
| **columns**      | Collection([columnDefinition][]) | A coleção de definições de campo para esta lista.
| **contentTypes** | Collection([contentType][])      | A coleção de tipos de conteúdo presentes nesta lista.
| **displayName**  | string                           | O título em exibição da lista.
| **list**         | [listInfo][]                     | Fornece mais detalhes sobre a lista.
| **system**       | [systemFacet][]                  | Se estiver presente, indica que se trata de uma lista gerenciada pelo sistema. Somente leitura.

As propriedades a seguir são herdadas do **[baseItem][]**.

| Nome da propriedade            | Tipo             | Descrição
|:-------------------------|:-----------------|:-------------------------------
| **id**                   | string           | O identificador exclusivo do item. Somente leitura.
| **name**                 | string           | O nome do item.
| **createdBy**            | [identitySet][]  | Identidade do criador desse item. Somente leitura.
| **createdDateTime**      | DateTimeOffset   | A data e a hora da criação do item. Somente leitura.
| **description**          | string           | O texto descritivo do item.
| **lastModifiedBy**       | [identitySet][]  | Identidade da última pessoa que alterou esse item. Somente leitura.
| **lastModifiedDateTime** | DateTimeOffset   | A data e a hora que o item foi modificado pela última vez. Somente leitura.
| **webUrl**               | string (url)     | A URL que exibe o item no navegador. Somente leitura.

## <a name="relationships"></a>Relações

O recurso **list** tem as seguintes relações com outros recursos.

| Nome da relação | Tipo                        | Descrição
|:------------------|:----------------------------|:------------------------------
| **drive**         | [drive][]                   | Presente somente em bibliotecas de documentos. Permite o acesso à lista como um recurso [drive][] com [driveItems][driveItem].
| **items**         | Collection([listItem][])    | Todos os itens contidos na lista.

[baseItem]: baseItem.md
[contentType]: contentType.md
[drive]: drive.md
[driveItem]: driveItem.md
[columnDefinition]: columnDefinition.md
[identitySet]: identitySet.md
[listInfo]: listInfo.md
[listItem]: listItem.md
[site]: site.md
[systemFacet]: systemFacet.md

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
