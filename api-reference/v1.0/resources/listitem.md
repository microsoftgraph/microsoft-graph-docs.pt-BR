---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ListItem
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: ba4b910f6d86caee23ce191b225d040ef023b4e7
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481612"
---
# <a name="listitem-resource"></a><span data-ttu-id="559c9-102">Recurso ListItem</span><span class="sxs-lookup"><span data-stu-id="559c9-102">ListItem resource</span></span>

<span data-ttu-id="559c9-103">Este recurso representa um item em uma **[list][]** do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="559c9-103">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="559c9-104">Os valores de coluna na lista estão disponíveis por meio do dicionário `fieldValueSet`.</span><span class="sxs-lookup"><span data-stu-id="559c9-104">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="559c9-105">Tarefas em um listItem</span><span class="sxs-lookup"><span data-stu-id="559c9-105">Tasks on a listItem</span></span>

<span data-ttu-id="559c9-106">As tarefas a seguir estão disponíveis para recursos **listItem**.</span><span class="sxs-lookup"><span data-stu-id="559c9-106">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="559c9-107">Todos os exemplos a seguir referem-se a uma **[list][]**, por exemplo: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="559c9-107">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="559c9-108">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="559c9-108">Common task</span></span>                    | <span data-ttu-id="559c9-109">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="559c9-109">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="559c9-110">[Get][]</span><span class="sxs-lookup"><span data-stu-id="559c9-110">[Get][]</span></span>                        | <span data-ttu-id="559c9-111">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="559c9-111">GET /items/{item-id}</span></span>
| <span data-ttu-id="559c9-112">[Obter valores de coluna][Get]</span><span class="sxs-lookup"><span data-stu-id="559c9-112">[Get column values][Get]</span></span>       | <span data-ttu-id="559c9-113">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="559c9-113">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="559c9-114">[Create][]</span><span class="sxs-lookup"><span data-stu-id="559c9-114">[Create][]</span></span>                     | <span data-ttu-id="559c9-115">POST /items</span><span class="sxs-lookup"><span data-stu-id="559c9-115">POST /items</span></span>
| <span data-ttu-id="559c9-116">[Delete][]</span><span class="sxs-lookup"><span data-stu-id="559c9-116">[Delete][]</span></span>                     | <span data-ttu-id="559c9-117">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="559c9-117">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="559c9-118">[Update][]</span><span class="sxs-lookup"><span data-stu-id="559c9-118">[Update][]</span></span>                     | <span data-ttu-id="559c9-119">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="559c9-119">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="559c9-120">[Atualizar valores de coluna][Update]</span><span class="sxs-lookup"><span data-stu-id="559c9-120">[Update column values][Update]</span></span> | <span data-ttu-id="559c9-121">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="559c9-121">PATCH /items/{item-id}/fields</span></span>

[Get]: ../api/listitem-get.md
[Create]: ../api/listitem-create.md
[Excluir]: ../api/listitem-delete.md
[Delete]: ../api/listitem-delete.md
[Update]: ../api/listitem-update.md

## <a name="json-representation"></a><span data-ttu-id="559c9-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="559c9-126">JSON representation</span></span>

<span data-ttu-id="559c9-127">Veja a seguir uma representação JSON de um recurso **listItem**.</span><span class="sxs-lookup"><span data-stu-id="559c9-127">Here is a JSON representation of a **listItem** resource.</span></span>

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.listItem"
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },

  /* relationships */
  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
  "versions": [{"@odata.type": "microsoft.graph.listItemVersion"}],

  /* inherited from baseItem */
  "id": "string",
  "name": "name of resource",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of resource",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference"},
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="559c9-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="559c9-128">Properties</span></span>

<span data-ttu-id="559c9-129">O recurso **listItem** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="559c9-129">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="559c9-130">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="559c9-130">Property name</span></span> | <span data-ttu-id="559c9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="559c9-131">Type</span></span>                | <span data-ttu-id="559c9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="559c9-132">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="559c9-133">contentType</span><span class="sxs-lookup"><span data-stu-id="559c9-133">contentType</span></span>   | <span data-ttu-id="559c9-134">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="559c9-134">[contentTypeInfo][]</span></span> | <span data-ttu-id="559c9-135">O tipo de conteúdo deste item de lista</span><span class="sxs-lookup"><span data-stu-id="559c9-135">The content type of this list item</span></span>

<span data-ttu-id="559c9-136">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="559c9-136">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="559c9-137">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="559c9-137">Property name</span></span>        | <span data-ttu-id="559c9-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="559c9-138">Type</span></span>              | <span data-ttu-id="559c9-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="559c9-139">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="559c9-140">id</span><span class="sxs-lookup"><span data-stu-id="559c9-140">id</span></span>                   | <span data-ttu-id="559c9-141">string</span><span class="sxs-lookup"><span data-stu-id="559c9-141">string</span></span>            | <span data-ttu-id="559c9-p103">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="559c9-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="559c9-144">name</span><span class="sxs-lookup"><span data-stu-id="559c9-144">name</span></span>                 | <span data-ttu-id="559c9-145">string</span><span class="sxs-lookup"><span data-stu-id="559c9-145">string</span></span>            | <span data-ttu-id="559c9-146">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="559c9-146">The name / title of the item.</span></span>
| <span data-ttu-id="559c9-147">createdBy</span><span class="sxs-lookup"><span data-stu-id="559c9-147">createdBy</span></span>            | <span data-ttu-id="559c9-148">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="559c9-148">[identitySet][]</span></span>   | <span data-ttu-id="559c9-149">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="559c9-149">Identity of the creator of this item.</span></span> <span data-ttu-id="559c9-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="559c9-150">Read-only.</span></span>
| <span data-ttu-id="559c9-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="559c9-151">createdDateTime</span></span>      | <span data-ttu-id="559c9-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="559c9-152">DateTimeOffset</span></span>    | <span data-ttu-id="559c9-p105">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="559c9-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="559c9-155">description</span><span class="sxs-lookup"><span data-stu-id="559c9-155">description</span></span>          | <span data-ttu-id="559c9-156">string</span><span class="sxs-lookup"><span data-stu-id="559c9-156">string</span></span>            | <span data-ttu-id="559c9-157">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="559c9-157">The descriptive text for the item.</span></span>
| <span data-ttu-id="559c9-158">eTag</span><span class="sxs-lookup"><span data-stu-id="559c9-158">eTag</span></span>                 | <span data-ttu-id="559c9-159">string</span><span class="sxs-lookup"><span data-stu-id="559c9-159">string</span></span>            | <span data-ttu-id="559c9-p106">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="559c9-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="559c9-162">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="559c9-162">lastModifiedBy</span></span>       | <span data-ttu-id="559c9-163">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="559c9-163">[identitySet][]</span></span>   | <span data-ttu-id="559c9-164">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="559c9-164">Identity of the last modifier of this item.</span></span> <span data-ttu-id="559c9-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="559c9-165">Read-only.</span></span>
| <span data-ttu-id="559c9-166">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="559c9-166">lastModifiedDateTime</span></span> | <span data-ttu-id="559c9-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="559c9-167">DateTimeOffset</span></span>    | <span data-ttu-id="559c9-p108">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="559c9-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="559c9-170">parentReference</span><span class="sxs-lookup"><span data-stu-id="559c9-170">parentReference</span></span>      | <span data-ttu-id="559c9-171">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="559c9-171">[itemReference][]</span></span> | <span data-ttu-id="559c9-p109">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="559c9-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="559c9-174">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="559c9-174">sharepointIds</span></span>        | <span data-ttu-id="559c9-175">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="559c9-175">[sharepointIds][]</span></span> | <span data-ttu-id="559c9-p110">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="559c9-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="559c9-178">webUrl</span><span class="sxs-lookup"><span data-stu-id="559c9-178">webUrl</span></span>               | <span data-ttu-id="559c9-179">string (url)</span><span class="sxs-lookup"><span data-stu-id="559c9-179">string (url)</span></span>      | <span data-ttu-id="559c9-p111">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="559c9-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="559c9-182">Relações</span><span class="sxs-lookup"><span data-stu-id="559c9-182">Relationships</span></span>

 <span data-ttu-id="559c9-183">O recurso **listItem** tem as seguintes relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="559c9-183">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="559c9-184">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="559c9-184">Relationship name</span></span> | <span data-ttu-id="559c9-185">Tipo</span><span class="sxs-lookup"><span data-stu-id="559c9-185">Type</span></span>                           | <span data-ttu-id="559c9-186">Descrição</span><span class="sxs-lookup"><span data-stu-id="559c9-186">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="559c9-187">driveItem</span><span class="sxs-lookup"><span data-stu-id="559c9-187">driveItem</span></span>         | <span data-ttu-id="559c9-188">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="559c9-188">[driveItem][]</span></span>                  | <span data-ttu-id="559c9-189">Para bibliotecas de documentos, a relação **driveItem** expõe listItem como um **[driveItem][]**</span><span class="sxs-lookup"><span data-stu-id="559c9-189">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="559c9-190">campos</span><span class="sxs-lookup"><span data-stu-id="559c9-190">fields</span></span>            | <span data-ttu-id="559c9-191">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="559c9-191">[fieldValueSet][]</span></span>              | <span data-ttu-id="559c9-192">Os valores das colunas definidos neste item de lista.</span><span class="sxs-lookup"><span data-stu-id="559c9-192">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="559c9-193">versões</span><span class="sxs-lookup"><span data-stu-id="559c9-193">Versions</span></span>          | <span data-ttu-id="559c9-194">coleção [listItemVersion][] </span><span class="sxs-lookup"><span data-stu-id="559c9-194">[listItemVersion][] collection</span></span> | <span data-ttu-id="559c9-195">A lista de versões anteriores do item de lista.</span><span class="sxs-lookup"><span data-stu-id="559c9-195">The list of previous versions of the list item.</span></span>

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[driveItem]: driveitem.md
[fieldValueSet]: fieldvalueset.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[list]: list.md
[listItemVersion]: listitemversion.md
[sharepointIds]: sharepointids.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ListItem",
  "tocBookmarks": {
    "ListItem": "#"
  }
} -->
