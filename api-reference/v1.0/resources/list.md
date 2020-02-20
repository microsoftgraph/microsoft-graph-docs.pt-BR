---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Listar
localization_priority: Priority
ms.prod: sharepoint
description: O recurso de lista representa uma lista em um site.
doc_type: resourcePageType
ms.openlocfilehash: db6fceb1f7806b5356a4e75f1e4fb6a247bd5b00
ms.sourcegitcommit: f51ba08d604d93f5f6af9ee8979cbf76baa285ce
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/19/2020
ms.locfileid: "42108480"
---
# <a name="list-resource"></a><span data-ttu-id="4c9cd-103">Recurso List</span><span class="sxs-lookup"><span data-stu-id="4c9cd-103">List resource</span></span>

<span data-ttu-id="4c9cd-104">O recurso **list** representa uma lista em um [site][].</span><span class="sxs-lookup"><span data-stu-id="4c9cd-104">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="4c9cd-105">Este recurso contém as propriedades de nível superior da lista, incluindo definições de modelo e campo.</span><span class="sxs-lookup"><span data-stu-id="4c9cd-105">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="4c9cd-106">Tarefas em list</span><span class="sxs-lookup"><span data-stu-id="4c9cd-106">Tasks on a list</span></span>

<span data-ttu-id="4c9cd-107">As tarefas a seguir estão disponíveis para os recursos list.</span><span class="sxs-lookup"><span data-stu-id="4c9cd-107">The following tasks are available for list resources.</span></span>
<span data-ttu-id="4c9cd-108">**Observação:** esta versão beta só permite navegar por listas, não criar ou atualizá-las.</span><span class="sxs-lookup"><span data-stu-id="4c9cd-108">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="4c9cd-109">Você pode, no entanto, criar ou atualizar [itens de lista][listItem].</span><span class="sxs-lookup"><span data-stu-id="4c9cd-109">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="4c9cd-110">Todos os exemplos a seguir referem-se a um site: `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="4c9cd-110">All examples below are relative to a site, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span></span>

| <span data-ttu-id="4c9cd-111">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="4c9cd-111">Common task</span></span>               | <span data-ttu-id="4c9cd-112">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="4c9cd-112">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="4c9cd-113">[Obter lista][]</span><span class="sxs-lookup"><span data-stu-id="4c9cd-113">[Get list][]</span></span>              | <span data-ttu-id="4c9cd-114">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="4c9cd-114">GET /lists/{list-id}</span></span>
| <span data-ttu-id="4c9cd-115">[Criar lista][]</span><span class="sxs-lookup"><span data-stu-id="4c9cd-115">[Create list][]</span></span>           | <span data-ttu-id="4c9cd-116">POSTAR/listas</span><span class="sxs-lookup"><span data-stu-id="4c9cd-116">POST /lists</span></span>
| <span data-ttu-id="4c9cd-117">[Enumerar itens de lista][]</span><span class="sxs-lookup"><span data-stu-id="4c9cd-117">[Enumerate list items][]</span></span>  | <span data-ttu-id="4c9cd-118">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="4c9cd-118">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="4c9cd-119">[Atualizar item de lista][]</span><span class="sxs-lookup"><span data-stu-id="4c9cd-119">[Update list item][]</span></span>      | <span data-ttu-id="4c9cd-120">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="4c9cd-120">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="4c9cd-121">[Excluir item de lista][]</span><span class="sxs-lookup"><span data-stu-id="4c9cd-121">[Delete list item][]</span></span>      | <span data-ttu-id="4c9cd-122">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="4c9cd-122">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="4c9cd-123">[Criar item de lista][]</span><span class="sxs-lookup"><span data-stu-id="4c9cd-123">[Create list item][]</span></span>      | <span data-ttu-id="4c9cd-124">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="4c9cd-124">POST /lists/{list-id}</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="4c9cd-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4c9cd-131">JSON representation</span></span>

<span data-ttu-id="4c9cd-132">Veja a seguir uma representação JSON de um recurso **list**.</span><span class="sxs-lookup"><span data-stu-id="4c9cd-132">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="4c9cd-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4c9cd-133">Properties</span></span>

<span data-ttu-id="4c9cd-134">O recurso **list** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="4c9cd-134">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="4c9cd-135">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="4c9cd-135">Property name</span></span>    | <span data-ttu-id="4c9cd-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c9cd-136">Type</span></span>                             | <span data-ttu-id="4c9cd-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c9cd-137">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="4c9cd-138">**displayName**</span><span class="sxs-lookup"><span data-stu-id="4c9cd-138">**displayName**</span></span>  | <span data-ttu-id="4c9cd-139">string</span><span class="sxs-lookup"><span data-stu-id="4c9cd-139">string</span></span>                           | <span data-ttu-id="4c9cd-140">O título em exibição da lista.</span><span class="sxs-lookup"><span data-stu-id="4c9cd-140">The displayable title of the list.</span></span>
| <span data-ttu-id="4c9cd-141">**list**</span><span class="sxs-lookup"><span data-stu-id="4c9cd-141">**list**</span></span>         | <span data-ttu-id="4c9cd-142">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="4c9cd-142">[listInfo][]</span></span>                     | <span data-ttu-id="4c9cd-143">Fornece mais detalhes sobre a lista.</span><span class="sxs-lookup"><span data-stu-id="4c9cd-143">Provides additional details about the list.</span></span>
| <span data-ttu-id="4c9cd-144">**system**</span><span class="sxs-lookup"><span data-stu-id="4c9cd-144">**system**</span></span>       | <span data-ttu-id="4c9cd-145">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="4c9cd-145">[systemFacet][]</span></span>                  | <span data-ttu-id="4c9cd-146">Se estiver presente, indica que se trata de uma lista gerenciada pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="4c9cd-146">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="4c9cd-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4c9cd-147">Read-only.</span></span>

<span data-ttu-id="4c9cd-148">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="4c9cd-148">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="4c9cd-149">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="4c9cd-149">Property name</span></span>            | <span data-ttu-id="4c9cd-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c9cd-150">Type</span></span>              | <span data-ttu-id="4c9cd-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c9cd-151">Description</span></span>
|:-------------------------|:------------------|:------------------------------
| <span data-ttu-id="4c9cd-152">**id**</span><span class="sxs-lookup"><span data-stu-id="4c9cd-152">**id**</span></span>                   | <span data-ttu-id="4c9cd-153">string</span><span class="sxs-lookup"><span data-stu-id="4c9cd-153">string</span></span>            | <span data-ttu-id="4c9cd-p104">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4c9cd-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="4c9cd-156">**name**</span><span class="sxs-lookup"><span data-stu-id="4c9cd-156">**name**</span></span>                 | <span data-ttu-id="4c9cd-157">string</span><span class="sxs-lookup"><span data-stu-id="4c9cd-157">string</span></span>            | <span data-ttu-id="4c9cd-158">O nome do item.</span><span class="sxs-lookup"><span data-stu-id="4c9cd-158">The name of the item.</span></span>
| <span data-ttu-id="4c9cd-159">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="4c9cd-159">**createdBy**</span></span>            | <span data-ttu-id="4c9cd-160">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="4c9cd-160">[identitySet][]</span></span>   | <span data-ttu-id="4c9cd-161">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="4c9cd-161">Identity of the creator of this item.</span></span> <span data-ttu-id="4c9cd-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4c9cd-162">Read-only.</span></span>
| <span data-ttu-id="4c9cd-163">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="4c9cd-163">**createdDateTime**</span></span>      | <span data-ttu-id="4c9cd-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c9cd-164">DateTimeOffset</span></span>    | <span data-ttu-id="4c9cd-p106">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4c9cd-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="4c9cd-167">**description**</span><span class="sxs-lookup"><span data-stu-id="4c9cd-167">**description**</span></span>          | <span data-ttu-id="4c9cd-168">string</span><span class="sxs-lookup"><span data-stu-id="4c9cd-168">string</span></span>            | <span data-ttu-id="4c9cd-169">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="4c9cd-169">The descriptive text for the item.</span></span>
| <span data-ttu-id="4c9cd-170">**eTag**</span><span class="sxs-lookup"><span data-stu-id="4c9cd-170">**eTag**</span></span>                 | <span data-ttu-id="4c9cd-171">string</span><span class="sxs-lookup"><span data-stu-id="4c9cd-171">string</span></span>            | <span data-ttu-id="4c9cd-p107">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4c9cd-p107">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="4c9cd-174">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="4c9cd-174">**lastModifiedBy**</span></span>       | <span data-ttu-id="4c9cd-175">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="4c9cd-175">[identitySet][]</span></span>   | <span data-ttu-id="4c9cd-176">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="4c9cd-176">Identity of the last modifier of this item.</span></span> <span data-ttu-id="4c9cd-177">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4c9cd-177">Read-only.</span></span>
| <span data-ttu-id="4c9cd-178">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="4c9cd-178">**lastModifiedDateTime**</span></span> | <span data-ttu-id="4c9cd-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c9cd-179">DateTimeOffset</span></span>    | <span data-ttu-id="4c9cd-p109">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4c9cd-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="4c9cd-182">**parentReference**</span><span class="sxs-lookup"><span data-stu-id="4c9cd-182">**parentReference**</span></span>      | <span data-ttu-id="4c9cd-183">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="4c9cd-183">[itemReference][]</span></span> | <span data-ttu-id="4c9cd-p110">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="4c9cd-p110">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="4c9cd-186">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="4c9cd-186">**sharepointIds**</span></span>        | <span data-ttu-id="4c9cd-187">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="4c9cd-187">[sharepointIds][]</span></span> | <span data-ttu-id="4c9cd-p111">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4c9cd-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="4c9cd-190">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="4c9cd-190">**webUrl**</span></span>               | <span data-ttu-id="4c9cd-191">string (url)</span><span class="sxs-lookup"><span data-stu-id="4c9cd-191">string (url)</span></span>      | <span data-ttu-id="4c9cd-p112">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4c9cd-p112">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="4c9cd-194">Relações</span><span class="sxs-lookup"><span data-stu-id="4c9cd-194">Relationships</span></span>

<span data-ttu-id="4c9cd-195">O recurso **list** tem as seguintes relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="4c9cd-195">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="4c9cd-196">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="4c9cd-196">Relationship name</span></span> | <span data-ttu-id="4c9cd-197">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c9cd-197">Type</span></span>                             | <span data-ttu-id="4c9cd-198">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c9cd-198">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="4c9cd-199">**drive**</span><span class="sxs-lookup"><span data-stu-id="4c9cd-199">**drive**</span></span>         | <span data-ttu-id="4c9cd-200">[drive][]</span><span class="sxs-lookup"><span data-stu-id="4c9cd-200">[drive][]</span></span>                        | <span data-ttu-id="4c9cd-201">Presente somente em bibliotecas de documentos.</span><span class="sxs-lookup"><span data-stu-id="4c9cd-201">Only present on document libraries.</span></span> <span data-ttu-id="4c9cd-202">Permite o acesso à lista como um recurso de [unidade][] com [driveItems][driveItem].</span><span class="sxs-lookup"><span data-stu-id="4c9cd-202">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="4c9cd-203">**items**</span><span class="sxs-lookup"><span data-stu-id="4c9cd-203">**items**</span></span>         | <span data-ttu-id="4c9cd-204">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="4c9cd-204">Collection([listItem][])</span></span>         | <span data-ttu-id="4c9cd-205">Todos os itens contidos na lista.</span><span class="sxs-lookup"><span data-stu-id="4c9cd-205">All items contained in the list.</span></span>
| <span data-ttu-id="4c9cd-206">**columns**</span><span class="sxs-lookup"><span data-stu-id="4c9cd-206">**columns**</span></span>       | <span data-ttu-id="4c9cd-207">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="4c9cd-207">Collection([columnDefinition][])</span></span> | <span data-ttu-id="4c9cd-208">A coleção de definições de campo para esta lista.</span><span class="sxs-lookup"><span data-stu-id="4c9cd-208">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="4c9cd-209">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="4c9cd-209">**contentTypes**</span></span>  | <span data-ttu-id="4c9cd-210">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="4c9cd-210">Collection([contentType][])</span></span>      | <span data-ttu-id="4c9cd-211">A coleção de tipos de conteúdo presentes nesta lista.</span><span class="sxs-lookup"><span data-stu-id="4c9cd-211">The collection of content types present in this list.</span></span>

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
