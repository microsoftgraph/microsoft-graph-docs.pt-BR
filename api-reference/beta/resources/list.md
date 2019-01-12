---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Listar
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 419f35226c09c1bde500994b6e023f764c54b3cc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953612"
---
# <a name="list-resource"></a><span data-ttu-id="8697e-102">Recurso List</span><span class="sxs-lookup"><span data-stu-id="8697e-102">List resource</span></span>

> <span data-ttu-id="8697e-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8697e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8697e-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8697e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8697e-105">O recurso **list** representa uma lista em um [site][].</span><span class="sxs-lookup"><span data-stu-id="8697e-105">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="8697e-106">Este recurso contém as propriedades de nível superior da lista, incluindo definições de modelo e campo.</span><span class="sxs-lookup"><span data-stu-id="8697e-106">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="8697e-107">Tarefas em list</span><span class="sxs-lookup"><span data-stu-id="8697e-107">Tasks on a list</span></span>

<span data-ttu-id="8697e-108">As tarefas a seguir estão disponíveis para os recursos list.</span><span class="sxs-lookup"><span data-stu-id="8697e-108">The following tasks are available for list resources.</span></span>
<span data-ttu-id="8697e-109">**Observação:** esta versão beta só permite navegar por listas, não criar ou atualizá-las.</span><span class="sxs-lookup"><span data-stu-id="8697e-109">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="8697e-110">Você pode, no entanto, criar ou atualizar [itens de lista][listItem].</span><span class="sxs-lookup"><span data-stu-id="8697e-110">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="8697e-111">Todos os exemplos a seguir referem-se a um site: `https://graph.microsoft.com/beta/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="8697e-111">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="8697e-112">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="8697e-112">Common task</span></span>               | <span data-ttu-id="8697e-113">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="8697e-113">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="8697e-114">[Obter lista][]</span><span class="sxs-lookup"><span data-stu-id="8697e-114">[Get list][]</span></span>              | <span data-ttu-id="8697e-115">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="8697e-115">GET /lists/{list-id}</span></span>
| <span data-ttu-id="8697e-116">[Enumerar itens de lista][]</span><span class="sxs-lookup"><span data-stu-id="8697e-116">[Enumerate list items][]</span></span>  | <span data-ttu-id="8697e-117">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="8697e-117">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="8697e-118">[Atualizar item de lista][]</span><span class="sxs-lookup"><span data-stu-id="8697e-118">[Update list item][]</span></span>      | <span data-ttu-id="8697e-119">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="8697e-119">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="8697e-120">[Excluir item de lista][]</span><span class="sxs-lookup"><span data-stu-id="8697e-120">[Delete list item][]</span></span>      | <span data-ttu-id="8697e-121">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="8697e-121">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="8697e-122">[Criar item de lista][]</span><span class="sxs-lookup"><span data-stu-id="8697e-122">[Create list item][]</span></span>      | <span data-ttu-id="8697e-123">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="8697e-123">POST /lists/{list-id}</span></span>
| <span data-ttu-id="8697e-124">[Obter atividades recentes][]</span><span class="sxs-lookup"><span data-stu-id="8697e-124">[Get recent activities][]</span></span> | <span data-ttu-id="8697e-125">GET /lists/{list-id}/activities</span><span class="sxs-lookup"><span data-stu-id="8697e-125">GET /lists/{list-id}/activities</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="8697e-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8697e-132">JSON representation</span></span>

<span data-ttu-id="8697e-133">Veja a seguir uma representação JSON de um recurso **list**.</span><span class="sxs-lookup"><span data-stu-id="8697e-133">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="8697e-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8697e-134">Properties</span></span>

<span data-ttu-id="8697e-135">O recurso **list** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="8697e-135">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="8697e-136">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="8697e-136">Property name</span></span>    | <span data-ttu-id="8697e-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="8697e-137">Type</span></span>                             | <span data-ttu-id="8697e-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="8697e-138">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="8697e-139">**columns**</span><span class="sxs-lookup"><span data-stu-id="8697e-139">**columns**</span></span>      | <span data-ttu-id="8697e-140">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="8697e-140">Collection([columnDefinition][])</span></span> | <span data-ttu-id="8697e-141">A coleção de definições de campo para esta lista.</span><span class="sxs-lookup"><span data-stu-id="8697e-141">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="8697e-142">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="8697e-142">**contentTypes**</span></span> | <span data-ttu-id="8697e-143">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="8697e-143">Collection([contentType][])</span></span>      | <span data-ttu-id="8697e-144">A coleção de tipos de conteúdo presentes nesta lista.</span><span class="sxs-lookup"><span data-stu-id="8697e-144">The collection of content types present in this list.</span></span>
| <span data-ttu-id="8697e-145">**displayName**</span><span class="sxs-lookup"><span data-stu-id="8697e-145">**displayName**</span></span>  | <span data-ttu-id="8697e-146">string</span><span class="sxs-lookup"><span data-stu-id="8697e-146">string</span></span>                           | <span data-ttu-id="8697e-147">O título em exibição da lista.</span><span class="sxs-lookup"><span data-stu-id="8697e-147">The displayable title of the list.</span></span>
| <span data-ttu-id="8697e-148">**list**</span><span class="sxs-lookup"><span data-stu-id="8697e-148">**list**</span></span>         | <span data-ttu-id="8697e-149">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="8697e-149">[listInfo][]</span></span>                     | <span data-ttu-id="8697e-150">Fornece mais detalhes sobre a lista.</span><span class="sxs-lookup"><span data-stu-id="8697e-150">Provides additional details about the list.</span></span>
| <span data-ttu-id="8697e-151">**system**</span><span class="sxs-lookup"><span data-stu-id="8697e-151">**system**</span></span>       | <span data-ttu-id="8697e-152">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="8697e-152">[systemFacet][]</span></span>                  | <span data-ttu-id="8697e-153">Se estiver presente, indica que se trata de uma lista gerenciada pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="8697e-153">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="8697e-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8697e-154">Read-only.</span></span>

<span data-ttu-id="8697e-155">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="8697e-155">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="8697e-156">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="8697e-156">Property name</span></span>            | <span data-ttu-id="8697e-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="8697e-157">Type</span></span>             | <span data-ttu-id="8697e-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="8697e-158">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="8697e-159">**id**</span><span class="sxs-lookup"><span data-stu-id="8697e-159">**id**</span></span>                   | <span data-ttu-id="8697e-160">string</span><span class="sxs-lookup"><span data-stu-id="8697e-160">string</span></span>           | <span data-ttu-id="8697e-p105">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8697e-p105">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="8697e-163">**name**</span><span class="sxs-lookup"><span data-stu-id="8697e-163">**name**</span></span>                 | <span data-ttu-id="8697e-164">string</span><span class="sxs-lookup"><span data-stu-id="8697e-164">string</span></span>           | <span data-ttu-id="8697e-165">O nome do item.</span><span class="sxs-lookup"><span data-stu-id="8697e-165">The name of the item.</span></span>
| <span data-ttu-id="8697e-166">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="8697e-166">**createdBy**</span></span>            | <span data-ttu-id="8697e-167">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="8697e-167">[identitySet][]</span></span>  | <span data-ttu-id="8697e-168">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="8697e-168">Identity of the creator of this item.</span></span> <span data-ttu-id="8697e-169">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8697e-169">Read-only.</span></span>
| <span data-ttu-id="8697e-170">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="8697e-170">**createdDateTime**</span></span>      | <span data-ttu-id="8697e-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8697e-171">DateTimeOffset</span></span>   | <span data-ttu-id="8697e-p107">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8697e-p107">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="8697e-174">**description**</span><span class="sxs-lookup"><span data-stu-id="8697e-174">**description**</span></span>          | <span data-ttu-id="8697e-175">string</span><span class="sxs-lookup"><span data-stu-id="8697e-175">string</span></span>           | <span data-ttu-id="8697e-176">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="8697e-176">The descriptive text for the item.</span></span>
| <span data-ttu-id="8697e-177">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="8697e-177">**lastModifiedBy**</span></span>       | <span data-ttu-id="8697e-178">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="8697e-178">[identitySet][]</span></span>  | <span data-ttu-id="8697e-179">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="8697e-179">Identity of the last modifier of this item.</span></span> <span data-ttu-id="8697e-180">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8697e-180">Read-only.</span></span>
| <span data-ttu-id="8697e-181">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="8697e-181">**lastModifiedDateTime**</span></span> | <span data-ttu-id="8697e-182">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8697e-182">DateTimeOffset</span></span>   | <span data-ttu-id="8697e-p109">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8697e-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="8697e-185">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="8697e-185">**webUrl**</span></span>               | <span data-ttu-id="8697e-186">string (url)</span><span class="sxs-lookup"><span data-stu-id="8697e-186">string (url)</span></span>     | <span data-ttu-id="8697e-p110">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8697e-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="8697e-189">Relações</span><span class="sxs-lookup"><span data-stu-id="8697e-189">Relationships</span></span>

<span data-ttu-id="8697e-190">O recurso **list** tem as seguintes relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="8697e-190">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="8697e-191">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="8697e-191">Relationship name</span></span> | <span data-ttu-id="8697e-192">Tipo</span><span class="sxs-lookup"><span data-stu-id="8697e-192">Type</span></span>                        | <span data-ttu-id="8697e-193">Descrição</span><span class="sxs-lookup"><span data-stu-id="8697e-193">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="8697e-194">**activities**</span><span class="sxs-lookup"><span data-stu-id="8697e-194">**activities**</span></span>    | <span data-ttu-id="8697e-195">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="8697e-195">[itemActivity][] collection</span></span> | <span data-ttu-id="8697e-196">As atividades recentes que ocorreram nesta lista.</span><span class="sxs-lookup"><span data-stu-id="8697e-196">The recent activities that took place within this list.</span></span>
| <span data-ttu-id="8697e-197">**drive**</span><span class="sxs-lookup"><span data-stu-id="8697e-197">**drive**</span></span>         | <span data-ttu-id="8697e-198">[drive][]</span><span class="sxs-lookup"><span data-stu-id="8697e-198">[drive][]</span></span>                   | <span data-ttu-id="8697e-199">Presente somente em bibliotecas de documentos.</span><span class="sxs-lookup"><span data-stu-id="8697e-199">Only present on document libraries.</span></span> <span data-ttu-id="8697e-200">Permite o acesso à lista como um recurso [drive][] com [driveItems][driveItem].</span><span class="sxs-lookup"><span data-stu-id="8697e-200">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="8697e-201">**items**</span><span class="sxs-lookup"><span data-stu-id="8697e-201">**items**</span></span>         | <span data-ttu-id="8697e-202">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="8697e-202">Collection([listItem][])</span></span>    | <span data-ttu-id="8697e-203">Todos os itens contidos na lista.</span><span class="sxs-lookup"><span data-stu-id="8697e-203">All items contained in the list.</span></span>

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
