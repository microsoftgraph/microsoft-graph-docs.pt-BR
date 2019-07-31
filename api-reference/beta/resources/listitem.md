---
author: JeremyKelley
description: Este recurso representa um item em uma list do SharePoint.
ms.date: 09/11/2017
title: ListItem
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 3c05125257eeec9d7b21a7d1eb03de79bc189ccd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009976"
---
# <a name="listitem-resource"></a><span data-ttu-id="ca032-103">Recurso ListItem</span><span class="sxs-lookup"><span data-stu-id="ca032-103">ListItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca032-104">Este recurso representa um item em uma **[list][]** do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ca032-104">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="ca032-105">Os valores de coluna na lista estão disponíveis por meio do dicionário `fieldValueSet`.</span><span class="sxs-lookup"><span data-stu-id="ca032-105">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="ca032-106">Tarefas em um listItem</span><span class="sxs-lookup"><span data-stu-id="ca032-106">Tasks on a listItem</span></span>

<span data-ttu-id="ca032-107">As tarefas a seguir estão disponíveis para recursos **listItem**.</span><span class="sxs-lookup"><span data-stu-id="ca032-107">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="ca032-108">Todos os exemplos a seguir referem-se a uma **[list][]**, por exemplo: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="ca032-108">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="ca032-109">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="ca032-109">Common task</span></span>                    | <span data-ttu-id="ca032-110">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="ca032-110">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="ca032-111">[Get][]</span><span class="sxs-lookup"><span data-stu-id="ca032-111">[Get][]</span></span>                        | <span data-ttu-id="ca032-112">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="ca032-112">GET /items/{item-id}</span></span>
| <span data-ttu-id="ca032-113">[Obter valores de coluna][Get]</span><span class="sxs-lookup"><span data-stu-id="ca032-113">[Get column values][Get]</span></span>       | <span data-ttu-id="ca032-114">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="ca032-114">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="ca032-115">[Obter análises][]</span><span class="sxs-lookup"><span data-stu-id="ca032-115">[Get analytics][]</span></span>              | <span data-ttu-id="ca032-116">OBTER/Items/{Item-ID}/Analytics</span><span class="sxs-lookup"><span data-stu-id="ca032-116">GET /items/{item-id}/analytics</span></span>
| <span data-ttu-id="ca032-117">[Obter atividades por intervalo][]</span><span class="sxs-lookup"><span data-stu-id="ca032-117">[Get activities by interval][]</span></span> | <span data-ttu-id="ca032-118">OBTER/items/{item-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="ca032-118">GET /items/{item-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="ca032-119">[Create][]</span><span class="sxs-lookup"><span data-stu-id="ca032-119">[Create][]</span></span>                     | <span data-ttu-id="ca032-120">POST /items</span><span class="sxs-lookup"><span data-stu-id="ca032-120">POST /items</span></span>
| <span data-ttu-id="ca032-121">[Delete][]</span><span class="sxs-lookup"><span data-stu-id="ca032-121">[Delete][]</span></span>                     | <span data-ttu-id="ca032-122">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="ca032-122">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="ca032-123">[Update][]</span><span class="sxs-lookup"><span data-stu-id="ca032-123">[Update][]</span></span>                     | <span data-ttu-id="ca032-124">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="ca032-124">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="ca032-125">[Atualizar valores de coluna][Update]</span><span class="sxs-lookup"><span data-stu-id="ca032-125">[Update column values][Update]</span></span> | <span data-ttu-id="ca032-126">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="ca032-126">PATCH /items/{item-id}/fields</span></span>

[Get]: ../api/listitem-get.md
[Obter análises]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[Obter atividades por intervalo]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md
[Create]: ../api/listitem-create.md
[Delete]: ../api/listitem-delete.md
[Update]: ../api/listitem-update.md

## <a name="json-representation"></a><span data-ttu-id="ca032-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ca032-133">JSON representation</span></span>

<span data-ttu-id="ca032-134">Veja a seguir uma representação JSON de um recurso **listItem**.</span><span class="sxs-lookup"><span data-stu-id="ca032-134">Here is a JSON representation of a **listItem** resource.</span></span>

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
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "analytics": { "@odata.type": "microsoft.graph.itemAnalytics" },
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

## <a name="properties"></a><span data-ttu-id="ca032-135">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ca032-135">Properties</span></span>

<span data-ttu-id="ca032-136">O recurso **listItem** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="ca032-136">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="ca032-137">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="ca032-137">Property name</span></span> | <span data-ttu-id="ca032-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca032-138">Type</span></span>                | <span data-ttu-id="ca032-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca032-139">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="ca032-140">contentType</span><span class="sxs-lookup"><span data-stu-id="ca032-140">contentType</span></span>   | <span data-ttu-id="ca032-141">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="ca032-141">[contentTypeInfo][]</span></span> | <span data-ttu-id="ca032-142">O tipo de conteúdo deste item de lista</span><span class="sxs-lookup"><span data-stu-id="ca032-142">The content type of this list item</span></span>

<span data-ttu-id="ca032-143">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="ca032-143">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="ca032-144">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="ca032-144">Property name</span></span>        | <span data-ttu-id="ca032-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca032-145">Type</span></span>              | <span data-ttu-id="ca032-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca032-146">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="ca032-147">id</span><span class="sxs-lookup"><span data-stu-id="ca032-147">id</span></span>                   | <span data-ttu-id="ca032-148">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca032-148">string</span></span>            | <span data-ttu-id="ca032-p103">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca032-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="ca032-151">name</span><span class="sxs-lookup"><span data-stu-id="ca032-151">name</span></span>                 | <span data-ttu-id="ca032-152">string</span><span class="sxs-lookup"><span data-stu-id="ca032-152">string</span></span>            | <span data-ttu-id="ca032-153">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="ca032-153">The name / title of the item.</span></span>
| <span data-ttu-id="ca032-154">createdBy</span><span class="sxs-lookup"><span data-stu-id="ca032-154">createdBy</span></span>            | <span data-ttu-id="ca032-155">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ca032-155">[identitySet][]</span></span>   | <span data-ttu-id="ca032-156">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="ca032-156">Identity of the creator of this item.</span></span> <span data-ttu-id="ca032-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca032-157">Read-only.</span></span>
| <span data-ttu-id="ca032-158">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ca032-158">createdDateTime</span></span>      | <span data-ttu-id="ca032-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca032-159">DateTimeOffset</span></span>    | <span data-ttu-id="ca032-p105">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca032-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="ca032-162">description</span><span class="sxs-lookup"><span data-stu-id="ca032-162">description</span></span>          | <span data-ttu-id="ca032-163">string</span><span class="sxs-lookup"><span data-stu-id="ca032-163">string</span></span>            | <span data-ttu-id="ca032-164">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="ca032-164">The descriptive text for the item.</span></span>
| <span data-ttu-id="ca032-165">eTag</span><span class="sxs-lookup"><span data-stu-id="ca032-165">eTag</span></span>                 | <span data-ttu-id="ca032-166">string</span><span class="sxs-lookup"><span data-stu-id="ca032-166">string</span></span>            | <span data-ttu-id="ca032-p106">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca032-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="ca032-169">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ca032-169">lastModifiedBy</span></span>       | <span data-ttu-id="ca032-170">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ca032-170">[identitySet][]</span></span>   | <span data-ttu-id="ca032-171">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="ca032-171">Identity of the last modifier of this item.</span></span> <span data-ttu-id="ca032-172">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca032-172">Read-only.</span></span>
| <span data-ttu-id="ca032-173">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca032-173">lastModifiedDateTime</span></span> | <span data-ttu-id="ca032-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca032-174">DateTimeOffset</span></span>    | <span data-ttu-id="ca032-p108">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca032-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="ca032-177">parentReference</span><span class="sxs-lookup"><span data-stu-id="ca032-177">parentReference</span></span>      | <span data-ttu-id="ca032-178">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="ca032-178">[itemReference][]</span></span> | <span data-ttu-id="ca032-p109">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="ca032-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="ca032-181">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="ca032-181">sharepointIds</span></span>        | <span data-ttu-id="ca032-182">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="ca032-182">[sharepointIds][]</span></span> | <span data-ttu-id="ca032-p110">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca032-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="ca032-185">webUrl</span><span class="sxs-lookup"><span data-stu-id="ca032-185">webUrl</span></span>               | <span data-ttu-id="ca032-186">string (url)</span><span class="sxs-lookup"><span data-stu-id="ca032-186">string (url)</span></span>      | <span data-ttu-id="ca032-p111">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca032-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="ca032-189">Relações</span><span class="sxs-lookup"><span data-stu-id="ca032-189">Relationships</span></span>

 <span data-ttu-id="ca032-190">O recurso **listItem** tem as seguintes relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="ca032-190">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="ca032-191">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="ca032-191">Relationship name</span></span> | <span data-ttu-id="ca032-192">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca032-192">Type</span></span>                           | <span data-ttu-id="ca032-193">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca032-193">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="ca032-194">activities</span><span class="sxs-lookup"><span data-stu-id="ca032-194">activities</span></span>        | <span data-ttu-id="ca032-195">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="ca032-195">[itemActivity][] collection</span></span>    | <span data-ttu-id="ca032-196">A lista de atividades recentes que ocorreram neste item.</span><span class="sxs-lookup"><span data-stu-id="ca032-196">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="ca032-197">análise</span><span class="sxs-lookup"><span data-stu-id="ca032-197">analytics</span></span>         | <span data-ttu-id="ca032-198">recurso [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="ca032-198">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="ca032-199">Análise sobre as atividades de visualização que ocorreram neste item.</span><span class="sxs-lookup"><span data-stu-id="ca032-199">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="ca032-200">driveItem</span><span class="sxs-lookup"><span data-stu-id="ca032-200">driveItem</span></span>         | <span data-ttu-id="ca032-201">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="ca032-201">[driveItem][]</span></span>                  | <span data-ttu-id="ca032-202">Para bibliotecas de documentos, a relação **driveItem** expõe listItem como um **[driveItem][]**</span><span class="sxs-lookup"><span data-stu-id="ca032-202">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="ca032-203">campos</span><span class="sxs-lookup"><span data-stu-id="ca032-203">fields</span></span>            | <span data-ttu-id="ca032-204">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="ca032-204">[fieldValueSet][]</span></span>              | <span data-ttu-id="ca032-205">Os valores das colunas definidos neste item de lista.</span><span class="sxs-lookup"><span data-stu-id="ca032-205">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="ca032-206">versões</span><span class="sxs-lookup"><span data-stu-id="ca032-206">versions</span></span>          | <span data-ttu-id="ca032-207">coleção [listItemVersion][] </span><span class="sxs-lookup"><span data-stu-id="ca032-207">[listItemVersion][] collection</span></span> | <span data-ttu-id="ca032-208">A lista de versões anteriores do item de lista.</span><span class="sxs-lookup"><span data-stu-id="ca032-208">The list of previous versions of the list item.</span></span>

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[driveItem]: driveitem.md
[fieldValueSet]: fieldvalueset.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[list]: list.md
[listItemVersion]: listitemversion.md
[sharepointIds]: sharepointids.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ListItem",
  "tocBookmarks": {
    "ListItem": "#"
  },
  "suppressions": []
}
-->
