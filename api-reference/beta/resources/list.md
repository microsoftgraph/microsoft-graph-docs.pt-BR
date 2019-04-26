---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Listar
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5e078c79603235059cbe326c850e51dfa33d2f8e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345329"
---
# <a name="list-resource"></a><span data-ttu-id="e7a0c-102">Recurso List</span><span class="sxs-lookup"><span data-stu-id="e7a0c-102">List resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7a0c-103">O recurso **list** representa uma lista em um [site][].</span><span class="sxs-lookup"><span data-stu-id="e7a0c-103">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="e7a0c-104">Este recurso contém as propriedades de nível superior da lista, incluindo definições de modelo e campo.</span><span class="sxs-lookup"><span data-stu-id="e7a0c-104">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="e7a0c-105">Tarefas em list</span><span class="sxs-lookup"><span data-stu-id="e7a0c-105">Tasks on a list</span></span>

<span data-ttu-id="e7a0c-106">As tarefas a seguir estão disponíveis para os recursos list.</span><span class="sxs-lookup"><span data-stu-id="e7a0c-106">The following tasks are available for list resources.</span></span>
<span data-ttu-id="e7a0c-107">**Observação:** esta versão beta só permite navegar por listas, não criar ou atualizá-las.</span><span class="sxs-lookup"><span data-stu-id="e7a0c-107">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="e7a0c-108">Você pode, no entanto, criar ou atualizar [itens de lista][listItem].</span><span class="sxs-lookup"><span data-stu-id="e7a0c-108">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="e7a0c-109">Todos os exemplos a seguir referem-se a um site: `https://graph.microsoft.com/beta/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="e7a0c-109">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="e7a0c-110">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="e7a0c-110">Common task</span></span>               | <span data-ttu-id="e7a0c-111">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="e7a0c-111">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="e7a0c-112">[Obter lista][]</span><span class="sxs-lookup"><span data-stu-id="e7a0c-112">[Get list][]</span></span>              | <span data-ttu-id="e7a0c-113">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="e7a0c-113">GET /lists/{list-id}</span></span>
| <span data-ttu-id="e7a0c-114">[Enumerar itens de lista][]</span><span class="sxs-lookup"><span data-stu-id="e7a0c-114">[Enumerate list items][]</span></span>  | <span data-ttu-id="e7a0c-115">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="e7a0c-115">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="e7a0c-116">[Atualizar item de lista][]</span><span class="sxs-lookup"><span data-stu-id="e7a0c-116">[Update list item][]</span></span>      | <span data-ttu-id="e7a0c-117">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="e7a0c-117">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="e7a0c-118">[Excluir item de lista][]</span><span class="sxs-lookup"><span data-stu-id="e7a0c-118">[Delete list item][]</span></span>      | <span data-ttu-id="e7a0c-119">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="e7a0c-119">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="e7a0c-120">[Criar item de lista][]</span><span class="sxs-lookup"><span data-stu-id="e7a0c-120">[Create list item][]</span></span>      | <span data-ttu-id="e7a0c-121">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="e7a0c-121">POST /lists/{list-id}</span></span>
| <span data-ttu-id="e7a0c-122">[Obter atividades recentes][]</span><span class="sxs-lookup"><span data-stu-id="e7a0c-122">[Get recent activities][]</span></span> | <span data-ttu-id="e7a0c-123">GET /lists/{list-id}/activities</span><span class="sxs-lookup"><span data-stu-id="e7a0c-123">GET /lists/{list-id}/activities</span></span>

[Obter lista]: ../api/list-get.md
[Get list]: ../api/list-get.md
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

## <a name="json-representation"></a><span data-ttu-id="e7a0c-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e7a0c-130">JSON representation</span></span>

<span data-ttu-id="e7a0c-131">Veja a seguir uma representação JSON de um recurso **list**.</span><span class="sxs-lookup"><span data-stu-id="e7a0c-131">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="e7a0c-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e7a0c-132">Properties</span></span>

<span data-ttu-id="e7a0c-133">O recurso **list** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="e7a0c-133">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="e7a0c-134">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="e7a0c-134">Property name</span></span>    | <span data-ttu-id="e7a0c-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7a0c-135">Type</span></span>                             | <span data-ttu-id="e7a0c-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7a0c-136">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="e7a0c-137">**columns**</span><span class="sxs-lookup"><span data-stu-id="e7a0c-137">**columns**</span></span>      | <span data-ttu-id="e7a0c-138">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="e7a0c-138">Collection([columnDefinition][])</span></span> | <span data-ttu-id="e7a0c-139">A coleção de definições de campo para esta lista.</span><span class="sxs-lookup"><span data-stu-id="e7a0c-139">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="e7a0c-140">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="e7a0c-140">**contentTypes**</span></span> | <span data-ttu-id="e7a0c-141">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="e7a0c-141">Collection([contentType][])</span></span>      | <span data-ttu-id="e7a0c-142">A coleção de tipos de conteúdo presentes nesta lista.</span><span class="sxs-lookup"><span data-stu-id="e7a0c-142">The collection of content types present in this list.</span></span>
| <span data-ttu-id="e7a0c-143">**displayName**</span><span class="sxs-lookup"><span data-stu-id="e7a0c-143">**displayName**</span></span>  | <span data-ttu-id="e7a0c-144">string</span><span class="sxs-lookup"><span data-stu-id="e7a0c-144">string</span></span>                           | <span data-ttu-id="e7a0c-145">O título em exibição da lista.</span><span class="sxs-lookup"><span data-stu-id="e7a0c-145">The displayable title of the list.</span></span>
| <span data-ttu-id="e7a0c-146">**list**</span><span class="sxs-lookup"><span data-stu-id="e7a0c-146">**list**</span></span>         | <span data-ttu-id="e7a0c-147">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="e7a0c-147">[listInfo][]</span></span>                     | <span data-ttu-id="e7a0c-148">Fornece mais detalhes sobre a lista.</span><span class="sxs-lookup"><span data-stu-id="e7a0c-148">Provides additional details about the list.</span></span>
| <span data-ttu-id="e7a0c-149">**system**</span><span class="sxs-lookup"><span data-stu-id="e7a0c-149">**system**</span></span>       | <span data-ttu-id="e7a0c-150">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="e7a0c-150">[systemFacet][]</span></span>                  | <span data-ttu-id="e7a0c-151">Se estiver presente, indica que se trata de uma lista gerenciada pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="e7a0c-151">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="e7a0c-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e7a0c-152">Read-only.</span></span>

<span data-ttu-id="e7a0c-153">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="e7a0c-153">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="e7a0c-154">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="e7a0c-154">Property name</span></span>            | <span data-ttu-id="e7a0c-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7a0c-155">Type</span></span>             | <span data-ttu-id="e7a0c-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7a0c-156">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="e7a0c-157">**id**</span><span class="sxs-lookup"><span data-stu-id="e7a0c-157">**id**</span></span>                   | <span data-ttu-id="e7a0c-158">string</span><span class="sxs-lookup"><span data-stu-id="e7a0c-158">string</span></span>           | <span data-ttu-id="e7a0c-p104">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e7a0c-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="e7a0c-161">**name**</span><span class="sxs-lookup"><span data-stu-id="e7a0c-161">**name**</span></span>                 | <span data-ttu-id="e7a0c-162">string</span><span class="sxs-lookup"><span data-stu-id="e7a0c-162">string</span></span>           | <span data-ttu-id="e7a0c-163">O nome do item.</span><span class="sxs-lookup"><span data-stu-id="e7a0c-163">The name of the item.</span></span>
| <span data-ttu-id="e7a0c-164">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="e7a0c-164">**createdBy**</span></span>            | <span data-ttu-id="e7a0c-165">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="e7a0c-165">[identitySet][]</span></span>  | <span data-ttu-id="e7a0c-166">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="e7a0c-166">Identity of the creator of this item.</span></span> <span data-ttu-id="e7a0c-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e7a0c-167">Read-only.</span></span>
| <span data-ttu-id="e7a0c-168">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="e7a0c-168">**createdDateTime**</span></span>      | <span data-ttu-id="e7a0c-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7a0c-169">DateTimeOffset</span></span>   | <span data-ttu-id="e7a0c-p106">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e7a0c-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="e7a0c-172">**description**</span><span class="sxs-lookup"><span data-stu-id="e7a0c-172">**description**</span></span>          | <span data-ttu-id="e7a0c-173">string</span><span class="sxs-lookup"><span data-stu-id="e7a0c-173">string</span></span>           | <span data-ttu-id="e7a0c-174">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="e7a0c-174">The descriptive text for the item.</span></span>
| <span data-ttu-id="e7a0c-175">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="e7a0c-175">**lastModifiedBy**</span></span>       | <span data-ttu-id="e7a0c-176">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="e7a0c-176">[identitySet][]</span></span>  | <span data-ttu-id="e7a0c-177">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="e7a0c-177">Identity of the last modifier of this item.</span></span> <span data-ttu-id="e7a0c-178">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e7a0c-178">Read-only.</span></span>
| <span data-ttu-id="e7a0c-179">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="e7a0c-179">**lastModifiedDateTime**</span></span> | <span data-ttu-id="e7a0c-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7a0c-180">DateTimeOffset</span></span>   | <span data-ttu-id="e7a0c-p108">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e7a0c-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="e7a0c-183">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="e7a0c-183">**webUrl**</span></span>               | <span data-ttu-id="e7a0c-184">string (url)</span><span class="sxs-lookup"><span data-stu-id="e7a0c-184">string (url)</span></span>     | <span data-ttu-id="e7a0c-p109">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e7a0c-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="e7a0c-187">Relações</span><span class="sxs-lookup"><span data-stu-id="e7a0c-187">Relationships</span></span>

<span data-ttu-id="e7a0c-188">O recurso **list** tem as seguintes relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="e7a0c-188">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="e7a0c-189">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="e7a0c-189">Relationship name</span></span> | <span data-ttu-id="e7a0c-190">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7a0c-190">Type</span></span>                        | <span data-ttu-id="e7a0c-191">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7a0c-191">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="e7a0c-192">**activities**</span><span class="sxs-lookup"><span data-stu-id="e7a0c-192">**activities**</span></span>    | <span data-ttu-id="e7a0c-193">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="e7a0c-193">[itemActivity][] collection</span></span> | <span data-ttu-id="e7a0c-194">As atividades recentes que ocorreram nesta lista.</span><span class="sxs-lookup"><span data-stu-id="e7a0c-194">The recent activities that took place within this list.</span></span>
| <span data-ttu-id="e7a0c-195">**drive**</span><span class="sxs-lookup"><span data-stu-id="e7a0c-195">**drive**</span></span>         | <span data-ttu-id="e7a0c-196">[drive][]</span><span class="sxs-lookup"><span data-stu-id="e7a0c-196">[drive][]</span></span>                   | <span data-ttu-id="e7a0c-197">Presente somente em bibliotecas de documentos.</span><span class="sxs-lookup"><span data-stu-id="e7a0c-197">Only present on document libraries.</span></span> <span data-ttu-id="e7a0c-198">Permite o acesso à lista como um recurso [drive][] com [driveItems][driveItem].</span><span class="sxs-lookup"><span data-stu-id="e7a0c-198">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="e7a0c-199">**items**</span><span class="sxs-lookup"><span data-stu-id="e7a0c-199">**items**</span></span>         | <span data-ttu-id="e7a0c-200">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="e7a0c-200">Collection([listItem][])</span></span>    | <span data-ttu-id="e7a0c-201">Todos os itens contidos na lista.</span><span class="sxs-lookup"><span data-stu-id="e7a0c-201">All items contained in the list.</span></span>

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
