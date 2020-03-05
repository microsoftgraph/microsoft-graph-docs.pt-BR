---
author: JeremyKelley
description: O recurso de lista representa uma lista em um site.
ms.date: 09/11/2017
title: Listar
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: a7e59cf2e81371428e3816acc6e89c4a102ca40e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522957"
---
# <a name="list-resource"></a><span data-ttu-id="dc20a-103">Recurso List</span><span class="sxs-lookup"><span data-stu-id="dc20a-103">List resource</span></span>

<span data-ttu-id="dc20a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dc20a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc20a-105">O recurso **list** representa uma lista em um [site][].</span><span class="sxs-lookup"><span data-stu-id="dc20a-105">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="dc20a-106">Este recurso contém as propriedades de nível superior da lista, incluindo definições de modelo e campo.</span><span class="sxs-lookup"><span data-stu-id="dc20a-106">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="dc20a-107">Tarefas em list</span><span class="sxs-lookup"><span data-stu-id="dc20a-107">Tasks on a list</span></span>

<span data-ttu-id="dc20a-108">As tarefas a seguir estão disponíveis para os recursos list.</span><span class="sxs-lookup"><span data-stu-id="dc20a-108">The following tasks are available for list resources.</span></span>
<span data-ttu-id="dc20a-109">**Observação:** esta versão beta só permite navegar por listas, não criar ou atualizá-las.</span><span class="sxs-lookup"><span data-stu-id="dc20a-109">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="dc20a-110">Você pode, no entanto, criar ou atualizar [itens de lista][listItem].</span><span class="sxs-lookup"><span data-stu-id="dc20a-110">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="dc20a-111">Todos os exemplos a seguir referem-se a um site: `https://graph.microsoft.com/beta/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="dc20a-111">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="dc20a-112">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="dc20a-112">Common task</span></span>               | <span data-ttu-id="dc20a-113">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="dc20a-113">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="dc20a-114">[Obter lista][]</span><span class="sxs-lookup"><span data-stu-id="dc20a-114">[Get list][]</span></span>              | <span data-ttu-id="dc20a-115">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="dc20a-115">GET /lists/{list-id}</span></span>
| <span data-ttu-id="dc20a-116">[Criar lista][]</span><span class="sxs-lookup"><span data-stu-id="dc20a-116">[Create list][]</span></span>           | <span data-ttu-id="dc20a-117">POSTAR/listas</span><span class="sxs-lookup"><span data-stu-id="dc20a-117">POST /lists</span></span>
| <span data-ttu-id="dc20a-118">[Enumerar itens de lista][]</span><span class="sxs-lookup"><span data-stu-id="dc20a-118">[Enumerate list items][]</span></span>  | <span data-ttu-id="dc20a-119">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="dc20a-119">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="dc20a-120">[Atualizar item de lista][]</span><span class="sxs-lookup"><span data-stu-id="dc20a-120">[Update list item][]</span></span>      | <span data-ttu-id="dc20a-121">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="dc20a-121">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="dc20a-122">[Excluir item de lista][]</span><span class="sxs-lookup"><span data-stu-id="dc20a-122">[Delete list item][]</span></span>      | <span data-ttu-id="dc20a-123">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="dc20a-123">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="dc20a-124">[Criar item de lista][]</span><span class="sxs-lookup"><span data-stu-id="dc20a-124">[Create list item][]</span></span>      | <span data-ttu-id="dc20a-125">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="dc20a-125">POST /lists/{list-id}</span></span>
| <span data-ttu-id="dc20a-126">[Obter atividades recentes][]</span><span class="sxs-lookup"><span data-stu-id="dc20a-126">[Get recent activities][]</span></span> | <span data-ttu-id="dc20a-127">GET /lists/{list-id}/activities</span><span class="sxs-lookup"><span data-stu-id="dc20a-127">GET /lists/{list-id}/activities</span></span>
| <span data-ttu-id="dc20a-128">[Obter canal WebSocket][]</span><span class="sxs-lookup"><span data-stu-id="dc20a-128">[Get WebSocket channel][]</span></span> | <span data-ttu-id="dc20a-129">OBTER/lists/{list-id}/subscriptions/socketIo</span><span class="sxs-lookup"><span data-stu-id="dc20a-129">GET /lists/{list-id}/subscriptions/socketIo</span></span>

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
[Obter canal WebSocket]: ../api/driveitem-subscriptions-socketio.md
[Get WebSocket channel]: ../api/driveitem-subscriptions-socketio.md

## <a name="json-representation"></a><span data-ttu-id="dc20a-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dc20a-138">JSON representation</span></span>

<span data-ttu-id="dc20a-139">Veja a seguir uma representação JSON de um recurso **list**.</span><span class="sxs-lookup"><span data-stu-id="dc20a-139">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="dc20a-140">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dc20a-140">Properties</span></span>

<span data-ttu-id="dc20a-141">O recurso **list** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="dc20a-141">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="dc20a-142">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="dc20a-142">Property name</span></span>    | <span data-ttu-id="dc20a-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc20a-143">Type</span></span>                             | <span data-ttu-id="dc20a-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc20a-144">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="dc20a-145">**columns**</span><span class="sxs-lookup"><span data-stu-id="dc20a-145">**columns**</span></span>      | <span data-ttu-id="dc20a-146">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="dc20a-146">Collection([columnDefinition][])</span></span> | <span data-ttu-id="dc20a-147">A coleção de definições de campo para esta lista.</span><span class="sxs-lookup"><span data-stu-id="dc20a-147">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="dc20a-148">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="dc20a-148">**contentTypes**</span></span> | <span data-ttu-id="dc20a-149">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="dc20a-149">Collection([contentType][])</span></span>      | <span data-ttu-id="dc20a-150">A coleção de tipos de conteúdo presentes nesta lista.</span><span class="sxs-lookup"><span data-stu-id="dc20a-150">The collection of content types present in this list.</span></span>
| <span data-ttu-id="dc20a-151">**displayName**</span><span class="sxs-lookup"><span data-stu-id="dc20a-151">**displayName**</span></span>  | <span data-ttu-id="dc20a-152">string</span><span class="sxs-lookup"><span data-stu-id="dc20a-152">string</span></span>                           | <span data-ttu-id="dc20a-153">O título em exibição da lista.</span><span class="sxs-lookup"><span data-stu-id="dc20a-153">The displayable title of the list.</span></span>
| <span data-ttu-id="dc20a-154">**list**</span><span class="sxs-lookup"><span data-stu-id="dc20a-154">**list**</span></span>         | <span data-ttu-id="dc20a-155">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="dc20a-155">[listInfo][]</span></span>                     | <span data-ttu-id="dc20a-156">Fornece mais detalhes sobre a lista.</span><span class="sxs-lookup"><span data-stu-id="dc20a-156">Provides additional details about the list.</span></span>
| <span data-ttu-id="dc20a-157">**system**</span><span class="sxs-lookup"><span data-stu-id="dc20a-157">**system**</span></span>       | <span data-ttu-id="dc20a-158">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="dc20a-158">[systemFacet][]</span></span>                  | <span data-ttu-id="dc20a-159">Se estiver presente, indica que se trata de uma lista gerenciada pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="dc20a-159">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="dc20a-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dc20a-160">Read-only.</span></span>

<span data-ttu-id="dc20a-161">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="dc20a-161">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="dc20a-162">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="dc20a-162">Property name</span></span>            | <span data-ttu-id="dc20a-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc20a-163">Type</span></span>             | <span data-ttu-id="dc20a-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc20a-164">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="dc20a-165">**id**</span><span class="sxs-lookup"><span data-stu-id="dc20a-165">**id**</span></span>                   | <span data-ttu-id="dc20a-166">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc20a-166">string</span></span>           | <span data-ttu-id="dc20a-p104">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dc20a-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="dc20a-169">**name**</span><span class="sxs-lookup"><span data-stu-id="dc20a-169">**name**</span></span>                 | <span data-ttu-id="dc20a-170">string</span><span class="sxs-lookup"><span data-stu-id="dc20a-170">string</span></span>           | <span data-ttu-id="dc20a-171">O nome do item.</span><span class="sxs-lookup"><span data-stu-id="dc20a-171">The name of the item.</span></span>
| <span data-ttu-id="dc20a-172">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="dc20a-172">**createdBy**</span></span>            | <span data-ttu-id="dc20a-173">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="dc20a-173">[identitySet][]</span></span>  | <span data-ttu-id="dc20a-174">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="dc20a-174">Identity of the creator of this item.</span></span> <span data-ttu-id="dc20a-175">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dc20a-175">Read-only.</span></span>
| <span data-ttu-id="dc20a-176">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="dc20a-176">**createdDateTime**</span></span>      | <span data-ttu-id="dc20a-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc20a-177">DateTimeOffset</span></span>   | <span data-ttu-id="dc20a-p106">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dc20a-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="dc20a-180">**description**</span><span class="sxs-lookup"><span data-stu-id="dc20a-180">**description**</span></span>          | <span data-ttu-id="dc20a-181">string</span><span class="sxs-lookup"><span data-stu-id="dc20a-181">string</span></span>           | <span data-ttu-id="dc20a-182">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="dc20a-182">The descriptive text for the item.</span></span>
| <span data-ttu-id="dc20a-183">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="dc20a-183">**lastModifiedBy**</span></span>       | <span data-ttu-id="dc20a-184">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="dc20a-184">[identitySet][]</span></span>  | <span data-ttu-id="dc20a-185">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="dc20a-185">Identity of the last modifier of this item.</span></span> <span data-ttu-id="dc20a-186">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dc20a-186">Read-only.</span></span>
| <span data-ttu-id="dc20a-187">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="dc20a-187">**lastModifiedDateTime**</span></span> | <span data-ttu-id="dc20a-188">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc20a-188">DateTimeOffset</span></span>   | <span data-ttu-id="dc20a-p108">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dc20a-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="dc20a-191">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="dc20a-191">**webUrl**</span></span>               | <span data-ttu-id="dc20a-192">string (url)</span><span class="sxs-lookup"><span data-stu-id="dc20a-192">string (url)</span></span>     | <span data-ttu-id="dc20a-p109">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dc20a-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="dc20a-195">Relações</span><span class="sxs-lookup"><span data-stu-id="dc20a-195">Relationships</span></span>

<span data-ttu-id="dc20a-196">O recurso **list** tem as seguintes relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="dc20a-196">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="dc20a-197">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="dc20a-197">Relationship name</span></span> | <span data-ttu-id="dc20a-198">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc20a-198">Type</span></span>                        | <span data-ttu-id="dc20a-199">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc20a-199">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="dc20a-200">**activities**</span><span class="sxs-lookup"><span data-stu-id="dc20a-200">**activities**</span></span>    | <span data-ttu-id="dc20a-201">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="dc20a-201">[itemActivity][] collection</span></span> | <span data-ttu-id="dc20a-202">As atividades recentes que ocorreram nesta lista.</span><span class="sxs-lookup"><span data-stu-id="dc20a-202">The recent activities that took place within this list.</span></span>
| <span data-ttu-id="dc20a-203">**drive**</span><span class="sxs-lookup"><span data-stu-id="dc20a-203">**drive**</span></span>         | <span data-ttu-id="dc20a-204">[drive][]</span><span class="sxs-lookup"><span data-stu-id="dc20a-204">[drive][]</span></span>                   | <span data-ttu-id="dc20a-205">Presente somente em bibliotecas de documentos.</span><span class="sxs-lookup"><span data-stu-id="dc20a-205">Only present on document libraries.</span></span> <span data-ttu-id="dc20a-206">Permite o acesso à lista como um recurso de [unidade][] com [driveItems][driveItem].</span><span class="sxs-lookup"><span data-stu-id="dc20a-206">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="dc20a-207">**items**</span><span class="sxs-lookup"><span data-stu-id="dc20a-207">**items**</span></span>         | <span data-ttu-id="dc20a-208">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="dc20a-208">Collection([listItem][])</span></span>    | <span data-ttu-id="dc20a-209">Todos os itens contidos na lista.</span><span class="sxs-lookup"><span data-stu-id="dc20a-209">All items contained in the list.</span></span>
| <span data-ttu-id="dc20a-210">assinaturas</span><span class="sxs-lookup"><span data-stu-id="dc20a-210">subscriptions</span></span>      | <span data-ttu-id="dc20a-211">conjunto de [assinaturas][]</span><span class="sxs-lookup"><span data-stu-id="dc20a-211">[subscription][] collection</span></span> | <span data-ttu-id="dc20a-212">O conjunto de assinaturas na lista.</span><span class="sxs-lookup"><span data-stu-id="dc20a-212">The set of subscriptions on the list.</span></span>

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
