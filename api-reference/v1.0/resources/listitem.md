---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListItem
ms.openlocfilehash: 0f5afaeff29da6f3a6330975adece44731e014bc
ms.sourcegitcommit: 4bdff5fdaea824c7c1204ec7dd641abc282d32a1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2018
---
# <a name="listitem-resource"></a><span data-ttu-id="71c25-102">Recurso ListItem</span><span class="sxs-lookup"><span data-stu-id="71c25-102">ListItem resource</span></span>

<span data-ttu-id="71c25-103">Este recurso representa um item em uma **[list][]** do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="71c25-103">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="71c25-104">Os valores de coluna na lista estão disponíveis por meio do dicionário `fieldValueSet`.</span><span class="sxs-lookup"><span data-stu-id="71c25-104">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="71c25-105">Tarefas em um listItem</span><span class="sxs-lookup"><span data-stu-id="71c25-105">Tasks on a listItem</span></span>

<span data-ttu-id="71c25-106">As tarefas a seguir estão disponíveis para recursos **listItem**.</span><span class="sxs-lookup"><span data-stu-id="71c25-106">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="71c25-107">Todos os exemplos a seguir referem-se a uma **[list][]**, por exemplo: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="71c25-107">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="71c25-108">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="71c25-108">Common task</span></span>                    | <span data-ttu-id="71c25-109">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="71c25-109">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="71c25-110">[Get][]</span><span class="sxs-lookup"><span data-stu-id="71c25-110">[Get][]</span></span>                        | <span data-ttu-id="71c25-111">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="71c25-111">GET /items/{item-id}</span></span>
| <span data-ttu-id="71c25-112">[Obter valores de coluna][Get]</span><span class="sxs-lookup"><span data-stu-id="71c25-112">[Get column values][Get]</span></span>       | <span data-ttu-id="71c25-113">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="71c25-113">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="71c25-114">[Create][]</span><span class="sxs-lookup"><span data-stu-id="71c25-114">[Create][]</span></span>                     | <span data-ttu-id="71c25-115">POST /items</span><span class="sxs-lookup"><span data-stu-id="71c25-115">POST /items</span></span>
| <span data-ttu-id="71c25-116">[Delete][]</span><span class="sxs-lookup"><span data-stu-id="71c25-116">[Delete][]</span></span>                     | <span data-ttu-id="71c25-117">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="71c25-117">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="71c25-118">[Update][]</span><span class="sxs-lookup"><span data-stu-id="71c25-118">[Update][]</span></span>                     | <span data-ttu-id="71c25-119">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="71c25-119">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="71c25-120">[Atualizar valores de coluna][Update]</span><span class="sxs-lookup"><span data-stu-id="71c25-120">[Update column values][Update]</span></span> | <span data-ttu-id="71c25-121">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="71c25-121">PATCH /items/{item-id}/fields</span></span>

[Get]: ../api/listItem_get.md
[Create]: ../api/listItem_create.md
[Delete]: ../api/listItem_delete.md
[Update]: ../api/listItem_update.md

## <a name="json-representation"></a><span data-ttu-id="71c25-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="71c25-126">JSON representation</span></span>

<span data-ttu-id="71c25-127">Veja a seguir uma representação JSON de um recurso **listItem**.</span><span class="sxs-lookup"><span data-stu-id="71c25-127">Here is a JSON representation of a **listItem** resource.</span></span>

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.listItem",
       "keyProperty": "id" } -->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentType" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },

  /* relationships */
  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },

  /* inherited from baseItem */
  "id": "string",
  "name": "name of resource",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of resource",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="71c25-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="71c25-128">Properties</span></span>

<span data-ttu-id="71c25-129">O recurso **listItem** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="71c25-129">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="71c25-130">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="71c25-130">Property name</span></span> | <span data-ttu-id="71c25-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="71c25-131">Type</span></span>                | <span data-ttu-id="71c25-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="71c25-132">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="71c25-133">contentType</span><span class="sxs-lookup"><span data-stu-id="71c25-133">contentType</span></span>   | <span data-ttu-id="71c25-134">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="71c25-134">[contentTypeInfo][]</span></span> | <span data-ttu-id="71c25-135">O tipo de conteúdo deste item de lista</span><span class="sxs-lookup"><span data-stu-id="71c25-135">The content type of this list item</span></span>
| <span data-ttu-id="71c25-136">campos</span><span class="sxs-lookup"><span data-stu-id="71c25-136">fields</span></span>        | <span data-ttu-id="71c25-137">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="71c25-137">[fieldValueSet][]</span></span>   | <span data-ttu-id="71c25-138">Os valores das colunas definidos neste item de lista.</span><span class="sxs-lookup"><span data-stu-id="71c25-138">The values of the columns set on this list item.</span></span>

<span data-ttu-id="71c25-139">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="71c25-139">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="71c25-140">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="71c25-140">Property name</span></span>        | <span data-ttu-id="71c25-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="71c25-141">Type</span></span>             | <span data-ttu-id="71c25-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="71c25-142">Description</span></span>
|:---------------------|:-----------------|:-----------------------------------
| <span data-ttu-id="71c25-143">id</span><span class="sxs-lookup"><span data-stu-id="71c25-143">id</span></span>                   | <span data-ttu-id="71c25-144">string</span><span class="sxs-lookup"><span data-stu-id="71c25-144">string</span></span>           | <span data-ttu-id="71c25-p103">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="71c25-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="71c25-147">name</span><span class="sxs-lookup"><span data-stu-id="71c25-147">name</span></span>                 | <span data-ttu-id="71c25-148">string</span><span class="sxs-lookup"><span data-stu-id="71c25-148">string</span></span>           | <span data-ttu-id="71c25-149">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="71c25-149">The name / title of the item.</span></span>
| <span data-ttu-id="71c25-150">createdBy</span><span class="sxs-lookup"><span data-stu-id="71c25-150">createdBy</span></span>            | <span data-ttu-id="71c25-151">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="71c25-151">[identitySet][]</span></span>  | <span data-ttu-id="71c25-152">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="71c25-152">Identity of the creator of this item.</span></span> <span data-ttu-id="71c25-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="71c25-153">Read-only.</span></span>
| <span data-ttu-id="71c25-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71c25-154">createdDateTime</span></span>      | <span data-ttu-id="71c25-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71c25-155">DateTimeOffset</span></span>   | <span data-ttu-id="71c25-p105">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="71c25-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="71c25-158">description</span><span class="sxs-lookup"><span data-stu-id="71c25-158">description</span></span>          | <span data-ttu-id="71c25-159">string</span><span class="sxs-lookup"><span data-stu-id="71c25-159">string</span></span>           | <span data-ttu-id="71c25-160">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="71c25-160">The descriptive text for the item.</span></span>
| <span data-ttu-id="71c25-161">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="71c25-161">lastModifiedBy</span></span>       | <span data-ttu-id="71c25-162">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="71c25-162">[identitySet][]</span></span>  | <span data-ttu-id="71c25-163">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="71c25-163">Identity of the last modifier of this item.</span></span> <span data-ttu-id="71c25-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="71c25-164">Read-only.</span></span>
| <span data-ttu-id="71c25-165">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71c25-165">lastModifiedDateTime</span></span> | <span data-ttu-id="71c25-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71c25-166">DateTimeOffset</span></span>   | <span data-ttu-id="71c25-p107">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="71c25-p107">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="71c25-169">webUrl</span><span class="sxs-lookup"><span data-stu-id="71c25-169">webUrl</span></span>               | <span data-ttu-id="71c25-170">string (url)</span><span class="sxs-lookup"><span data-stu-id="71c25-170">string (url)</span></span>     | <span data-ttu-id="71c25-p108">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="71c25-p108">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="71c25-173">Relações</span><span class="sxs-lookup"><span data-stu-id="71c25-173">Relationships</span></span>

 <span data-ttu-id="71c25-174">O recurso **listItem** tem as seguintes relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="71c25-174">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="71c25-175">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="71c25-175">Relationship name</span></span> | <span data-ttu-id="71c25-176">Tipo</span><span class="sxs-lookup"><span data-stu-id="71c25-176">Type</span></span>                        | <span data-ttu-id="71c25-177">Descrição</span><span class="sxs-lookup"><span data-stu-id="71c25-177">Description</span></span>
|:------------------|:----------------------------|:-------------------------------
| <span data-ttu-id="71c25-178">driveItem</span><span class="sxs-lookup"><span data-stu-id="71c25-178">driveItem</span></span>         | <span data-ttu-id="71c25-179">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="71c25-179">[driveItem][]</span></span>               | <span data-ttu-id="71c25-180">Para bibliotecas de documentos, a relação **driveItem** expõe listItem como um **[driveItem][]**</span><span class="sxs-lookup"><span data-stu-id="71c25-180">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>

[baseItem]: baseItem.md
[contentTypeInfo]: contentTypeInfo.md
[driveItem]: driveItem.md
[fieldValueSet]: fieldValueSet.md
[identitySet]: identitySet.md
[list]: list.md

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
