---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Listar
ms.openlocfilehash: ba0c01ce1887a32bd8b671cf511104e9128b5efb
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="list-resource"></a><span data-ttu-id="54ee0-102">Recurso List</span><span class="sxs-lookup"><span data-stu-id="54ee0-102">List resource</span></span>

<span data-ttu-id="54ee0-103">O recurso **list** representa uma lista em um [site][].</span><span class="sxs-lookup"><span data-stu-id="54ee0-103">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="54ee0-104">Este recurso contém as propriedades de nível superior da lista, incluindo definições de modelo e campo.</span><span class="sxs-lookup"><span data-stu-id="54ee0-104">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="54ee0-105">Tarefas em list</span><span class="sxs-lookup"><span data-stu-id="54ee0-105">Tasks on a list</span></span>

<span data-ttu-id="54ee0-106">As tarefas a seguir estão disponíveis para os recursos list.</span><span class="sxs-lookup"><span data-stu-id="54ee0-106">The following tasks are available for {type} resources.</span></span>
<span data-ttu-id="54ee0-107">**Observação:** esta versão beta só permite navegar por listas, não criar ou atualizá-las.</span><span class="sxs-lookup"><span data-stu-id="54ee0-107">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="54ee0-108">Você pode, no entanto, criar ou atualizar [itens de lista][listItem].</span><span class="sxs-lookup"><span data-stu-id="54ee0-108">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="54ee0-109">Todos os exemplos a seguir referem-se a um site: `https://graph.microsoft.com/beta/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="54ee0-109">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="54ee0-110">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="54ee0-110">Common task</span></span>               | <span data-ttu-id="54ee0-111">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="54ee0-111">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="54ee0-112">[Obter lista][]</span><span class="sxs-lookup"><span data-stu-id="54ee0-112">[Get list][]</span></span>              | <span data-ttu-id="54ee0-113">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="54ee0-113">GET /lists/{list-id}</span></span>
| <span data-ttu-id="54ee0-114">[Enumerar itens de lista][]</span><span class="sxs-lookup"><span data-stu-id="54ee0-114">[Enumerate list items][]</span></span>  | <span data-ttu-id="54ee0-115">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="54ee0-115">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="54ee0-116">[Atualizar item de lista][]</span><span class="sxs-lookup"><span data-stu-id="54ee0-116">[Update list item][]</span></span>      | <span data-ttu-id="54ee0-117">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="54ee0-117">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="54ee0-118">[Excluir item de lista][]</span><span class="sxs-lookup"><span data-stu-id="54ee0-118">[Delete list item][]</span></span>      | <span data-ttu-id="54ee0-119">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="54ee0-119">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="54ee0-120">[Criar item de lista][]</span><span class="sxs-lookup"><span data-stu-id="54ee0-120">[Create list item][]</span></span>      | <span data-ttu-id="54ee0-121">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="54ee0-121">POST /lists/{list-id}</span></span>

[Obter lista]: ../api/list_get.md
[Enumerar itens de lista]: ../api/listitem_list.md
[Atualizar item de lista]: ../api/listItem_update.md
[Excluir item de lista]: ../api/listItem_delete.md
[Criar item de lista]: ../api/listItem_create.md

## <a name="json-representation"></a><span data-ttu-id="54ee0-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="54ee0-127">JSON representation</span></span>

<span data-ttu-id="54ee0-128">Veja a seguir uma representação JSON de um recurso **list**.</span><span class="sxs-lookup"><span data-stu-id="54ee0-128">Here is a JSON representation of a **baseItem** resource.</span></span>

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.list",
       "keyProperty": "id", 
       "optionalProperties": [ "items", "drive"] } -->

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

## <a name="properties"></a><span data-ttu-id="54ee0-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="54ee0-129">Properties</span></span>

<span data-ttu-id="54ee0-130">O recurso **list** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="54ee0-130">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="54ee0-131">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="54ee0-131">Property name</span></span>    | <span data-ttu-id="54ee0-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="54ee0-132">Type</span></span>                             | <span data-ttu-id="54ee0-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="54ee0-133">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="54ee0-134">**columns**</span><span class="sxs-lookup"><span data-stu-id="54ee0-134">**columns**</span></span>      | <span data-ttu-id="54ee0-135">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="54ee0-135">Collection([columnDefinition][])</span></span> | <span data-ttu-id="54ee0-136">A coleção de definições de campo para esta lista.</span><span class="sxs-lookup"><span data-stu-id="54ee0-136">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="54ee0-137">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="54ee0-137">**contentTypes**</span></span> | <span data-ttu-id="54ee0-138">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="54ee0-138">Collection([contentType][])</span></span>      | <span data-ttu-id="54ee0-139">A coleção de tipos de conteúdo presentes nesta lista.</span><span class="sxs-lookup"><span data-stu-id="54ee0-139">The collection of content types present in this list.</span></span>
| <span data-ttu-id="54ee0-140">**displayName**</span><span class="sxs-lookup"><span data-stu-id="54ee0-140">**displayName**</span></span>  | <span data-ttu-id="54ee0-141">string</span><span class="sxs-lookup"><span data-stu-id="54ee0-141">string</span></span>                           | <span data-ttu-id="54ee0-142">O título em exibição da lista.</span><span class="sxs-lookup"><span data-stu-id="54ee0-142">The displayable title of the list.</span></span>
| <span data-ttu-id="54ee0-143">**list**</span><span class="sxs-lookup"><span data-stu-id="54ee0-143">**list**</span></span>         | <span data-ttu-id="54ee0-144">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="54ee0-144">[listInfo][]</span></span>                     | <span data-ttu-id="54ee0-145">Fornece mais detalhes sobre a lista.</span><span class="sxs-lookup"><span data-stu-id="54ee0-145">Provides additional details about the list.</span></span>
| <span data-ttu-id="54ee0-146">**system**</span><span class="sxs-lookup"><span data-stu-id="54ee0-146">**System**</span></span>       | <span data-ttu-id="54ee0-147">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="54ee0-147">[systemFacet][]</span></span>                  | <span data-ttu-id="54ee0-148">Se estiver presente, indica que se trata de uma lista gerenciada pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="54ee0-148">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="54ee0-149">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54ee0-149">Read-only.</span></span>

<span data-ttu-id="54ee0-150">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="54ee0-150">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="54ee0-151">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="54ee0-151">Property name</span></span>            | <span data-ttu-id="54ee0-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="54ee0-152">Type</span></span>             | <span data-ttu-id="54ee0-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="54ee0-153">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="54ee0-154">**id**</span><span class="sxs-lookup"><span data-stu-id="54ee0-154">**id**</span></span>                   | <span data-ttu-id="54ee0-155">string</span><span class="sxs-lookup"><span data-stu-id="54ee0-155">string</span></span>           | <span data-ttu-id="54ee0-p104">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54ee0-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="54ee0-158">**name**</span><span class="sxs-lookup"><span data-stu-id="54ee0-158">**name**</span></span>                 | <span data-ttu-id="54ee0-159">string</span><span class="sxs-lookup"><span data-stu-id="54ee0-159">string</span></span>           | <span data-ttu-id="54ee0-160">O nome do item.</span><span class="sxs-lookup"><span data-stu-id="54ee0-160">The name of the item.</span></span>
| <span data-ttu-id="54ee0-161">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="54ee0-161">**createdBy**</span></span>            | <span data-ttu-id="54ee0-162">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="54ee0-162">[identitySet][]</span></span>  | <span data-ttu-id="54ee0-163">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="54ee0-163">Identity of the creator of this item.</span></span> <span data-ttu-id="54ee0-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54ee0-164">Read-only.</span></span>
| <span data-ttu-id="54ee0-165">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="54ee0-165">**createdDateTime**</span></span>      | <span data-ttu-id="54ee0-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54ee0-166">DateTimeOffset</span></span>   | <span data-ttu-id="54ee0-p106">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54ee0-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="54ee0-169">**description**</span><span class="sxs-lookup"><span data-stu-id="54ee0-169">**description**</span></span>          | <span data-ttu-id="54ee0-170">string</span><span class="sxs-lookup"><span data-stu-id="54ee0-170">string</span></span>           | <span data-ttu-id="54ee0-171">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="54ee0-171">The descriptive text for the site.</span></span>
| <span data-ttu-id="54ee0-172">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="54ee0-172">**lastModifiedBy**</span></span>       | <span data-ttu-id="54ee0-173">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="54ee0-173">[identitySet][]</span></span>  | <span data-ttu-id="54ee0-174">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="54ee0-174">Identity of the last modifier of this item.</span></span> <span data-ttu-id="54ee0-175">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54ee0-175">Read-only.</span></span>
| <span data-ttu-id="54ee0-176">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="54ee0-176">**lastModifiedDateTime**</span></span> | <span data-ttu-id="54ee0-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54ee0-177">DateTimeOffset</span></span>   | <span data-ttu-id="54ee0-p108">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54ee0-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="54ee0-180">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="54ee0-180">**webUrl**</span></span>               | <span data-ttu-id="54ee0-181">string (url)</span><span class="sxs-lookup"><span data-stu-id="54ee0-181">string (url)</span></span>     | <span data-ttu-id="54ee0-p109">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54ee0-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="54ee0-184">Relações</span><span class="sxs-lookup"><span data-stu-id="54ee0-184">Relationships</span></span>

<span data-ttu-id="54ee0-185">O recurso **list** tem as seguintes relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="54ee0-185">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="54ee0-186">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="54ee0-186">Relationship name</span></span> | <span data-ttu-id="54ee0-187">Tipo</span><span class="sxs-lookup"><span data-stu-id="54ee0-187">Type</span></span>                        | <span data-ttu-id="54ee0-188">Descrição</span><span class="sxs-lookup"><span data-stu-id="54ee0-188">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="54ee0-189">**drive**</span><span class="sxs-lookup"><span data-stu-id="54ee0-189">**drive**</span></span>         | <span data-ttu-id="54ee0-190">[drive][]</span><span class="sxs-lookup"><span data-stu-id="54ee0-190">[drive][]</span></span>                   | <span data-ttu-id="54ee0-191">Presente somente em bibliotecas de documentos.</span><span class="sxs-lookup"><span data-stu-id="54ee0-191">Only present on document libraries.</span></span> <span data-ttu-id="54ee0-192">Permite o acesso à lista como um recurso [drive][] com [driveItems][driveItem].</span><span class="sxs-lookup"><span data-stu-id="54ee0-192">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="54ee0-193">**items**</span><span class="sxs-lookup"><span data-stu-id="54ee0-193">**items**</span></span>         | <span data-ttu-id="54ee0-194">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="54ee0-194">Collection([listItem][])</span></span>    | <span data-ttu-id="54ee0-195">Todos os itens contidos na lista.</span><span class="sxs-lookup"><span data-stu-id="54ee0-195">All items contained in the drive.</span></span>

[baseItem]: baseItem.md
[contentType]: contentType.md
[drive]: drive.md
[driveItem]: driveItem.md
[columnDefinition]: columnDefinition.md
[identitySet]: identitySet.md
[listInfo]: listInfo.md
[listItem]: listItem.md
[site]: site.md
[systemFacet]: systemFacet.md

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
