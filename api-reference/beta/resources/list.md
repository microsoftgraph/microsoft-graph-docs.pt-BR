---
author: JeremyKelley
description: O recurso de lista representa uma lista em um site.
ms.date: 09/11/2017
title: Listar
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 9bc255a0bcddadbbf9190decc2d429eb88e91e67
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964552"
---
# <a name="list-resource"></a><span data-ttu-id="ffec1-103">Recurso List</span><span class="sxs-lookup"><span data-stu-id="ffec1-103">List resource</span></span>

<span data-ttu-id="ffec1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffec1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ffec1-105">O recurso **list** representa uma lista em um [site][].</span><span class="sxs-lookup"><span data-stu-id="ffec1-105">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="ffec1-106">Este recurso contém as propriedades de nível superior da lista, incluindo definições de modelo e campo.</span><span class="sxs-lookup"><span data-stu-id="ffec1-106">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="ffec1-107">Tarefas em list</span><span class="sxs-lookup"><span data-stu-id="ffec1-107">Tasks on a list</span></span>

<span data-ttu-id="ffec1-108">As tarefas a seguir estão disponíveis para os recursos list.</span><span class="sxs-lookup"><span data-stu-id="ffec1-108">The following tasks are available for list resources.</span></span>
<span data-ttu-id="ffec1-109">**Observação:** esta versão beta só permite navegar por listas, não criar ou atualizá-las.</span><span class="sxs-lookup"><span data-stu-id="ffec1-109">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="ffec1-110">Você pode, no entanto, criar ou atualizar [itens de lista][listItem].</span><span class="sxs-lookup"><span data-stu-id="ffec1-110">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="ffec1-111">Todos os exemplos a seguir referem-se a um site: `https://graph.microsoft.com/beta/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="ffec1-111">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="ffec1-112">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="ffec1-112">Common task</span></span>               | <span data-ttu-id="ffec1-113">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="ffec1-113">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="ffec1-114">[Obter listas em um site][]</span><span class="sxs-lookup"><span data-stu-id="ffec1-114">[Get lists in a site][]</span></span>   | <span data-ttu-id="ffec1-115">GET /sites/{site-id}/lists</span><span class="sxs-lookup"><span data-stu-id="ffec1-115">GET /sites/{site-id}/lists</span></span>
| <span data-ttu-id="ffec1-116">[Criar lista][]</span><span class="sxs-lookup"><span data-stu-id="ffec1-116">[Create list][]</span></span>           | <span data-ttu-id="ffec1-117">POSTAR/listas</span><span class="sxs-lookup"><span data-stu-id="ffec1-117">POST /lists</span></span>
| <span data-ttu-id="ffec1-118">[Obter lista][]</span><span class="sxs-lookup"><span data-stu-id="ffec1-118">[Get list][]</span></span>              | <span data-ttu-id="ffec1-119">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="ffec1-119">GET /lists/{list-id}</span></span>
| <span data-ttu-id="ffec1-120">[Enumerar itens de lista][]</span><span class="sxs-lookup"><span data-stu-id="ffec1-120">[Enumerate list items][]</span></span>  | <span data-ttu-id="ffec1-121">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="ffec1-121">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="ffec1-122">[Atualizar item de lista][]</span><span class="sxs-lookup"><span data-stu-id="ffec1-122">[Update list item][]</span></span>      | <span data-ttu-id="ffec1-123">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="ffec1-123">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="ffec1-124">[Excluir item de lista][]</span><span class="sxs-lookup"><span data-stu-id="ffec1-124">[Delete list item][]</span></span>      | <span data-ttu-id="ffec1-125">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="ffec1-125">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="ffec1-126">[Criar item de lista][]</span><span class="sxs-lookup"><span data-stu-id="ffec1-126">[Create list item][]</span></span>      | <span data-ttu-id="ffec1-127">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="ffec1-127">POST /lists/{list-id}</span></span>
| <span data-ttu-id="ffec1-128">[Obter atividades recentes][]</span><span class="sxs-lookup"><span data-stu-id="ffec1-128">[Get recent activities][]</span></span> | <span data-ttu-id="ffec1-129">GET /lists/{list-id}/activities</span><span class="sxs-lookup"><span data-stu-id="ffec1-129">GET /lists/{list-id}/activities</span></span>
| <span data-ttu-id="ffec1-130">[Obter canal WebSocket][]</span><span class="sxs-lookup"><span data-stu-id="ffec1-130">[Get WebSocket channel][]</span></span> | <span data-ttu-id="ffec1-131">GET /lists/{list-id}/subscriptions/socketIo</span><span class="sxs-lookup"><span data-stu-id="ffec1-131">GET /lists/{list-id}/subscriptions/socketIo</span></span>
|<span data-ttu-id="ffec1-132">[Listar tipos de conteúdo][]</span><span class="sxs-lookup"><span data-stu-id="ffec1-132">[List content types][]</span></span>          | <span data-ttu-id="ffec1-133">GET /lists/{list-id}/contentTypes</span><span class="sxs-lookup"><span data-stu-id="ffec1-133">GET /lists/{list-id}/contentTypes</span></span>
|<span data-ttu-id="ffec1-134">[Adicionar cópia do tipo de conteúdo do site][]</span><span class="sxs-lookup"><span data-stu-id="ffec1-134">[Add copy of content type from site][]</span></span> | <span data-ttu-id="ffec1-135">POST /lists/{list-id}/contentTypes/addCopy</span><span class="sxs-lookup"><span data-stu-id="ffec1-135">POST /lists/{list-id}/contentTypes/addCopy</span></span>
|<span data-ttu-id="ffec1-136">[List columns][]</span><span class="sxs-lookup"><span data-stu-id="ffec1-136">[List columns][]</span></span>               | <span data-ttu-id="ffec1-137">GET /lists/{list-id}/columns</span><span class="sxs-lookup"><span data-stu-id="ffec1-137">GET /lists/{list-id}/columns</span></span>
|<span data-ttu-id="ffec1-138">[Criar coluna][]</span><span class="sxs-lookup"><span data-stu-id="ffec1-138">[Create column][]</span></span>              | <span data-ttu-id="ffec1-139">POST /lists/{list-id}/columns</span><span class="sxs-lookup"><span data-stu-id="ffec1-139">POST /lists/{list-id}/columns</span></span>

[Obter listas em um site]: ../api/list-list.md
[Get lists in a site]: ../api/list-list.md
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
[Obter atividades recentes]: ../api/activities-list.md
[Get recent activities]: ../api/activities-list.md
[Obter canal WebSocket]: ../api/subscriptions-socketio.md
[Get WebSocket channel]: ../api/subscriptions-socketio.md
[Listar tipos de conteúdo]: ../api/list-list-contenttypes.md
[List content types]: ../api/list-list-contenttypes.md
[Adicionar cópia do tipo de conteúdo do site]: ../api/contenttype-addCopy.md
[Add copy of content type from site]: ../api/contenttype-addCopy.md
[List columns]: ../api/list-list-columns.md
[Criar coluna]: ../api/list-post-columns.md
[Create column]: ../api/list-post-columns.md
## <a name="json-representation"></a><span data-ttu-id="ffec1-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ffec1-153">JSON representation</span></span>

<span data-ttu-id="ffec1-154">Veja a seguir uma representação JSON de um recurso **list**.</span><span class="sxs-lookup"><span data-stu-id="ffec1-154">Here is a JSON representation of a **list** resource.</span></span>

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
    "template": "documentLibrary | genericList | survey | links | announcements | contacts ..."
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
  "webUrl": "url to visit the list in a browser"
}
```

## <a name="properties"></a><span data-ttu-id="ffec1-155">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ffec1-155">Properties</span></span>

<span data-ttu-id="ffec1-156">O recurso **list** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="ffec1-156">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="ffec1-157">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="ffec1-157">Property name</span></span>    | <span data-ttu-id="ffec1-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="ffec1-158">Type</span></span>                             | <span data-ttu-id="ffec1-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="ffec1-159">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="ffec1-160">**columns**</span><span class="sxs-lookup"><span data-stu-id="ffec1-160">**columns**</span></span>      | <span data-ttu-id="ffec1-161">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="ffec1-161">Collection([columnDefinition][])</span></span> | <span data-ttu-id="ffec1-162">A coleção de definições de campo para esta lista.</span><span class="sxs-lookup"><span data-stu-id="ffec1-162">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="ffec1-163">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="ffec1-163">**contentTypes**</span></span> | <span data-ttu-id="ffec1-164">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="ffec1-164">Collection([contentType][])</span></span>      | <span data-ttu-id="ffec1-165">A coleção de tipos de conteúdo presentes nesta lista.</span><span class="sxs-lookup"><span data-stu-id="ffec1-165">The collection of content types present in this list.</span></span>
| <span data-ttu-id="ffec1-166">**displayName**</span><span class="sxs-lookup"><span data-stu-id="ffec1-166">**displayName**</span></span>  | <span data-ttu-id="ffec1-167">string</span><span class="sxs-lookup"><span data-stu-id="ffec1-167">string</span></span>                           | <span data-ttu-id="ffec1-168">O título em exibição da lista.</span><span class="sxs-lookup"><span data-stu-id="ffec1-168">The displayable title of the list.</span></span>
| <span data-ttu-id="ffec1-169">**list**</span><span class="sxs-lookup"><span data-stu-id="ffec1-169">**list**</span></span>         | <span data-ttu-id="ffec1-170">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="ffec1-170">[listInfo][]</span></span>                     | <span data-ttu-id="ffec1-171">Fornece mais detalhes sobre a lista.</span><span class="sxs-lookup"><span data-stu-id="ffec1-171">Provides additional details about the list.</span></span>
| <span data-ttu-id="ffec1-172">**system**</span><span class="sxs-lookup"><span data-stu-id="ffec1-172">**system**</span></span>       | <span data-ttu-id="ffec1-173">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="ffec1-173">[systemFacet][]</span></span>                  | <span data-ttu-id="ffec1-174">Se estiver presente, indica que se trata de uma lista gerenciada pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="ffec1-174">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="ffec1-175">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ffec1-175">Read-only.</span></span>

<span data-ttu-id="ffec1-176">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="ffec1-176">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="ffec1-177">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="ffec1-177">Property name</span></span>            | <span data-ttu-id="ffec1-178">Tipo</span><span class="sxs-lookup"><span data-stu-id="ffec1-178">Type</span></span>             | <span data-ttu-id="ffec1-179">Descrição</span><span class="sxs-lookup"><span data-stu-id="ffec1-179">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="ffec1-180">**id**</span><span class="sxs-lookup"><span data-stu-id="ffec1-180">**id**</span></span>                   | <span data-ttu-id="ffec1-181">string</span><span class="sxs-lookup"><span data-stu-id="ffec1-181">string</span></span>           | <span data-ttu-id="ffec1-p104">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ffec1-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="ffec1-184">**name**</span><span class="sxs-lookup"><span data-stu-id="ffec1-184">**name**</span></span>                 | <span data-ttu-id="ffec1-185">string</span><span class="sxs-lookup"><span data-stu-id="ffec1-185">string</span></span>           | <span data-ttu-id="ffec1-186">O nome do item.</span><span class="sxs-lookup"><span data-stu-id="ffec1-186">The name of the item.</span></span>
| <span data-ttu-id="ffec1-187">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="ffec1-187">**createdBy**</span></span>            | <span data-ttu-id="ffec1-188">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ffec1-188">[identitySet][]</span></span>  | <span data-ttu-id="ffec1-189">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="ffec1-189">Identity of the creator of this item.</span></span> <span data-ttu-id="ffec1-190">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ffec1-190">Read-only.</span></span>
| <span data-ttu-id="ffec1-191">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="ffec1-191">**createdDateTime**</span></span>      | <span data-ttu-id="ffec1-192">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffec1-192">DateTimeOffset</span></span>   | <span data-ttu-id="ffec1-p106">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ffec1-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="ffec1-195">**description**</span><span class="sxs-lookup"><span data-stu-id="ffec1-195">**description**</span></span>          | <span data-ttu-id="ffec1-196">string</span><span class="sxs-lookup"><span data-stu-id="ffec1-196">string</span></span>           | <span data-ttu-id="ffec1-197">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="ffec1-197">The descriptive text for the item.</span></span>
| <span data-ttu-id="ffec1-198">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="ffec1-198">**lastModifiedBy**</span></span>       | <span data-ttu-id="ffec1-199">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ffec1-199">[identitySet][]</span></span>  | <span data-ttu-id="ffec1-200">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="ffec1-200">Identity of the last modifier of this item.</span></span> <span data-ttu-id="ffec1-201">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ffec1-201">Read-only.</span></span>
| <span data-ttu-id="ffec1-202">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="ffec1-202">**lastModifiedDateTime**</span></span> | <span data-ttu-id="ffec1-203">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffec1-203">DateTimeOffset</span></span>   | <span data-ttu-id="ffec1-p108">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ffec1-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="ffec1-206">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="ffec1-206">**webUrl**</span></span>               | <span data-ttu-id="ffec1-207">string (url)</span><span class="sxs-lookup"><span data-stu-id="ffec1-207">string (url)</span></span>     | <span data-ttu-id="ffec1-p109">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ffec1-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="ffec1-210">Relações</span><span class="sxs-lookup"><span data-stu-id="ffec1-210">Relationships</span></span>

<span data-ttu-id="ffec1-211">O recurso **list** tem as seguintes relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="ffec1-211">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="ffec1-212">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="ffec1-212">Relationship name</span></span> | <span data-ttu-id="ffec1-213">Tipo</span><span class="sxs-lookup"><span data-stu-id="ffec1-213">Type</span></span>                        | <span data-ttu-id="ffec1-214">Descrição</span><span class="sxs-lookup"><span data-stu-id="ffec1-214">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="ffec1-215">**activities**</span><span class="sxs-lookup"><span data-stu-id="ffec1-215">**activities**</span></span>    | <span data-ttu-id="ffec1-216">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="ffec1-216">[itemActivity][] collection</span></span> | <span data-ttu-id="ffec1-217">As atividades recentes que ocorreram nesta lista.</span><span class="sxs-lookup"><span data-stu-id="ffec1-217">The recent activities that took place within this list.</span></span>
| <span data-ttu-id="ffec1-218">**drive**</span><span class="sxs-lookup"><span data-stu-id="ffec1-218">**drive**</span></span>         | <span data-ttu-id="ffec1-219">[drive][]</span><span class="sxs-lookup"><span data-stu-id="ffec1-219">[drive][]</span></span>                   | <span data-ttu-id="ffec1-220">Presente somente em bibliotecas de documentos.</span><span class="sxs-lookup"><span data-stu-id="ffec1-220">Only present on document libraries.</span></span> <span data-ttu-id="ffec1-221">Permite o acesso à lista como um recurso de [unidade][] com [driveItems][driveItem].</span><span class="sxs-lookup"><span data-stu-id="ffec1-221">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="ffec1-222">**items**</span><span class="sxs-lookup"><span data-stu-id="ffec1-222">**items**</span></span>         | <span data-ttu-id="ffec1-223">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="ffec1-223">Collection([listItem][])</span></span>    | <span data-ttu-id="ffec1-224">Todos os itens contidos na lista.</span><span class="sxs-lookup"><span data-stu-id="ffec1-224">All items contained in the list.</span></span>
| <span data-ttu-id="ffec1-225">assinaturas</span><span class="sxs-lookup"><span data-stu-id="ffec1-225">subscriptions</span></span>      | <span data-ttu-id="ffec1-226">conjunto de [assinaturas][]</span><span class="sxs-lookup"><span data-stu-id="ffec1-226">[subscription][] collection</span></span> | <span data-ttu-id="ffec1-227">O conjunto de assinaturas na lista.</span><span class="sxs-lookup"><span data-stu-id="ffec1-227">The set of subscriptions on the list.</span></span>

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
[subscription]: subscription.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Lists",
  "tocBookmarks": {
    "Lists": "#"
  },
  "suppressions": []
}
-->


