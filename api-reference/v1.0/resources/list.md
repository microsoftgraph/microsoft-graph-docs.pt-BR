---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Listar
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 6bfd46e0822045869074cb0d78f14e3f0be0c994
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984385"
---
# <a name="list-resource"></a><span data-ttu-id="0c02f-102">Recurso List</span><span class="sxs-lookup"><span data-stu-id="0c02f-102">List resource</span></span>

<span data-ttu-id="0c02f-103">O recurso **list** representa uma lista em um [site][].</span><span class="sxs-lookup"><span data-stu-id="0c02f-103">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="0c02f-104">Este recurso contém as propriedades de nível superior da lista, incluindo definições de modelo e campo.</span><span class="sxs-lookup"><span data-stu-id="0c02f-104">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="0c02f-105">Tarefas em list</span><span class="sxs-lookup"><span data-stu-id="0c02f-105">Tasks on a list</span></span>

<span data-ttu-id="0c02f-106">As tarefas a seguir estão disponíveis para os recursos list.</span><span class="sxs-lookup"><span data-stu-id="0c02f-106">The following tasks are available for list resources.</span></span>
<span data-ttu-id="0c02f-107">**Observação:** esta versão beta só permite navegar por listas, não criar ou atualizá-las.</span><span class="sxs-lookup"><span data-stu-id="0c02f-107">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="0c02f-108">Você pode, no entanto, criar ou atualizar [itens de lista][listItem].</span><span class="sxs-lookup"><span data-stu-id="0c02f-108">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="0c02f-109">Todos os exemplos a seguir referem-se a um site: `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="0c02f-109">All examples below are relative to a site, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span></span>

| <span data-ttu-id="0c02f-110">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="0c02f-110">Common task</span></span>               | <span data-ttu-id="0c02f-111">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="0c02f-111">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="0c02f-112">[Obter lista][]</span><span class="sxs-lookup"><span data-stu-id="0c02f-112">[Get list][]</span></span>              | <span data-ttu-id="0c02f-113">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="0c02f-113">GET /lists/{list-id}</span></span>
| <span data-ttu-id="0c02f-114">[Enumerar itens de lista][]</span><span class="sxs-lookup"><span data-stu-id="0c02f-114">[Enumerate list items][]</span></span>  | <span data-ttu-id="0c02f-115">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="0c02f-115">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="0c02f-116">[Atualizar item de lista][]</span><span class="sxs-lookup"><span data-stu-id="0c02f-116">[Update list item][]</span></span>      | <span data-ttu-id="0c02f-117">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="0c02f-117">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="0c02f-118">[Excluir item de lista][]</span><span class="sxs-lookup"><span data-stu-id="0c02f-118">[Delete list item][]</span></span>      | <span data-ttu-id="0c02f-119">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="0c02f-119">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="0c02f-120">[Criar item de lista][]</span><span class="sxs-lookup"><span data-stu-id="0c02f-120">[Create list item][]</span></span>      | <span data-ttu-id="0c02f-121">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="0c02f-121">POST /lists/{list-id}</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="0c02f-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0c02f-127">JSON representation</span></span>

<span data-ttu-id="0c02f-128">Veja a seguir uma representação JSON de um recurso **list**.</span><span class="sxs-lookup"><span data-stu-id="0c02f-128">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="0c02f-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0c02f-129">Properties</span></span>

<span data-ttu-id="0c02f-130">O recurso **list** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="0c02f-130">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="0c02f-131">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="0c02f-131">Property name</span></span>    | <span data-ttu-id="0c02f-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c02f-132">Type</span></span>                             | <span data-ttu-id="0c02f-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c02f-133">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="0c02f-134">**displayName**</span><span class="sxs-lookup"><span data-stu-id="0c02f-134">**displayName**</span></span>  | <span data-ttu-id="0c02f-135">string</span><span class="sxs-lookup"><span data-stu-id="0c02f-135">string</span></span>                           | <span data-ttu-id="0c02f-136">O título em exibição da lista.</span><span class="sxs-lookup"><span data-stu-id="0c02f-136">The displayable title of the list.</span></span>
| <span data-ttu-id="0c02f-137">**list**</span><span class="sxs-lookup"><span data-stu-id="0c02f-137">**list**</span></span>         | <span data-ttu-id="0c02f-138">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="0c02f-138">[listInfo][]</span></span>                     | <span data-ttu-id="0c02f-139">Fornece mais detalhes sobre a lista.</span><span class="sxs-lookup"><span data-stu-id="0c02f-139">Provides additional details about the list.</span></span>
| <span data-ttu-id="0c02f-140">**system**</span><span class="sxs-lookup"><span data-stu-id="0c02f-140">**system**</span></span>       | <span data-ttu-id="0c02f-141">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="0c02f-141">[systemFacet][]</span></span>                  | <span data-ttu-id="0c02f-142">Se estiver presente, indica que se trata de uma lista gerenciada pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="0c02f-142">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="0c02f-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0c02f-143">Read-only.</span></span>

<span data-ttu-id="0c02f-144">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="0c02f-144">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="0c02f-145">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="0c02f-145">Property name</span></span>            | <span data-ttu-id="0c02f-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c02f-146">Type</span></span>              | <span data-ttu-id="0c02f-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c02f-147">Description</span></span>
|:-------------------------|:------------------|:------------------------------
| <span data-ttu-id="0c02f-148">**id**</span><span class="sxs-lookup"><span data-stu-id="0c02f-148">**id**</span></span>                   | <span data-ttu-id="0c02f-149">string</span><span class="sxs-lookup"><span data-stu-id="0c02f-149">string</span></span>            | <span data-ttu-id="0c02f-p104">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0c02f-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="0c02f-152">**name**</span><span class="sxs-lookup"><span data-stu-id="0c02f-152">**name**</span></span>                 | <span data-ttu-id="0c02f-153">string</span><span class="sxs-lookup"><span data-stu-id="0c02f-153">string</span></span>            | <span data-ttu-id="0c02f-154">O nome do item.</span><span class="sxs-lookup"><span data-stu-id="0c02f-154">The name of the item.</span></span>
| <span data-ttu-id="0c02f-155">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="0c02f-155">**createdBy**</span></span>            | <span data-ttu-id="0c02f-156">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="0c02f-156">[identitySet][]</span></span>   | <span data-ttu-id="0c02f-157">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="0c02f-157">Identity of the creator of this item.</span></span> <span data-ttu-id="0c02f-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0c02f-158">Read-only.</span></span>
| <span data-ttu-id="0c02f-159">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="0c02f-159">**createdDateTime**</span></span>      | <span data-ttu-id="0c02f-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c02f-160">DateTimeOffset</span></span>    | <span data-ttu-id="0c02f-p106">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0c02f-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="0c02f-163">**description**</span><span class="sxs-lookup"><span data-stu-id="0c02f-163">**description**</span></span>          | <span data-ttu-id="0c02f-164">string</span><span class="sxs-lookup"><span data-stu-id="0c02f-164">string</span></span>            | <span data-ttu-id="0c02f-165">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="0c02f-165">The descriptive text for the item.</span></span>
| <span data-ttu-id="0c02f-166">**eTag**</span><span class="sxs-lookup"><span data-stu-id="0c02f-166">**eTag**</span></span>                 | <span data-ttu-id="0c02f-167">string</span><span class="sxs-lookup"><span data-stu-id="0c02f-167">string</span></span>            | <span data-ttu-id="0c02f-p107">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0c02f-p107">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="0c02f-170">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="0c02f-170">**lastModifiedBy**</span></span>       | <span data-ttu-id="0c02f-171">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="0c02f-171">[identitySet][]</span></span>   | <span data-ttu-id="0c02f-172">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="0c02f-172">Identity of the last modifier of this item.</span></span> <span data-ttu-id="0c02f-173">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0c02f-173">Read-only.</span></span>
| <span data-ttu-id="0c02f-174">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="0c02f-174">**lastModifiedDateTime**</span></span> | <span data-ttu-id="0c02f-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c02f-175">DateTimeOffset</span></span>    | <span data-ttu-id="0c02f-p109">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0c02f-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="0c02f-178">**parentReference**</span><span class="sxs-lookup"><span data-stu-id="0c02f-178">**parentReference**</span></span>      | <span data-ttu-id="0c02f-179">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="0c02f-179">[itemReference][]</span></span> | <span data-ttu-id="0c02f-p110">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="0c02f-p110">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="0c02f-182">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="0c02f-182">**sharepointIds**</span></span>        | <span data-ttu-id="0c02f-183">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="0c02f-183">[sharepointIds][]</span></span> | <span data-ttu-id="0c02f-p111">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0c02f-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="0c02f-186">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="0c02f-186">**webUrl**</span></span>               | <span data-ttu-id="0c02f-187">string (url)</span><span class="sxs-lookup"><span data-stu-id="0c02f-187">string (url)</span></span>      | <span data-ttu-id="0c02f-p112">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0c02f-p112">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="0c02f-190">Relações</span><span class="sxs-lookup"><span data-stu-id="0c02f-190">Relationships</span></span>

<span data-ttu-id="0c02f-191">O recurso **list** tem as seguintes relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="0c02f-191">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="0c02f-192">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="0c02f-192">Relationship name</span></span> | <span data-ttu-id="0c02f-193">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c02f-193">Type</span></span>                             | <span data-ttu-id="0c02f-194">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c02f-194">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="0c02f-195">**drive**</span><span class="sxs-lookup"><span data-stu-id="0c02f-195">**drive**</span></span>         | <span data-ttu-id="0c02f-196">[drive][]</span><span class="sxs-lookup"><span data-stu-id="0c02f-196">[drive][]</span></span>                        | <span data-ttu-id="0c02f-197">Presente somente em bibliotecas de documentos.</span><span class="sxs-lookup"><span data-stu-id="0c02f-197">Only present on document libraries.</span></span> <span data-ttu-id="0c02f-198">Permite o acesso à lista como um recurso [drive][] com [driveItems][driveItem].</span><span class="sxs-lookup"><span data-stu-id="0c02f-198">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="0c02f-199">**items**</span><span class="sxs-lookup"><span data-stu-id="0c02f-199">**items**</span></span>         | <span data-ttu-id="0c02f-200">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="0c02f-200">Collection([listItem][])</span></span>         | <span data-ttu-id="0c02f-201">Todos os itens contidos na lista.</span><span class="sxs-lookup"><span data-stu-id="0c02f-201">All items contained in the list.</span></span>
| <span data-ttu-id="0c02f-202">**columns**</span><span class="sxs-lookup"><span data-stu-id="0c02f-202">**columns**</span></span>       | <span data-ttu-id="0c02f-203">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="0c02f-203">Collection([columnDefinition][])</span></span> | <span data-ttu-id="0c02f-204">A coleção de definições de campo para esta lista.</span><span class="sxs-lookup"><span data-stu-id="0c02f-204">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="0c02f-205">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="0c02f-205">**contentTypes**</span></span>  | <span data-ttu-id="0c02f-206">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="0c02f-206">Collection([contentType][])</span></span>      | <span data-ttu-id="0c02f-207">A coleção de tipos de conteúdo presentes nesta lista.</span><span class="sxs-lookup"><span data-stu-id="0c02f-207">The collection of content types present in this list.</span></span>

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
