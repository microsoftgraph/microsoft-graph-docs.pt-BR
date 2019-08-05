---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Listar
localization_priority: Priority
ms.prod: sharepoint
description: O recurso de lista representa uma lista em um site.
doc_type: resourcePageType
ms.openlocfilehash: 51821bb20188c004af3f2aca868c3cfd953ce19c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036404"
---
# <a name="list-resource"></a><span data-ttu-id="70625-103">Recurso List</span><span class="sxs-lookup"><span data-stu-id="70625-103">List resource</span></span>

<span data-ttu-id="70625-104">O recurso **list** representa uma lista em um [site][].</span><span class="sxs-lookup"><span data-stu-id="70625-104">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="70625-105">Este recurso contém as propriedades de nível superior da lista, incluindo definições de modelo e campo.</span><span class="sxs-lookup"><span data-stu-id="70625-105">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="70625-106">Tarefas em list</span><span class="sxs-lookup"><span data-stu-id="70625-106">Tasks on a list</span></span>

<span data-ttu-id="70625-107">As tarefas a seguir estão disponíveis para os recursos list.</span><span class="sxs-lookup"><span data-stu-id="70625-107">The following tasks are available for list resources.</span></span>
<span data-ttu-id="70625-108">**Observação:** esta versão beta só permite navegar por listas, não criar ou atualizá-las.</span><span class="sxs-lookup"><span data-stu-id="70625-108">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="70625-109">Você pode, no entanto, criar ou atualizar [itens de lista][listItem].</span><span class="sxs-lookup"><span data-stu-id="70625-109">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="70625-110">Todos os exemplos a seguir referem-se a um site: `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="70625-110">All examples below are relative to a site, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span></span>

| <span data-ttu-id="70625-111">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="70625-111">Common task</span></span>               | <span data-ttu-id="70625-112">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="70625-112">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="70625-113">[Obter lista][]</span><span class="sxs-lookup"><span data-stu-id="70625-113">[Get list][]</span></span>              | <span data-ttu-id="70625-114">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="70625-114">GET /lists/{list-id}</span></span>
| <span data-ttu-id="70625-115">[Enumerar itens de lista][]</span><span class="sxs-lookup"><span data-stu-id="70625-115">[Enumerate list items][]</span></span>  | <span data-ttu-id="70625-116">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="70625-116">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="70625-117">[Atualizar item de lista][]</span><span class="sxs-lookup"><span data-stu-id="70625-117">[Update list item][]</span></span>      | <span data-ttu-id="70625-118">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="70625-118">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="70625-119">[Excluir item de lista][]</span><span class="sxs-lookup"><span data-stu-id="70625-119">[Delete list item][]</span></span>      | <span data-ttu-id="70625-120">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="70625-120">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="70625-121">[Criar item de lista][]</span><span class="sxs-lookup"><span data-stu-id="70625-121">[Create list item][]</span></span>      | <span data-ttu-id="70625-122">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="70625-122">POST /lists/{list-id}</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="70625-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="70625-128">JSON representation</span></span>

<span data-ttu-id="70625-129">Veja a seguir uma representação JSON de um recurso **list**.</span><span class="sxs-lookup"><span data-stu-id="70625-129">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="70625-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="70625-130">Properties</span></span>

<span data-ttu-id="70625-131">O recurso **list** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="70625-131">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="70625-132">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="70625-132">Property name</span></span>    | <span data-ttu-id="70625-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="70625-133">Type</span></span>                             | <span data-ttu-id="70625-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="70625-134">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="70625-135">**displayName**</span><span class="sxs-lookup"><span data-stu-id="70625-135">**displayName**</span></span>  | <span data-ttu-id="70625-136">string</span><span class="sxs-lookup"><span data-stu-id="70625-136">string</span></span>                           | <span data-ttu-id="70625-137">O título em exibição da lista.</span><span class="sxs-lookup"><span data-stu-id="70625-137">The displayable title of the list.</span></span>
| <span data-ttu-id="70625-138">**list**</span><span class="sxs-lookup"><span data-stu-id="70625-138">**list**</span></span>         | <span data-ttu-id="70625-139">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="70625-139">[listInfo][]</span></span>                     | <span data-ttu-id="70625-140">Fornece mais detalhes sobre a lista.</span><span class="sxs-lookup"><span data-stu-id="70625-140">Provides additional details about the list.</span></span>
| <span data-ttu-id="70625-141">**system**</span><span class="sxs-lookup"><span data-stu-id="70625-141">**system**</span></span>       | <span data-ttu-id="70625-142">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="70625-142">[systemFacet][]</span></span>                  | <span data-ttu-id="70625-143">Se estiver presente, indica que se trata de uma lista gerenciada pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="70625-143">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="70625-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="70625-144">Read-only.</span></span>

<span data-ttu-id="70625-145">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="70625-145">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="70625-146">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="70625-146">Property name</span></span>            | <span data-ttu-id="70625-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="70625-147">Type</span></span>              | <span data-ttu-id="70625-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="70625-148">Description</span></span>
|:-------------------------|:------------------|:------------------------------
| <span data-ttu-id="70625-149">**id**</span><span class="sxs-lookup"><span data-stu-id="70625-149">**id**</span></span>                   | <span data-ttu-id="70625-150">string</span><span class="sxs-lookup"><span data-stu-id="70625-150">string</span></span>            | <span data-ttu-id="70625-p104">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="70625-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="70625-153">**name**</span><span class="sxs-lookup"><span data-stu-id="70625-153">**name**</span></span>                 | <span data-ttu-id="70625-154">string</span><span class="sxs-lookup"><span data-stu-id="70625-154">string</span></span>            | <span data-ttu-id="70625-155">O nome do item.</span><span class="sxs-lookup"><span data-stu-id="70625-155">The name of the item.</span></span>
| <span data-ttu-id="70625-156">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="70625-156">**createdBy**</span></span>            | <span data-ttu-id="70625-157">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="70625-157">[identitySet][]</span></span>   | <span data-ttu-id="70625-158">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="70625-158">Identity of the creator of this item.</span></span> <span data-ttu-id="70625-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="70625-159">Read-only.</span></span>
| <span data-ttu-id="70625-160">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="70625-160">**createdDateTime**</span></span>      | <span data-ttu-id="70625-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70625-161">DateTimeOffset</span></span>    | <span data-ttu-id="70625-p106">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="70625-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="70625-164">**description**</span><span class="sxs-lookup"><span data-stu-id="70625-164">**description**</span></span>          | <span data-ttu-id="70625-165">string</span><span class="sxs-lookup"><span data-stu-id="70625-165">string</span></span>            | <span data-ttu-id="70625-166">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="70625-166">The descriptive text for the item.</span></span>
| <span data-ttu-id="70625-167">**eTag**</span><span class="sxs-lookup"><span data-stu-id="70625-167">**eTag**</span></span>                 | <span data-ttu-id="70625-168">string</span><span class="sxs-lookup"><span data-stu-id="70625-168">string</span></span>            | <span data-ttu-id="70625-p107">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="70625-p107">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="70625-171">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="70625-171">**lastModifiedBy**</span></span>       | <span data-ttu-id="70625-172">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="70625-172">[identitySet][]</span></span>   | <span data-ttu-id="70625-173">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="70625-173">Identity of the last modifier of this item.</span></span> <span data-ttu-id="70625-174">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="70625-174">Read-only.</span></span>
| <span data-ttu-id="70625-175">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="70625-175">**lastModifiedDateTime**</span></span> | <span data-ttu-id="70625-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70625-176">DateTimeOffset</span></span>    | <span data-ttu-id="70625-p109">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="70625-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="70625-179">**parentReference**</span><span class="sxs-lookup"><span data-stu-id="70625-179">**parentReference**</span></span>      | <span data-ttu-id="70625-180">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="70625-180">[itemReference][]</span></span> | <span data-ttu-id="70625-p110">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="70625-p110">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="70625-183">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="70625-183">**sharepointIds**</span></span>        | <span data-ttu-id="70625-184">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="70625-184">[sharepointIds][]</span></span> | <span data-ttu-id="70625-p111">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="70625-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="70625-187">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="70625-187">**webUrl**</span></span>               | <span data-ttu-id="70625-188">string (url)</span><span class="sxs-lookup"><span data-stu-id="70625-188">string (url)</span></span>      | <span data-ttu-id="70625-p112">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="70625-p112">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="70625-191">Relações</span><span class="sxs-lookup"><span data-stu-id="70625-191">Relationships</span></span>

<span data-ttu-id="70625-192">O recurso **list** tem as seguintes relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="70625-192">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="70625-193">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="70625-193">Relationship name</span></span> | <span data-ttu-id="70625-194">Tipo</span><span class="sxs-lookup"><span data-stu-id="70625-194">Type</span></span>                             | <span data-ttu-id="70625-195">Descrição</span><span class="sxs-lookup"><span data-stu-id="70625-195">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="70625-196">**drive**</span><span class="sxs-lookup"><span data-stu-id="70625-196">**drive**</span></span>         | <span data-ttu-id="70625-197">[drive][]</span><span class="sxs-lookup"><span data-stu-id="70625-197">[drive][]</span></span>                        | <span data-ttu-id="70625-198">Presente somente em bibliotecas de documentos.</span><span class="sxs-lookup"><span data-stu-id="70625-198">Only present on document libraries.</span></span> <span data-ttu-id="70625-199">Permite o acesso à lista como um recurso de [unidade][] com [driveItems][driveItem].</span><span class="sxs-lookup"><span data-stu-id="70625-199">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="70625-200">**items**</span><span class="sxs-lookup"><span data-stu-id="70625-200">**items**</span></span>         | <span data-ttu-id="70625-201">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="70625-201">Collection([listItem][])</span></span>         | <span data-ttu-id="70625-202">Todos os itens contidos na lista.</span><span class="sxs-lookup"><span data-stu-id="70625-202">All items contained in the list.</span></span>
| <span data-ttu-id="70625-203">**columns**</span><span class="sxs-lookup"><span data-stu-id="70625-203">**columns**</span></span>       | <span data-ttu-id="70625-204">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="70625-204">Collection([columnDefinition][])</span></span> | <span data-ttu-id="70625-205">A coleção de definições de campo para esta lista.</span><span class="sxs-lookup"><span data-stu-id="70625-205">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="70625-206">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="70625-206">**contentTypes**</span></span>  | <span data-ttu-id="70625-207">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="70625-207">Collection([contentType][])</span></span>      | <span data-ttu-id="70625-208">A coleção de tipos de conteúdo presentes nesta lista.</span><span class="sxs-lookup"><span data-stu-id="70625-208">The collection of content types present in this list.</span></span>

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
