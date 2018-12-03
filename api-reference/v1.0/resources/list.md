---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Listar
ms.openlocfilehash: 3439443090e27c5ef48c2877fe9ea74a9c00cf42
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005805"
---
# <a name="list-resource"></a><span data-ttu-id="3c1f0-102">Recurso List</span><span class="sxs-lookup"><span data-stu-id="3c1f0-102">List resource</span></span>

<span data-ttu-id="3c1f0-103">O recurso **list** representa uma lista em um [site][].</span><span class="sxs-lookup"><span data-stu-id="3c1f0-103">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="3c1f0-104">Este recurso contém as propriedades de nível superior da lista, incluindo definições de modelo e campo.</span><span class="sxs-lookup"><span data-stu-id="3c1f0-104">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="3c1f0-105">Tarefas em list</span><span class="sxs-lookup"><span data-stu-id="3c1f0-105">Tasks on a list</span></span>

<span data-ttu-id="3c1f0-106">As tarefas a seguir estão disponíveis para os recursos list.</span><span class="sxs-lookup"><span data-stu-id="3c1f0-106">The following tasks are available for list resources.</span></span>
<span data-ttu-id="3c1f0-107">**Observação:** esta versão beta só permite navegar por listas, não criar ou atualizá-las.</span><span class="sxs-lookup"><span data-stu-id="3c1f0-107">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="3c1f0-108">Você pode, no entanto, criar ou atualizar [itens de lista][listItem].</span><span class="sxs-lookup"><span data-stu-id="3c1f0-108">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="3c1f0-109">Todos os exemplos a seguir referem-se a um site: `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="3c1f0-109">All examples below are relative to a site, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span></span>

| <span data-ttu-id="3c1f0-110">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="3c1f0-110">Common task</span></span>               | <span data-ttu-id="3c1f0-111">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="3c1f0-111">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="3c1f0-112">[Obter lista][]</span><span class="sxs-lookup"><span data-stu-id="3c1f0-112">[Get list][]</span></span>              | <span data-ttu-id="3c1f0-113">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="3c1f0-113">GET /lists/{list-id}</span></span>
| <span data-ttu-id="3c1f0-114">[Enumerar itens de lista][]</span><span class="sxs-lookup"><span data-stu-id="3c1f0-114">[Enumerate list items][]</span></span>  | <span data-ttu-id="3c1f0-115">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="3c1f0-115">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="3c1f0-116">[Atualizar item de lista][]</span><span class="sxs-lookup"><span data-stu-id="3c1f0-116">[Update list item][]</span></span>      | <span data-ttu-id="3c1f0-117">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="3c1f0-117">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="3c1f0-118">[Excluir item de lista][]</span><span class="sxs-lookup"><span data-stu-id="3c1f0-118">[Delete list item][]</span></span>      | <span data-ttu-id="3c1f0-119">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="3c1f0-119">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="3c1f0-120">[Criar item de lista][]</span><span class="sxs-lookup"><span data-stu-id="3c1f0-120">[Create list item][]</span></span>      | <span data-ttu-id="3c1f0-121">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="3c1f0-121">POST /lists/{list-id}</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="3c1f0-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3c1f0-127">JSON representation</span></span>

<span data-ttu-id="3c1f0-128">Veja a seguir uma representação JSON de um recurso **list**.</span><span class="sxs-lookup"><span data-stu-id="3c1f0-128">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="3c1f0-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3c1f0-129">Properties</span></span>

<span data-ttu-id="3c1f0-130">O recurso **list** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="3c1f0-130">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="3c1f0-131">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="3c1f0-131">Property name</span></span>    | <span data-ttu-id="3c1f0-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c1f0-132">Type</span></span>                             | <span data-ttu-id="3c1f0-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c1f0-133">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="3c1f0-134">**displayName**</span><span class="sxs-lookup"><span data-stu-id="3c1f0-134">**displayName**</span></span>  | <span data-ttu-id="3c1f0-135">string</span><span class="sxs-lookup"><span data-stu-id="3c1f0-135">string</span></span>                           | <span data-ttu-id="3c1f0-136">O título em exibição da lista.</span><span class="sxs-lookup"><span data-stu-id="3c1f0-136">The displayable title of the list.</span></span>
| <span data-ttu-id="3c1f0-137">**list**</span><span class="sxs-lookup"><span data-stu-id="3c1f0-137">**list**</span></span>         | <span data-ttu-id="3c1f0-138">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="3c1f0-138">[listInfo][]</span></span>                     | <span data-ttu-id="3c1f0-139">Fornece mais detalhes sobre a lista.</span><span class="sxs-lookup"><span data-stu-id="3c1f0-139">Provides additional details about the list.</span></span>
| <span data-ttu-id="3c1f0-140">**system**</span><span class="sxs-lookup"><span data-stu-id="3c1f0-140">**system**</span></span>       | <span data-ttu-id="3c1f0-141">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="3c1f0-141">[systemFacet][]</span></span>                  | <span data-ttu-id="3c1f0-142">Se estiver presente, indica que se trata de uma lista gerenciada pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="3c1f0-142">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="3c1f0-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3c1f0-143">Read-only.</span></span>

<span data-ttu-id="3c1f0-144">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="3c1f0-144">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="3c1f0-145">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="3c1f0-145">Property name</span></span>            | <span data-ttu-id="3c1f0-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c1f0-146">Type</span></span>              | <span data-ttu-id="3c1f0-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c1f0-147">Description</span></span>
|:-------------------------|:------------------|:------------------------------
| <span data-ttu-id="3c1f0-148">**id**</span><span class="sxs-lookup"><span data-stu-id="3c1f0-148">**id**</span></span>                   | <span data-ttu-id="3c1f0-149">string</span><span class="sxs-lookup"><span data-stu-id="3c1f0-149">string</span></span>            | <span data-ttu-id="3c1f0-p104">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3c1f0-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="3c1f0-152">**name**</span><span class="sxs-lookup"><span data-stu-id="3c1f0-152">**name**</span></span>                 | <span data-ttu-id="3c1f0-153">string</span><span class="sxs-lookup"><span data-stu-id="3c1f0-153">string</span></span>            | <span data-ttu-id="3c1f0-154">O nome do item.</span><span class="sxs-lookup"><span data-stu-id="3c1f0-154">The name of the item.</span></span>
| <span data-ttu-id="3c1f0-155">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="3c1f0-155">**createdBy**</span></span>            | <span data-ttu-id="3c1f0-156">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="3c1f0-156">[identitySet][]</span></span>   | <span data-ttu-id="3c1f0-157">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="3c1f0-157">Identity of the creator of this item.</span></span> <span data-ttu-id="3c1f0-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3c1f0-158">Read-only.</span></span>
| <span data-ttu-id="3c1f0-159">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="3c1f0-159">**createdDateTime**</span></span>      | <span data-ttu-id="3c1f0-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c1f0-160">DateTimeOffset</span></span>    | <span data-ttu-id="3c1f0-p106">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3c1f0-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="3c1f0-163">**description**</span><span class="sxs-lookup"><span data-stu-id="3c1f0-163">**description**</span></span>          | <span data-ttu-id="3c1f0-164">string</span><span class="sxs-lookup"><span data-stu-id="3c1f0-164">string</span></span>            | <span data-ttu-id="3c1f0-165">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="3c1f0-165">The descriptive text for the item.</span></span>
| <span data-ttu-id="3c1f0-166">**eTag**</span><span class="sxs-lookup"><span data-stu-id="3c1f0-166">**eTag**</span></span>                 | <span data-ttu-id="3c1f0-167">string</span><span class="sxs-lookup"><span data-stu-id="3c1f0-167">string</span></span>            | <span data-ttu-id="3c1f0-p107">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3c1f0-p107">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="3c1f0-170">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="3c1f0-170">**lastModifiedBy**</span></span>       | <span data-ttu-id="3c1f0-171">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="3c1f0-171">[identitySet][]</span></span>   | <span data-ttu-id="3c1f0-172">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="3c1f0-172">Identity of the last modifier of this item.</span></span> <span data-ttu-id="3c1f0-173">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3c1f0-173">Read-only.</span></span>
| <span data-ttu-id="3c1f0-174">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="3c1f0-174">**lastModifiedDateTime**</span></span> | <span data-ttu-id="3c1f0-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c1f0-175">DateTimeOffset</span></span>    | <span data-ttu-id="3c1f0-p109">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3c1f0-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="3c1f0-178">**parentReference**</span><span class="sxs-lookup"><span data-stu-id="3c1f0-178">**parentReference**</span></span>      | <span data-ttu-id="3c1f0-179">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="3c1f0-179">[itemReference][]</span></span> | <span data-ttu-id="3c1f0-p110">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="3c1f0-p110">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="3c1f0-182">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="3c1f0-182">**sharepointIds**</span></span>        | <span data-ttu-id="3c1f0-183">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="3c1f0-183">[sharepointIds][]</span></span> | <span data-ttu-id="3c1f0-p111">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3c1f0-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="3c1f0-186">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="3c1f0-186">**webUrl**</span></span>               | <span data-ttu-id="3c1f0-187">string (url)</span><span class="sxs-lookup"><span data-stu-id="3c1f0-187">string (url)</span></span>      | <span data-ttu-id="3c1f0-p112">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3c1f0-p112">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="3c1f0-190">Relações</span><span class="sxs-lookup"><span data-stu-id="3c1f0-190">Relationships</span></span>

<span data-ttu-id="3c1f0-191">O recurso **list** tem as seguintes relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="3c1f0-191">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="3c1f0-192">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="3c1f0-192">Relationship name</span></span> | <span data-ttu-id="3c1f0-193">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c1f0-193">Type</span></span>                             | <span data-ttu-id="3c1f0-194">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c1f0-194">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="3c1f0-195">**drive**</span><span class="sxs-lookup"><span data-stu-id="3c1f0-195">**drive**</span></span>         | <span data-ttu-id="3c1f0-196">[drive][]</span><span class="sxs-lookup"><span data-stu-id="3c1f0-196">[drive][]</span></span>                        | <span data-ttu-id="3c1f0-197">Presente somente em bibliotecas de documentos.</span><span class="sxs-lookup"><span data-stu-id="3c1f0-197">Only present on document libraries.</span></span> <span data-ttu-id="3c1f0-198">Permite o acesso à lista como um recurso [drive][] com [driveItems][driveItem].</span><span class="sxs-lookup"><span data-stu-id="3c1f0-198">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="3c1f0-199">**items**</span><span class="sxs-lookup"><span data-stu-id="3c1f0-199">**items**</span></span>         | <span data-ttu-id="3c1f0-200">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="3c1f0-200">Collection([listItem][])</span></span>         | <span data-ttu-id="3c1f0-201">Todos os itens contidos na lista.</span><span class="sxs-lookup"><span data-stu-id="3c1f0-201">All items contained in the list.</span></span>
| <span data-ttu-id="3c1f0-202">**columns**</span><span class="sxs-lookup"><span data-stu-id="3c1f0-202">**columns**</span></span>       | <span data-ttu-id="3c1f0-203">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="3c1f0-203">Collection([columnDefinition][])</span></span> | <span data-ttu-id="3c1f0-204">A coleção de definições de campo para esta lista.</span><span class="sxs-lookup"><span data-stu-id="3c1f0-204">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="3c1f0-205">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="3c1f0-205">**contentTypes**</span></span>  | <span data-ttu-id="3c1f0-206">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="3c1f0-206">Collection([contentType][])</span></span>      | <span data-ttu-id="3c1f0-207">A coleção de tipos de conteúdo presentes nesta lista.</span><span class="sxs-lookup"><span data-stu-id="3c1f0-207">The collection of content types present in this list.</span></span>

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
