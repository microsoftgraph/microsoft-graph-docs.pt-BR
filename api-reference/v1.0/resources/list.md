---
author: JeremyKelley
ms.date: 09/11/2017
title: Listar
localization_priority: Priority
ms.prod: sharepoint
description: O recurso de lista representa uma lista em um site.
doc_type: resourcePageType
ms.openlocfilehash: 0f7c8600b8a4d8f41e6dd6e6ad4240252c004bbf
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317004"
---
# <a name="list-resource"></a><span data-ttu-id="e6ab0-103">Recurso List</span><span class="sxs-lookup"><span data-stu-id="e6ab0-103">List resource</span></span>

<span data-ttu-id="e6ab0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6ab0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e6ab0-105">O recurso **list** representa uma lista em um [site][].</span><span class="sxs-lookup"><span data-stu-id="e6ab0-105">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="e6ab0-106">Este recurso contém as propriedades de nível superior da lista, incluindo definições de modelo e campo.</span><span class="sxs-lookup"><span data-stu-id="e6ab0-106">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="e6ab0-107">Tarefas em list</span><span class="sxs-lookup"><span data-stu-id="e6ab0-107">Tasks on a list</span></span>

<span data-ttu-id="e6ab0-108">As tarefas a seguir estão disponíveis para os recursos list.</span><span class="sxs-lookup"><span data-stu-id="e6ab0-108">The following tasks are available for list resources.</span></span>
<span data-ttu-id="e6ab0-109">**Observação:** esta versão beta só permite navegar por listas, não criar ou atualizá-las.</span><span class="sxs-lookup"><span data-stu-id="e6ab0-109">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="e6ab0-110">Você pode, no entanto, criar ou atualizar [itens de lista][listItem].</span><span class="sxs-lookup"><span data-stu-id="e6ab0-110">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="e6ab0-111">Todos os exemplos abaixo são relativos a um site, por exemplo, `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="e6ab0-111">All examples below are relative to a site, for example, `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span></span>

| <span data-ttu-id="e6ab0-112">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="e6ab0-112">Common task</span></span>               | <span data-ttu-id="e6ab0-113">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="e6ab0-113">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="e6ab0-114">[Obter lista][]</span><span class="sxs-lookup"><span data-stu-id="e6ab0-114">[Get list][]</span></span>              | <span data-ttu-id="e6ab0-115">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="e6ab0-115">GET /lists/{list-id}</span></span>
| <span data-ttu-id="e6ab0-116">[Criar lista][]</span><span class="sxs-lookup"><span data-stu-id="e6ab0-116">[Create list][]</span></span>           | <span data-ttu-id="e6ab0-117">POSTAR/listas</span><span class="sxs-lookup"><span data-stu-id="e6ab0-117">POST /lists</span></span>
| <span data-ttu-id="e6ab0-118">[Enumerar itens de lista][]</span><span class="sxs-lookup"><span data-stu-id="e6ab0-118">[Enumerate list items][]</span></span>  | <span data-ttu-id="e6ab0-119">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="e6ab0-119">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="e6ab0-120">[Atualizar item de lista][]</span><span class="sxs-lookup"><span data-stu-id="e6ab0-120">[Update list item][]</span></span>      | <span data-ttu-id="e6ab0-121">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="e6ab0-121">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="e6ab0-122">[Excluir item de lista][]</span><span class="sxs-lookup"><span data-stu-id="e6ab0-122">[Delete list item][]</span></span>      | <span data-ttu-id="e6ab0-123">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="e6ab0-123">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="e6ab0-124">[Criar item de lista][]</span><span class="sxs-lookup"><span data-stu-id="e6ab0-124">[Create list item][]</span></span>      | <span data-ttu-id="e6ab0-125">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="e6ab0-125">POST /lists/{list-id}</span></span>
| <span data-ttu-id="e6ab0-126">[Obter canal WebSocket][]</span><span class="sxs-lookup"><span data-stu-id="e6ab0-126">[Get WebSocket channel][]</span></span> | <span data-ttu-id="e6ab0-127">GET /lists/{list-id}/subscriptions/socketIo</span><span class="sxs-lookup"><span data-stu-id="e6ab0-127">GET /lists/{list-id}/subscriptions/socketIo</span></span>

[Obter lista]: ../api/list-get.md
[Get list]: ../api/list-get.md
[Criar lista]: ../api/list-create.md
[Create list]: ../api/list-create.md
[Enumerar itens de lista]: ../api/listitem-list.md
[Enumerate list items]: ../api/listitem-list.md
[Atualizar item de lista]: ../api/listitem-update.md
[Update list item]: ../api/listitem-update.md
[Excluir item de lista]: ../api/listitem-delete.md
[Delete list item]: ../api/listitem-delete.md
[Criar item de lista]: ../api/listitem-create.md
[Create list item]: ../api/listitem-create.md
[Obter canal WebSocket]: ../api/subscriptions-socketio.md
[Get WebSocket channel]: ../api/subscriptions-socketio.md

## <a name="json-representation"></a><span data-ttu-id="e6ab0-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e6ab0-135">JSON representation</span></span>

<span data-ttu-id="e6ab0-136">Veja a seguir uma representação JSON de um recurso **list**.</span><span class="sxs-lookup"><span data-stu-id="e6ab0-136">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="e6ab0-137">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e6ab0-137">Properties</span></span>

<span data-ttu-id="e6ab0-138">O recurso **list** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="e6ab0-138">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="e6ab0-139">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="e6ab0-139">Property name</span></span>    | <span data-ttu-id="e6ab0-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6ab0-140">Type</span></span>                             | <span data-ttu-id="e6ab0-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6ab0-141">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="e6ab0-142">**displayName**</span><span class="sxs-lookup"><span data-stu-id="e6ab0-142">**displayName**</span></span>  | <span data-ttu-id="e6ab0-143">string</span><span class="sxs-lookup"><span data-stu-id="e6ab0-143">string</span></span>                           | <span data-ttu-id="e6ab0-144">O título em exibição da lista.</span><span class="sxs-lookup"><span data-stu-id="e6ab0-144">The displayable title of the list.</span></span>
| <span data-ttu-id="e6ab0-145">**list**</span><span class="sxs-lookup"><span data-stu-id="e6ab0-145">**list**</span></span>         | <span data-ttu-id="e6ab0-146">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="e6ab0-146">[listInfo][]</span></span>                     | <span data-ttu-id="e6ab0-147">Fornece mais detalhes sobre a lista.</span><span class="sxs-lookup"><span data-stu-id="e6ab0-147">Provides additional details about the list.</span></span>
| <span data-ttu-id="e6ab0-148">**system**</span><span class="sxs-lookup"><span data-stu-id="e6ab0-148">**system**</span></span>       | <span data-ttu-id="e6ab0-149">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="e6ab0-149">[systemFacet][]</span></span>                  | <span data-ttu-id="e6ab0-p103">Se presente, indica que esta é uma lista gerenciada pelo sistema. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6ab0-p103">If present, indicates that this is a system-managed list. Read-only.</span></span>

<span data-ttu-id="e6ab0-152">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="e6ab0-152">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="e6ab0-153">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="e6ab0-153">Property name</span></span>            | <span data-ttu-id="e6ab0-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6ab0-154">Type</span></span>              | <span data-ttu-id="e6ab0-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6ab0-155">Description</span></span>
|:-------------------------|:------------------|:------------------------------
| <span data-ttu-id="e6ab0-156">**id**</span><span class="sxs-lookup"><span data-stu-id="e6ab0-156">**id**</span></span>                   | <span data-ttu-id="e6ab0-157">string</span><span class="sxs-lookup"><span data-stu-id="e6ab0-157">string</span></span>            | <span data-ttu-id="e6ab0-p104">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6ab0-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="e6ab0-160">**name**</span><span class="sxs-lookup"><span data-stu-id="e6ab0-160">**name**</span></span>                 | <span data-ttu-id="e6ab0-161">string</span><span class="sxs-lookup"><span data-stu-id="e6ab0-161">string</span></span>            | <span data-ttu-id="e6ab0-162">O nome do item.</span><span class="sxs-lookup"><span data-stu-id="e6ab0-162">The name of the item.</span></span>
| <span data-ttu-id="e6ab0-163">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="e6ab0-163">**createdBy**</span></span>            | <span data-ttu-id="e6ab0-164">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="e6ab0-164">[identitySet][]</span></span>   | <span data-ttu-id="e6ab0-p105">Identidade do criador deste item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6ab0-p105">Identity of the creator of this item. Read-only.</span></span>
| <span data-ttu-id="e6ab0-167">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="e6ab0-167">**createdDateTime**</span></span>      | <span data-ttu-id="e6ab0-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6ab0-168">DateTimeOffset</span></span>    | <span data-ttu-id="e6ab0-p106">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6ab0-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="e6ab0-171">**description**</span><span class="sxs-lookup"><span data-stu-id="e6ab0-171">**description**</span></span>          | <span data-ttu-id="e6ab0-172">string</span><span class="sxs-lookup"><span data-stu-id="e6ab0-172">string</span></span>            | <span data-ttu-id="e6ab0-173">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="e6ab0-173">The descriptive text for the item.</span></span>
| <span data-ttu-id="e6ab0-174">**eTag**</span><span class="sxs-lookup"><span data-stu-id="e6ab0-174">**eTag**</span></span>                 | <span data-ttu-id="e6ab0-175">string</span><span class="sxs-lookup"><span data-stu-id="e6ab0-175">string</span></span>            | <span data-ttu-id="e6ab0-p107">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6ab0-p107">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="e6ab0-178">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="e6ab0-178">**lastModifiedBy**</span></span>       | <span data-ttu-id="e6ab0-179">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="e6ab0-179">[identitySet][]</span></span>   | <span data-ttu-id="e6ab0-p108">Identidade do último modificador deste item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6ab0-p108">Identity of the last modifier of this item. Read-only.</span></span>
| <span data-ttu-id="e6ab0-182">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="e6ab0-182">**lastModifiedDateTime**</span></span> | <span data-ttu-id="e6ab0-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6ab0-183">DateTimeOffset</span></span>    | <span data-ttu-id="e6ab0-p109">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6ab0-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="e6ab0-186">**parentReference**</span><span class="sxs-lookup"><span data-stu-id="e6ab0-186">**parentReference**</span></span>      | <span data-ttu-id="e6ab0-187">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="e6ab0-187">[itemReference][]</span></span> | <span data-ttu-id="e6ab0-p110">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="e6ab0-p110">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="e6ab0-190">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="e6ab0-190">**sharepointIds**</span></span>        | <span data-ttu-id="e6ab0-191">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="e6ab0-191">[sharepointIds][]</span></span> | <span data-ttu-id="e6ab0-p111">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6ab0-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="e6ab0-194">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="e6ab0-194">**webUrl**</span></span>               | <span data-ttu-id="e6ab0-195">string (url)</span><span class="sxs-lookup"><span data-stu-id="e6ab0-195">string (url)</span></span>      | <span data-ttu-id="e6ab0-p112">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6ab0-p112">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="e6ab0-198">Relações</span><span class="sxs-lookup"><span data-stu-id="e6ab0-198">Relationships</span></span>

<span data-ttu-id="e6ab0-199">O recurso **list** tem as seguintes relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="e6ab0-199">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="e6ab0-200">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="e6ab0-200">Relationship name</span></span> | <span data-ttu-id="e6ab0-201">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6ab0-201">Type</span></span>                             | <span data-ttu-id="e6ab0-202">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6ab0-202">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="e6ab0-203">**drive**</span><span class="sxs-lookup"><span data-stu-id="e6ab0-203">**drive**</span></span>         | <span data-ttu-id="e6ab0-204">[drive][]</span><span class="sxs-lookup"><span data-stu-id="e6ab0-204">[drive][]</span></span>                        | <span data-ttu-id="e6ab0-205">Presente somente em bibliotecas de documentos.</span><span class="sxs-lookup"><span data-stu-id="e6ab0-205">Only present on document libraries.</span></span> <span data-ttu-id="e6ab0-206">Permite o acesso à lista como um recurso de [unidade][] com [driveItems][driveItem].</span><span class="sxs-lookup"><span data-stu-id="e6ab0-206">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="e6ab0-207">**items**</span><span class="sxs-lookup"><span data-stu-id="e6ab0-207">**items**</span></span>         | <span data-ttu-id="e6ab0-208">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="e6ab0-208">Collection([listItem][])</span></span>         | <span data-ttu-id="e6ab0-209">Todos os itens contidos na lista.</span><span class="sxs-lookup"><span data-stu-id="e6ab0-209">All items contained in the list.</span></span>
| <span data-ttu-id="e6ab0-210">**columns**</span><span class="sxs-lookup"><span data-stu-id="e6ab0-210">**columns**</span></span>       | <span data-ttu-id="e6ab0-211">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="e6ab0-211">Collection([columnDefinition][])</span></span> | <span data-ttu-id="e6ab0-212">A coleção de definições de campo para esta lista.</span><span class="sxs-lookup"><span data-stu-id="e6ab0-212">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="e6ab0-213">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="e6ab0-213">**contentTypes**</span></span>  | <span data-ttu-id="e6ab0-214">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="e6ab0-214">Collection([contentType][])</span></span>      | <span data-ttu-id="e6ab0-215">A coleção de tipos de conteúdo presentes nesta lista.</span><span class="sxs-lookup"><span data-stu-id="e6ab0-215">The collection of content types present in this list.</span></span>
| <span data-ttu-id="e6ab0-216">**assinaturas**</span><span class="sxs-lookup"><span data-stu-id="e6ab0-216">**subscriptions**</span></span> | <span data-ttu-id="e6ab0-217">Conjunto([assinatura][])</span><span class="sxs-lookup"><span data-stu-id="e6ab0-217">Collection([subscription][])</span></span>     | <span data-ttu-id="e6ab0-218">O conjunto de assinaturas na lista.</span><span class="sxs-lookup"><span data-stu-id="e6ab0-218">The set of subscriptions on the list.</span></span>

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
[subscription]: subscription.md

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

