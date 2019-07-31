---
author: JeremyKelley
description: O recurso list representa uma lista em um site.
ms.date: 09/11/2017
title: Listar
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: b79172049278758c77ac620f00c391d52633792b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009990"
---
# <a name="list-resource"></a><span data-ttu-id="26940-103">Recurso List</span><span class="sxs-lookup"><span data-stu-id="26940-103">List resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26940-104">O recurso **list** representa uma lista em um [site][].</span><span class="sxs-lookup"><span data-stu-id="26940-104">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="26940-105">Este recurso contém as propriedades de nível superior da lista, incluindo definições de modelo e campo.</span><span class="sxs-lookup"><span data-stu-id="26940-105">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="26940-106">Tarefas em list</span><span class="sxs-lookup"><span data-stu-id="26940-106">Tasks on a list</span></span>

<span data-ttu-id="26940-107">As tarefas a seguir estão disponíveis para os recursos list.</span><span class="sxs-lookup"><span data-stu-id="26940-107">The following tasks are available for list resources.</span></span>
<span data-ttu-id="26940-108">**Observação:** esta versão beta só permite navegar por listas, não criar ou atualizá-las.</span><span class="sxs-lookup"><span data-stu-id="26940-108">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="26940-109">Você pode, no entanto, criar ou atualizar [itens de lista][listItem].</span><span class="sxs-lookup"><span data-stu-id="26940-109">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="26940-110">Todos os exemplos a seguir referem-se a um site: `https://graph.microsoft.com/beta/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="26940-110">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="26940-111">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="26940-111">Common task</span></span>               | <span data-ttu-id="26940-112">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="26940-112">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="26940-113">[Obter lista][]</span><span class="sxs-lookup"><span data-stu-id="26940-113">[Get list][]</span></span>              | <span data-ttu-id="26940-114">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="26940-114">GET /lists/{list-id}</span></span>
| <span data-ttu-id="26940-115">[Enumerar itens de lista][]</span><span class="sxs-lookup"><span data-stu-id="26940-115">[Enumerate list items][]</span></span>  | <span data-ttu-id="26940-116">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="26940-116">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="26940-117">[Atualizar item de lista][]</span><span class="sxs-lookup"><span data-stu-id="26940-117">[Update list item][]</span></span>      | <span data-ttu-id="26940-118">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="26940-118">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="26940-119">[Excluir item de lista][]</span><span class="sxs-lookup"><span data-stu-id="26940-119">[Delete list item][]</span></span>      | <span data-ttu-id="26940-120">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="26940-120">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="26940-121">[Criar item de lista][]</span><span class="sxs-lookup"><span data-stu-id="26940-121">[Create list item][]</span></span>      | <span data-ttu-id="26940-122">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="26940-122">POST /lists/{list-id}</span></span>
| <span data-ttu-id="26940-123">[Obter atividades recentes][]</span><span class="sxs-lookup"><span data-stu-id="26940-123">[Get recent activities][]</span></span> | <span data-ttu-id="26940-124">GET /lists/{list-id}/activities</span><span class="sxs-lookup"><span data-stu-id="26940-124">GET /lists/{list-id}/activities</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="26940-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="26940-131">JSON representation</span></span>

<span data-ttu-id="26940-132">Veja a seguir uma representação JSON de um recurso **list**.</span><span class="sxs-lookup"><span data-stu-id="26940-132">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="26940-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="26940-133">Properties</span></span>

<span data-ttu-id="26940-134">O recurso **list** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="26940-134">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="26940-135">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="26940-135">Property name</span></span>    | <span data-ttu-id="26940-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="26940-136">Type</span></span>                             | <span data-ttu-id="26940-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="26940-137">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="26940-138">**columns**</span><span class="sxs-lookup"><span data-stu-id="26940-138">**columns**</span></span>      | <span data-ttu-id="26940-139">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="26940-139">Collection([columnDefinition][])</span></span> | <span data-ttu-id="26940-140">A coleção de definições de campo para esta lista.</span><span class="sxs-lookup"><span data-stu-id="26940-140">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="26940-141">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="26940-141">**contentTypes**</span></span> | <span data-ttu-id="26940-142">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="26940-142">Collection([contentType][])</span></span>      | <span data-ttu-id="26940-143">A coleção de tipos de conteúdo presentes nesta lista.</span><span class="sxs-lookup"><span data-stu-id="26940-143">The collection of content types present in this list.</span></span>
| <span data-ttu-id="26940-144">**displayName**</span><span class="sxs-lookup"><span data-stu-id="26940-144">**displayName**</span></span>  | <span data-ttu-id="26940-145">string</span><span class="sxs-lookup"><span data-stu-id="26940-145">string</span></span>                           | <span data-ttu-id="26940-146">O título em exibição da lista.</span><span class="sxs-lookup"><span data-stu-id="26940-146">The displayable title of the list.</span></span>
| <span data-ttu-id="26940-147">**list**</span><span class="sxs-lookup"><span data-stu-id="26940-147">**list**</span></span>         | <span data-ttu-id="26940-148">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="26940-148">[listInfo][]</span></span>                     | <span data-ttu-id="26940-149">Fornece mais detalhes sobre a lista.</span><span class="sxs-lookup"><span data-stu-id="26940-149">Provides additional details about the list.</span></span>
| <span data-ttu-id="26940-150">**system**</span><span class="sxs-lookup"><span data-stu-id="26940-150">**system**</span></span>       | <span data-ttu-id="26940-151">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="26940-151">[systemFacet][]</span></span>                  | <span data-ttu-id="26940-152">Se estiver presente, indica que se trata de uma lista gerenciada pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="26940-152">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="26940-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="26940-153">Read-only.</span></span>

<span data-ttu-id="26940-154">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="26940-154">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="26940-155">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="26940-155">Property name</span></span>            | <span data-ttu-id="26940-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="26940-156">Type</span></span>             | <span data-ttu-id="26940-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="26940-157">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="26940-158">**id**</span><span class="sxs-lookup"><span data-stu-id="26940-158">**id**</span></span>                   | <span data-ttu-id="26940-159">string</span><span class="sxs-lookup"><span data-stu-id="26940-159">string</span></span>           | <span data-ttu-id="26940-p104">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="26940-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="26940-162">**name**</span><span class="sxs-lookup"><span data-stu-id="26940-162">**name**</span></span>                 | <span data-ttu-id="26940-163">string</span><span class="sxs-lookup"><span data-stu-id="26940-163">string</span></span>           | <span data-ttu-id="26940-164">O nome do item.</span><span class="sxs-lookup"><span data-stu-id="26940-164">The name of the item.</span></span>
| <span data-ttu-id="26940-165">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="26940-165">**createdBy**</span></span>            | <span data-ttu-id="26940-166">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="26940-166">[identitySet][]</span></span>  | <span data-ttu-id="26940-167">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="26940-167">Identity of the creator of this item.</span></span> <span data-ttu-id="26940-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="26940-168">Read-only.</span></span>
| <span data-ttu-id="26940-169">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="26940-169">**createdDateTime**</span></span>      | <span data-ttu-id="26940-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26940-170">DateTimeOffset</span></span>   | <span data-ttu-id="26940-p106">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="26940-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="26940-173">**description**</span><span class="sxs-lookup"><span data-stu-id="26940-173">**description**</span></span>          | <span data-ttu-id="26940-174">string</span><span class="sxs-lookup"><span data-stu-id="26940-174">string</span></span>           | <span data-ttu-id="26940-175">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="26940-175">The descriptive text for the item.</span></span>
| <span data-ttu-id="26940-176">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="26940-176">**lastModifiedBy**</span></span>       | <span data-ttu-id="26940-177">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="26940-177">[identitySet][]</span></span>  | <span data-ttu-id="26940-178">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="26940-178">Identity of the last modifier of this item.</span></span> <span data-ttu-id="26940-179">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="26940-179">Read-only.</span></span>
| <span data-ttu-id="26940-180">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="26940-180">**lastModifiedDateTime**</span></span> | <span data-ttu-id="26940-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26940-181">DateTimeOffset</span></span>   | <span data-ttu-id="26940-p108">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="26940-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="26940-184">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="26940-184">**webUrl**</span></span>               | <span data-ttu-id="26940-185">string (url)</span><span class="sxs-lookup"><span data-stu-id="26940-185">string (url)</span></span>     | <span data-ttu-id="26940-p109">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="26940-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="26940-188">Relações</span><span class="sxs-lookup"><span data-stu-id="26940-188">Relationships</span></span>

<span data-ttu-id="26940-189">O recurso **list** tem as seguintes relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="26940-189">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="26940-190">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="26940-190">Relationship name</span></span> | <span data-ttu-id="26940-191">Tipo</span><span class="sxs-lookup"><span data-stu-id="26940-191">Type</span></span>                        | <span data-ttu-id="26940-192">Descrição</span><span class="sxs-lookup"><span data-stu-id="26940-192">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="26940-193">**activities**</span><span class="sxs-lookup"><span data-stu-id="26940-193">**activities**</span></span>    | <span data-ttu-id="26940-194">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="26940-194">[itemActivity][] collection</span></span> | <span data-ttu-id="26940-195">As atividades recentes que ocorreram nesta lista.</span><span class="sxs-lookup"><span data-stu-id="26940-195">The recent activities that took place within this list.</span></span>
| <span data-ttu-id="26940-196">**drive**</span><span class="sxs-lookup"><span data-stu-id="26940-196">**drive**</span></span>         | <span data-ttu-id="26940-197">[drive][]</span><span class="sxs-lookup"><span data-stu-id="26940-197">[drive][]</span></span>                   | <span data-ttu-id="26940-198">Presente somente em bibliotecas de documentos.</span><span class="sxs-lookup"><span data-stu-id="26940-198">Only present on document libraries.</span></span> <span data-ttu-id="26940-199">Permite o acesso à lista como um recurso [drive][] com [driveItems][driveItem].</span><span class="sxs-lookup"><span data-stu-id="26940-199">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="26940-200">**items**</span><span class="sxs-lookup"><span data-stu-id="26940-200">**items**</span></span>         | <span data-ttu-id="26940-201">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="26940-201">Collection([listItem][])</span></span>    | <span data-ttu-id="26940-202">Todos os itens contidos na lista.</span><span class="sxs-lookup"><span data-stu-id="26940-202">All items contained in the list.</span></span>

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
