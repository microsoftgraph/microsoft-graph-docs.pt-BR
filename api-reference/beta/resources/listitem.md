---
author: JeremyKelley
description: Este recurso representa um item em uma list do SharePoint.
ms.date: 09/11/2017
title: ListItem
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 03f3dae851cf9a23dbe300f834846046dce4de74
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522943"
---
# <a name="listitem-resource"></a><span data-ttu-id="b4cb5-103">Recurso ListItem</span><span class="sxs-lookup"><span data-stu-id="b4cb5-103">ListItem resource</span></span>

<span data-ttu-id="b4cb5-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b4cb5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4cb5-105">Este recurso representa um item em uma **[list][]** do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-105">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="b4cb5-106">Os valores de coluna na lista estão disponíveis por meio do dicionário `fieldValueSet`.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-106">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="b4cb5-107">Tarefas em um listItem</span><span class="sxs-lookup"><span data-stu-id="b4cb5-107">Tasks on a listItem</span></span>

<span data-ttu-id="b4cb5-108">As tarefas a seguir estão disponíveis para recursos **listItem**.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-108">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="b4cb5-109">Todos os exemplos a seguir referem-se a uma **[list][]**, por exemplo: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-109">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="b4cb5-110">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="b4cb5-110">Common task</span></span>                    | <span data-ttu-id="b4cb5-111">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="b4cb5-111">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="b4cb5-112">[Get][]</span><span class="sxs-lookup"><span data-stu-id="b4cb5-112">[Get][]</span></span>                        | <span data-ttu-id="b4cb5-113">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="b4cb5-113">GET /items/{item-id}</span></span>
| <span data-ttu-id="b4cb5-114">[Obter valores de coluna][Get]</span><span class="sxs-lookup"><span data-stu-id="b4cb5-114">[Get column values][Get]</span></span>       | <span data-ttu-id="b4cb5-115">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="b4cb5-115">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="b4cb5-116">[Obter análises][]</span><span class="sxs-lookup"><span data-stu-id="b4cb5-116">[Get analytics][]</span></span>              | <span data-ttu-id="b4cb5-117">OBTER/Items/{Item-ID}/Analytics</span><span class="sxs-lookup"><span data-stu-id="b4cb5-117">GET /items/{item-id}/analytics</span></span>
| <span data-ttu-id="b4cb5-118">[Obter atividades por intervalo][]</span><span class="sxs-lookup"><span data-stu-id="b4cb5-118">[Get activities by interval][]</span></span> | <span data-ttu-id="b4cb5-119">OBTER/items/{item-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="b4cb5-119">GET /items/{item-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="b4cb5-120">[Create][]</span><span class="sxs-lookup"><span data-stu-id="b4cb5-120">[Create][]</span></span>                     | <span data-ttu-id="b4cb5-121">POST /items</span><span class="sxs-lookup"><span data-stu-id="b4cb5-121">POST /items</span></span>
| <span data-ttu-id="b4cb5-122">[Delete][]</span><span class="sxs-lookup"><span data-stu-id="b4cb5-122">[Delete][]</span></span>                     | <span data-ttu-id="b4cb5-123">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="b4cb5-123">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="b4cb5-124">[Update][]</span><span class="sxs-lookup"><span data-stu-id="b4cb5-124">[Update][]</span></span>                     | <span data-ttu-id="b4cb5-125">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="b4cb5-125">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="b4cb5-126">[Atualizar valores de coluna][Update]</span><span class="sxs-lookup"><span data-stu-id="b4cb5-126">[Update column values][Update]</span></span> | <span data-ttu-id="b4cb5-127">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="b4cb5-127">PATCH /items/{item-id}/fields</span></span>

[Get]: ../api/listitem-get.md
[Obter análises]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[Obter atividades por intervalo]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md
[Create]: ../api/listitem-create.md
[Delete]: ../api/listitem-delete.md
[Update]: ../api/listitem-update.md

## <a name="json-representation"></a><span data-ttu-id="b4cb5-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b4cb5-134">JSON representation</span></span>

<span data-ttu-id="b4cb5-135">Veja a seguir uma representação JSON de um recurso **listItem**.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-135">Here is a JSON representation of a **listItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="b4cb5-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b4cb5-136">Properties</span></span>

<span data-ttu-id="b4cb5-137">O recurso **listItem** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-137">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="b4cb5-138">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="b4cb5-138">Property name</span></span> | <span data-ttu-id="b4cb5-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4cb5-139">Type</span></span>                | <span data-ttu-id="b4cb5-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4cb5-140">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="b4cb5-141">contentType</span><span class="sxs-lookup"><span data-stu-id="b4cb5-141">contentType</span></span>   | <span data-ttu-id="b4cb5-142">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="b4cb5-142">[contentTypeInfo][]</span></span> | <span data-ttu-id="b4cb5-143">O tipo de conteúdo deste item de lista</span><span class="sxs-lookup"><span data-stu-id="b4cb5-143">The content type of this list item</span></span>

<span data-ttu-id="b4cb5-144">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-144">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="b4cb5-145">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="b4cb5-145">Property name</span></span>        | <span data-ttu-id="b4cb5-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4cb5-146">Type</span></span>              | <span data-ttu-id="b4cb5-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4cb5-147">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="b4cb5-148">id</span><span class="sxs-lookup"><span data-stu-id="b4cb5-148">id</span></span>                   | <span data-ttu-id="b4cb5-149">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b4cb5-149">string</span></span>            | <span data-ttu-id="b4cb5-p103">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="b4cb5-152">name</span><span class="sxs-lookup"><span data-stu-id="b4cb5-152">name</span></span>                 | <span data-ttu-id="b4cb5-153">string</span><span class="sxs-lookup"><span data-stu-id="b4cb5-153">string</span></span>            | <span data-ttu-id="b4cb5-154">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-154">The name / title of the item.</span></span>
| <span data-ttu-id="b4cb5-155">createdBy</span><span class="sxs-lookup"><span data-stu-id="b4cb5-155">createdBy</span></span>            | <span data-ttu-id="b4cb5-156">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="b4cb5-156">[identitySet][]</span></span>   | <span data-ttu-id="b4cb5-157">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-157">Identity of the creator of this item.</span></span> <span data-ttu-id="b4cb5-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-158">Read-only.</span></span>
| <span data-ttu-id="b4cb5-159">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b4cb5-159">createdDateTime</span></span>      | <span data-ttu-id="b4cb5-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4cb5-160">DateTimeOffset</span></span>    | <span data-ttu-id="b4cb5-p105">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="b4cb5-163">description</span><span class="sxs-lookup"><span data-stu-id="b4cb5-163">description</span></span>          | <span data-ttu-id="b4cb5-164">string</span><span class="sxs-lookup"><span data-stu-id="b4cb5-164">string</span></span>            | <span data-ttu-id="b4cb5-165">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-165">The descriptive text for the item.</span></span>
| <span data-ttu-id="b4cb5-166">eTag</span><span class="sxs-lookup"><span data-stu-id="b4cb5-166">eTag</span></span>                 | <span data-ttu-id="b4cb5-167">string</span><span class="sxs-lookup"><span data-stu-id="b4cb5-167">string</span></span>            | <span data-ttu-id="b4cb5-p106">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="b4cb5-170">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="b4cb5-170">lastModifiedBy</span></span>       | <span data-ttu-id="b4cb5-171">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="b4cb5-171">[identitySet][]</span></span>   | <span data-ttu-id="b4cb5-172">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-172">Identity of the last modifier of this item.</span></span> <span data-ttu-id="b4cb5-173">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-173">Read-only.</span></span>
| <span data-ttu-id="b4cb5-174">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4cb5-174">lastModifiedDateTime</span></span> | <span data-ttu-id="b4cb5-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4cb5-175">DateTimeOffset</span></span>    | <span data-ttu-id="b4cb5-p108">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="b4cb5-178">parentReference</span><span class="sxs-lookup"><span data-stu-id="b4cb5-178">parentReference</span></span>      | <span data-ttu-id="b4cb5-179">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="b4cb5-179">[itemReference][]</span></span> | <span data-ttu-id="b4cb5-p109">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="b4cb5-182">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="b4cb5-182">sharepointIds</span></span>        | <span data-ttu-id="b4cb5-183">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="b4cb5-183">[sharepointIds][]</span></span> | <span data-ttu-id="b4cb5-p110">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="b4cb5-186">webUrl</span><span class="sxs-lookup"><span data-stu-id="b4cb5-186">webUrl</span></span>               | <span data-ttu-id="b4cb5-187">string (url)</span><span class="sxs-lookup"><span data-stu-id="b4cb5-187">string (url)</span></span>      | <span data-ttu-id="b4cb5-p111">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="b4cb5-190">Relações</span><span class="sxs-lookup"><span data-stu-id="b4cb5-190">Relationships</span></span>

 <span data-ttu-id="b4cb5-191">O recurso **listItem** tem as seguintes relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-191">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="b4cb5-192">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="b4cb5-192">Relationship name</span></span> | <span data-ttu-id="b4cb5-193">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4cb5-193">Type</span></span>                           | <span data-ttu-id="b4cb5-194">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4cb5-194">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="b4cb5-195">activities</span><span class="sxs-lookup"><span data-stu-id="b4cb5-195">activities</span></span>        | <span data-ttu-id="b4cb5-196">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="b4cb5-196">[itemActivity][] collection</span></span>    | <span data-ttu-id="b4cb5-197">A lista de atividades recentes que ocorreram neste item.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-197">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="b4cb5-198">análise</span><span class="sxs-lookup"><span data-stu-id="b4cb5-198">analytics</span></span>         | <span data-ttu-id="b4cb5-199">recurso [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="b4cb5-199">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="b4cb5-200">Análise sobre as atividades de visualização que ocorreram neste item.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-200">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="b4cb5-201">driveItem</span><span class="sxs-lookup"><span data-stu-id="b4cb5-201">driveItem</span></span>         | <span data-ttu-id="b4cb5-202">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="b4cb5-202">[driveItem][]</span></span>                  | <span data-ttu-id="b4cb5-203">Para bibliotecas de documentos, a relação **driveItem** expõe listItem como um **[driveItem][]**</span><span class="sxs-lookup"><span data-stu-id="b4cb5-203">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="b4cb5-204">campos</span><span class="sxs-lookup"><span data-stu-id="b4cb5-204">fields</span></span>            | <span data-ttu-id="b4cb5-205">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="b4cb5-205">[fieldValueSet][]</span></span>              | <span data-ttu-id="b4cb5-206">Os valores das colunas definidos neste item de lista.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-206">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="b4cb5-207">versões</span><span class="sxs-lookup"><span data-stu-id="b4cb5-207">versions</span></span>          | <span data-ttu-id="b4cb5-208">coleção [listItemVersion][] </span><span class="sxs-lookup"><span data-stu-id="b4cb5-208">[listItemVersion][] collection</span></span> | <span data-ttu-id="b4cb5-209">A lista de versões anteriores do item de lista.</span><span class="sxs-lookup"><span data-stu-id="b4cb5-209">The list of previous versions of the list item.</span></span>

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
