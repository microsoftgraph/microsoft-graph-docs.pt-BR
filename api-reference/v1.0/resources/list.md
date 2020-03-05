---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Listar
localization_priority: Priority
ms.prod: sharepoint
description: O recurso de lista representa uma lista em um site.
doc_type: resourcePageType
ms.openlocfilehash: af970267f4aebcac986659324a30238a8510c010
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447581"
---
# <a name="list-resource"></a><span data-ttu-id="384d8-103">Recurso List</span><span class="sxs-lookup"><span data-stu-id="384d8-103">List resource</span></span>

<span data-ttu-id="384d8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="384d8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="384d8-105">O recurso **list** representa uma lista em um [site][].</span><span class="sxs-lookup"><span data-stu-id="384d8-105">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="384d8-106">Este recurso contém as propriedades de nível superior da lista, incluindo definições de modelo e campo.</span><span class="sxs-lookup"><span data-stu-id="384d8-106">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="384d8-107">Tarefas em list</span><span class="sxs-lookup"><span data-stu-id="384d8-107">Tasks on a list</span></span>

<span data-ttu-id="384d8-108">As tarefas a seguir estão disponíveis para os recursos list.</span><span class="sxs-lookup"><span data-stu-id="384d8-108">The following tasks are available for list resources.</span></span>
<span data-ttu-id="384d8-109">**Observação:** esta versão beta só permite navegar por listas, não criar ou atualizá-las.</span><span class="sxs-lookup"><span data-stu-id="384d8-109">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="384d8-110">Você pode, no entanto, criar ou atualizar [itens de lista][listItem].</span><span class="sxs-lookup"><span data-stu-id="384d8-110">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="384d8-111">Todos os exemplos a seguir referem-se a um site: `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="384d8-111">All examples below are relative to a site, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span></span>

| <span data-ttu-id="384d8-112">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="384d8-112">Common task</span></span>               | <span data-ttu-id="384d8-113">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="384d8-113">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="384d8-114">[Obter lista][]</span><span class="sxs-lookup"><span data-stu-id="384d8-114">[Get list][]</span></span>              | <span data-ttu-id="384d8-115">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="384d8-115">GET /lists/{list-id}</span></span>
| <span data-ttu-id="384d8-116">[Criar lista][]</span><span class="sxs-lookup"><span data-stu-id="384d8-116">[Create list][]</span></span>           | <span data-ttu-id="384d8-117">POSTAR/listas</span><span class="sxs-lookup"><span data-stu-id="384d8-117">POST /lists</span></span>
| <span data-ttu-id="384d8-118">[Enumerar itens de lista][]</span><span class="sxs-lookup"><span data-stu-id="384d8-118">[Enumerate list items][]</span></span>  | <span data-ttu-id="384d8-119">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="384d8-119">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="384d8-120">[Atualizar item de lista][]</span><span class="sxs-lookup"><span data-stu-id="384d8-120">[Update list item][]</span></span>      | <span data-ttu-id="384d8-121">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="384d8-121">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="384d8-122">[Excluir item de lista][]</span><span class="sxs-lookup"><span data-stu-id="384d8-122">[Delete list item][]</span></span>      | <span data-ttu-id="384d8-123">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="384d8-123">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="384d8-124">[Criar item de lista][]</span><span class="sxs-lookup"><span data-stu-id="384d8-124">[Create list item][]</span></span>      | <span data-ttu-id="384d8-125">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="384d8-125">POST /lists/{list-id}</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="384d8-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="384d8-132">JSON representation</span></span>

<span data-ttu-id="384d8-133">Veja a seguir uma representação JSON de um recurso **list**.</span><span class="sxs-lookup"><span data-stu-id="384d8-133">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="384d8-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="384d8-134">Properties</span></span>

<span data-ttu-id="384d8-135">O recurso **list** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="384d8-135">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="384d8-136">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="384d8-136">Property name</span></span>    | <span data-ttu-id="384d8-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="384d8-137">Type</span></span>                             | <span data-ttu-id="384d8-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="384d8-138">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="384d8-139">**displayName**</span><span class="sxs-lookup"><span data-stu-id="384d8-139">**displayName**</span></span>  | <span data-ttu-id="384d8-140">string</span><span class="sxs-lookup"><span data-stu-id="384d8-140">string</span></span>                           | <span data-ttu-id="384d8-141">O título em exibição da lista.</span><span class="sxs-lookup"><span data-stu-id="384d8-141">The displayable title of the list.</span></span>
| <span data-ttu-id="384d8-142">**list**</span><span class="sxs-lookup"><span data-stu-id="384d8-142">**list**</span></span>         | <span data-ttu-id="384d8-143">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="384d8-143">[listInfo][]</span></span>                     | <span data-ttu-id="384d8-144">Fornece mais detalhes sobre a lista.</span><span class="sxs-lookup"><span data-stu-id="384d8-144">Provides additional details about the list.</span></span>
| <span data-ttu-id="384d8-145">**system**</span><span class="sxs-lookup"><span data-stu-id="384d8-145">**system**</span></span>       | <span data-ttu-id="384d8-146">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="384d8-146">[systemFacet][]</span></span>                  | <span data-ttu-id="384d8-147">Se estiver presente, indica que se trata de uma lista gerenciada pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="384d8-147">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="384d8-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="384d8-148">Read-only.</span></span>

<span data-ttu-id="384d8-149">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="384d8-149">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="384d8-150">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="384d8-150">Property name</span></span>            | <span data-ttu-id="384d8-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="384d8-151">Type</span></span>              | <span data-ttu-id="384d8-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="384d8-152">Description</span></span>
|:-------------------------|:------------------|:------------------------------
| <span data-ttu-id="384d8-153">**id**</span><span class="sxs-lookup"><span data-stu-id="384d8-153">**id**</span></span>                   | <span data-ttu-id="384d8-154">string</span><span class="sxs-lookup"><span data-stu-id="384d8-154">string</span></span>            | <span data-ttu-id="384d8-p104">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="384d8-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="384d8-157">**name**</span><span class="sxs-lookup"><span data-stu-id="384d8-157">**name**</span></span>                 | <span data-ttu-id="384d8-158">string</span><span class="sxs-lookup"><span data-stu-id="384d8-158">string</span></span>            | <span data-ttu-id="384d8-159">O nome do item.</span><span class="sxs-lookup"><span data-stu-id="384d8-159">The name of the item.</span></span>
| <span data-ttu-id="384d8-160">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="384d8-160">**createdBy**</span></span>            | <span data-ttu-id="384d8-161">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="384d8-161">[identitySet][]</span></span>   | <span data-ttu-id="384d8-162">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="384d8-162">Identity of the creator of this item.</span></span> <span data-ttu-id="384d8-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="384d8-163">Read-only.</span></span>
| <span data-ttu-id="384d8-164">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="384d8-164">**createdDateTime**</span></span>      | <span data-ttu-id="384d8-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="384d8-165">DateTimeOffset</span></span>    | <span data-ttu-id="384d8-p106">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="384d8-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="384d8-168">**description**</span><span class="sxs-lookup"><span data-stu-id="384d8-168">**description**</span></span>          | <span data-ttu-id="384d8-169">string</span><span class="sxs-lookup"><span data-stu-id="384d8-169">string</span></span>            | <span data-ttu-id="384d8-170">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="384d8-170">The descriptive text for the item.</span></span>
| <span data-ttu-id="384d8-171">**eTag**</span><span class="sxs-lookup"><span data-stu-id="384d8-171">**eTag**</span></span>                 | <span data-ttu-id="384d8-172">string</span><span class="sxs-lookup"><span data-stu-id="384d8-172">string</span></span>            | <span data-ttu-id="384d8-p107">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="384d8-p107">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="384d8-175">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="384d8-175">**lastModifiedBy**</span></span>       | <span data-ttu-id="384d8-176">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="384d8-176">[identitySet][]</span></span>   | <span data-ttu-id="384d8-177">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="384d8-177">Identity of the last modifier of this item.</span></span> <span data-ttu-id="384d8-178">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="384d8-178">Read-only.</span></span>
| <span data-ttu-id="384d8-179">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="384d8-179">**lastModifiedDateTime**</span></span> | <span data-ttu-id="384d8-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="384d8-180">DateTimeOffset</span></span>    | <span data-ttu-id="384d8-p109">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="384d8-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="384d8-183">**parentReference**</span><span class="sxs-lookup"><span data-stu-id="384d8-183">**parentReference**</span></span>      | <span data-ttu-id="384d8-184">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="384d8-184">[itemReference][]</span></span> | <span data-ttu-id="384d8-p110">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="384d8-p110">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="384d8-187">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="384d8-187">**sharepointIds**</span></span>        | <span data-ttu-id="384d8-188">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="384d8-188">[sharepointIds][]</span></span> | <span data-ttu-id="384d8-p111">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="384d8-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="384d8-191">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="384d8-191">**webUrl**</span></span>               | <span data-ttu-id="384d8-192">string (url)</span><span class="sxs-lookup"><span data-stu-id="384d8-192">string (url)</span></span>      | <span data-ttu-id="384d8-p112">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="384d8-p112">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="384d8-195">Relações</span><span class="sxs-lookup"><span data-stu-id="384d8-195">Relationships</span></span>

<span data-ttu-id="384d8-196">O recurso **list** tem as seguintes relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="384d8-196">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="384d8-197">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="384d8-197">Relationship name</span></span> | <span data-ttu-id="384d8-198">Tipo</span><span class="sxs-lookup"><span data-stu-id="384d8-198">Type</span></span>                             | <span data-ttu-id="384d8-199">Descrição</span><span class="sxs-lookup"><span data-stu-id="384d8-199">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="384d8-200">**drive**</span><span class="sxs-lookup"><span data-stu-id="384d8-200">**drive**</span></span>         | <span data-ttu-id="384d8-201">[drive][]</span><span class="sxs-lookup"><span data-stu-id="384d8-201">[drive][]</span></span>                        | <span data-ttu-id="384d8-202">Presente somente em bibliotecas de documentos.</span><span class="sxs-lookup"><span data-stu-id="384d8-202">Only present on document libraries.</span></span> <span data-ttu-id="384d8-203">Permite o acesso à lista como um recurso de [unidade][] com [driveItems][driveItem].</span><span class="sxs-lookup"><span data-stu-id="384d8-203">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="384d8-204">**items**</span><span class="sxs-lookup"><span data-stu-id="384d8-204">**items**</span></span>         | <span data-ttu-id="384d8-205">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="384d8-205">Collection([listItem][])</span></span>         | <span data-ttu-id="384d8-206">Todos os itens contidos na lista.</span><span class="sxs-lookup"><span data-stu-id="384d8-206">All items contained in the list.</span></span>
| <span data-ttu-id="384d8-207">**columns**</span><span class="sxs-lookup"><span data-stu-id="384d8-207">**columns**</span></span>       | <span data-ttu-id="384d8-208">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="384d8-208">Collection([columnDefinition][])</span></span> | <span data-ttu-id="384d8-209">A coleção de definições de campo para esta lista.</span><span class="sxs-lookup"><span data-stu-id="384d8-209">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="384d8-210">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="384d8-210">**contentTypes**</span></span>  | <span data-ttu-id="384d8-211">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="384d8-211">Collection([contentType][])</span></span>      | <span data-ttu-id="384d8-212">A coleção de tipos de conteúdo presentes nesta lista.</span><span class="sxs-lookup"><span data-stu-id="384d8-212">The collection of content types present in this list.</span></span>

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
