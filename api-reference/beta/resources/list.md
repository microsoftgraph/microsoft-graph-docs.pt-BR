---
author: JeremyKelley
description: O recurso de lista representa uma lista em um site.
ms.date: 09/11/2017
title: Listar
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 4df869eeba7b66dad0bddef48b7d5686d8899702
ms.sourcegitcommit: f51ba08d604d93f5f6af9ee8979cbf76baa285ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/19/2020
ms.locfileid: "42108459"
---
# <a name="list-resource"></a><span data-ttu-id="75929-103">Recurso List</span><span class="sxs-lookup"><span data-stu-id="75929-103">List resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75929-104">O recurso **list** representa uma lista em um [site][].</span><span class="sxs-lookup"><span data-stu-id="75929-104">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="75929-105">Este recurso contém as propriedades de nível superior da lista, incluindo definições de modelo e campo.</span><span class="sxs-lookup"><span data-stu-id="75929-105">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="75929-106">Tarefas em list</span><span class="sxs-lookup"><span data-stu-id="75929-106">Tasks on a list</span></span>

<span data-ttu-id="75929-107">As tarefas a seguir estão disponíveis para os recursos list.</span><span class="sxs-lookup"><span data-stu-id="75929-107">The following tasks are available for list resources.</span></span>
<span data-ttu-id="75929-108">**Observação:** esta versão beta só permite navegar por listas, não criar ou atualizá-las.</span><span class="sxs-lookup"><span data-stu-id="75929-108">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="75929-109">Você pode, no entanto, criar ou atualizar [itens de lista][listItem].</span><span class="sxs-lookup"><span data-stu-id="75929-109">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="75929-110">Todos os exemplos a seguir referem-se a um site: `https://graph.microsoft.com/beta/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="75929-110">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="75929-111">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="75929-111">Common task</span></span>               | <span data-ttu-id="75929-112">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="75929-112">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="75929-113">[Obter lista][]</span><span class="sxs-lookup"><span data-stu-id="75929-113">[Get list][]</span></span>              | <span data-ttu-id="75929-114">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="75929-114">GET /lists/{list-id}</span></span>
| <span data-ttu-id="75929-115">[Criar lista][]</span><span class="sxs-lookup"><span data-stu-id="75929-115">[Create list][]</span></span>           | <span data-ttu-id="75929-116">POSTAR/Lists</span><span class="sxs-lookup"><span data-stu-id="75929-116">POST /lists</span></span>
| <span data-ttu-id="75929-117">[Enumerar itens de lista][]</span><span class="sxs-lookup"><span data-stu-id="75929-117">[Enumerate list items][]</span></span>  | <span data-ttu-id="75929-118">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="75929-118">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="75929-119">[Atualizar item de lista][]</span><span class="sxs-lookup"><span data-stu-id="75929-119">[Update list item][]</span></span>      | <span data-ttu-id="75929-120">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="75929-120">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="75929-121">[Excluir item de lista][]</span><span class="sxs-lookup"><span data-stu-id="75929-121">[Delete list item][]</span></span>      | <span data-ttu-id="75929-122">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="75929-122">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="75929-123">[Criar item de lista][]</span><span class="sxs-lookup"><span data-stu-id="75929-123">[Create list item][]</span></span>      | <span data-ttu-id="75929-124">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="75929-124">POST /lists/{list-id}</span></span>
| <span data-ttu-id="75929-125">[Obter atividades recentes][]</span><span class="sxs-lookup"><span data-stu-id="75929-125">[Get recent activities][]</span></span> | <span data-ttu-id="75929-126">GET /lists/{list-id}/activities</span><span class="sxs-lookup"><span data-stu-id="75929-126">GET /lists/{list-id}/activities</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="75929-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="75929-134">JSON representation</span></span>

<span data-ttu-id="75929-135">Veja a seguir uma representação JSON de um recurso **list**.</span><span class="sxs-lookup"><span data-stu-id="75929-135">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="75929-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="75929-136">Properties</span></span>

<span data-ttu-id="75929-137">O recurso **list** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="75929-137">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="75929-138">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="75929-138">Property name</span></span>    | <span data-ttu-id="75929-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="75929-139">Type</span></span>                             | <span data-ttu-id="75929-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="75929-140">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="75929-141">**columns**</span><span class="sxs-lookup"><span data-stu-id="75929-141">**columns**</span></span>      | <span data-ttu-id="75929-142">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="75929-142">Collection([columnDefinition][])</span></span> | <span data-ttu-id="75929-143">A coleção de definições de campo para esta lista.</span><span class="sxs-lookup"><span data-stu-id="75929-143">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="75929-144">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="75929-144">**contentTypes**</span></span> | <span data-ttu-id="75929-145">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="75929-145">Collection([contentType][])</span></span>      | <span data-ttu-id="75929-146">A coleção de tipos de conteúdo presentes nesta lista.</span><span class="sxs-lookup"><span data-stu-id="75929-146">The collection of content types present in this list.</span></span>
| <span data-ttu-id="75929-147">**displayName**</span><span class="sxs-lookup"><span data-stu-id="75929-147">**displayName**</span></span>  | <span data-ttu-id="75929-148">string</span><span class="sxs-lookup"><span data-stu-id="75929-148">string</span></span>                           | <span data-ttu-id="75929-149">O título em exibição da lista.</span><span class="sxs-lookup"><span data-stu-id="75929-149">The displayable title of the list.</span></span>
| <span data-ttu-id="75929-150">**list**</span><span class="sxs-lookup"><span data-stu-id="75929-150">**list**</span></span>         | <span data-ttu-id="75929-151">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="75929-151">[listInfo][]</span></span>                     | <span data-ttu-id="75929-152">Fornece mais detalhes sobre a lista.</span><span class="sxs-lookup"><span data-stu-id="75929-152">Provides additional details about the list.</span></span>
| <span data-ttu-id="75929-153">**system**</span><span class="sxs-lookup"><span data-stu-id="75929-153">**system**</span></span>       | <span data-ttu-id="75929-154">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="75929-154">[systemFacet][]</span></span>                  | <span data-ttu-id="75929-155">Se estiver presente, indica que se trata de uma lista gerenciada pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="75929-155">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="75929-156">Apenas leitura.</span><span class="sxs-lookup"><span data-stu-id="75929-156">Read-only.</span></span>

<span data-ttu-id="75929-157">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="75929-157">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="75929-158">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="75929-158">Property name</span></span>            | <span data-ttu-id="75929-159">Tipo</span><span class="sxs-lookup"><span data-stu-id="75929-159">Type</span></span>             | <span data-ttu-id="75929-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="75929-160">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="75929-161">**id**</span><span class="sxs-lookup"><span data-stu-id="75929-161">**id**</span></span>                   | <span data-ttu-id="75929-162">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75929-162">string</span></span>           | <span data-ttu-id="75929-p104">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="75929-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="75929-165">**name**</span><span class="sxs-lookup"><span data-stu-id="75929-165">**name**</span></span>                 | <span data-ttu-id="75929-166">string</span><span class="sxs-lookup"><span data-stu-id="75929-166">string</span></span>           | <span data-ttu-id="75929-167">O nome do item.</span><span class="sxs-lookup"><span data-stu-id="75929-167">The name of the item.</span></span>
| <span data-ttu-id="75929-168">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="75929-168">**createdBy**</span></span>            | <span data-ttu-id="75929-169">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="75929-169">[identitySet][]</span></span>  | <span data-ttu-id="75929-170">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="75929-170">Identity of the creator of this item.</span></span> <span data-ttu-id="75929-171">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="75929-171">Read-only.</span></span>
| <span data-ttu-id="75929-172">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="75929-172">**createdDateTime**</span></span>      | <span data-ttu-id="75929-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75929-173">DateTimeOffset</span></span>   | <span data-ttu-id="75929-p106">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="75929-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="75929-176">**description**</span><span class="sxs-lookup"><span data-stu-id="75929-176">**description**</span></span>          | <span data-ttu-id="75929-177">string</span><span class="sxs-lookup"><span data-stu-id="75929-177">string</span></span>           | <span data-ttu-id="75929-178">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="75929-178">The descriptive text for the item.</span></span>
| <span data-ttu-id="75929-179">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="75929-179">**lastModifiedBy**</span></span>       | <span data-ttu-id="75929-180">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="75929-180">[identitySet][]</span></span>  | <span data-ttu-id="75929-181">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="75929-181">Identity of the last modifier of this item.</span></span> <span data-ttu-id="75929-182">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="75929-182">Read-only.</span></span>
| <span data-ttu-id="75929-183">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="75929-183">**lastModifiedDateTime**</span></span> | <span data-ttu-id="75929-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75929-184">DateTimeOffset</span></span>   | <span data-ttu-id="75929-p108">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="75929-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="75929-187">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="75929-187">**webUrl**</span></span>               | <span data-ttu-id="75929-188">string (url)</span><span class="sxs-lookup"><span data-stu-id="75929-188">string (url)</span></span>     | <span data-ttu-id="75929-p109">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="75929-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="75929-191">Relações</span><span class="sxs-lookup"><span data-stu-id="75929-191">Relationships</span></span>

<span data-ttu-id="75929-192">O recurso **list** tem as seguintes relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="75929-192">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="75929-193">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="75929-193">Relationship name</span></span> | <span data-ttu-id="75929-194">Tipo</span><span class="sxs-lookup"><span data-stu-id="75929-194">Type</span></span>                        | <span data-ttu-id="75929-195">Descrição</span><span class="sxs-lookup"><span data-stu-id="75929-195">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="75929-196">**activities**</span><span class="sxs-lookup"><span data-stu-id="75929-196">**activities**</span></span>    | <span data-ttu-id="75929-197">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="75929-197">[itemActivity][] collection</span></span> | <span data-ttu-id="75929-198">As atividades recentes que ocorreram nesta lista.</span><span class="sxs-lookup"><span data-stu-id="75929-198">The recent activities that took place within this list.</span></span>
| <span data-ttu-id="75929-199">**drive**</span><span class="sxs-lookup"><span data-stu-id="75929-199">**drive**</span></span>         | <span data-ttu-id="75929-200">[drive][]</span><span class="sxs-lookup"><span data-stu-id="75929-200">[drive][]</span></span>                   | <span data-ttu-id="75929-201">Presente somente em bibliotecas de documentos.</span><span class="sxs-lookup"><span data-stu-id="75929-201">Only present on document libraries.</span></span> <span data-ttu-id="75929-202">Permite o acesso à lista como um recurso de [unidade][] com [driveItems][driveItem].</span><span class="sxs-lookup"><span data-stu-id="75929-202">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="75929-203">**items**</span><span class="sxs-lookup"><span data-stu-id="75929-203">**items**</span></span>         | <span data-ttu-id="75929-204">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="75929-204">Collection([listItem][])</span></span>    | <span data-ttu-id="75929-205">Todos os itens contidos na lista.</span><span class="sxs-lookup"><span data-stu-id="75929-205">All items contained in the list.</span></span>

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
