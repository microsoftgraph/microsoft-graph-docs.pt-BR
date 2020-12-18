---
author: JeremyKelley
description: Este recurso representa um item em uma list do SharePoint.
ms.date: 09/11/2017
title: ListItem
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 226213d1361c78f592f92ddfe9b6f52c4f3defd0
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714290"
---
# <a name="listitem-resource"></a><span data-ttu-id="a3aa0-103">Recurso ListItem</span><span class="sxs-lookup"><span data-stu-id="a3aa0-103">ListItem resource</span></span>

<span data-ttu-id="a3aa0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3aa0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3aa0-105">Representa um item em uma [lista][] do Sharepoint.</span><span class="sxs-lookup"><span data-stu-id="a3aa0-105">Represents an item in a SharePoint [list][].</span></span>

<span data-ttu-id="a3aa0-106">Todos os itens em uma biblioteca de documentos do SharePoint podem ser representados como um recurso **ListItem** ou [driveItem][] .</span><span class="sxs-lookup"><span data-stu-id="a3aa0-106">All items in a SharePoint document library can be represented as a **listItem** or [driveItem][] resource.</span></span>

<span data-ttu-id="a3aa0-107">Os valores de coluna na lista estão disponíveis por meio do dicionário `fieldValueSet`.</span><span class="sxs-lookup"><span data-stu-id="a3aa0-107">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="a3aa0-108">Tarefas em um listItem</span><span class="sxs-lookup"><span data-stu-id="a3aa0-108">Tasks on a listItem</span></span>

<span data-ttu-id="a3aa0-109">As tarefas a seguir estão disponíveis para recursos **listItem**.</span><span class="sxs-lookup"><span data-stu-id="a3aa0-109">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="a3aa0-110">Todos os exemplos a seguir referem-se a uma **[list][]**, por exemplo: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="a3aa0-110">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="a3aa0-111">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="a3aa0-111">Common task</span></span>                    | <span data-ttu-id="a3aa0-112">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="a3aa0-112">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="a3aa0-113">[Get][]</span><span class="sxs-lookup"><span data-stu-id="a3aa0-113">[Get][]</span></span>                        | <span data-ttu-id="a3aa0-114">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="a3aa0-114">GET /items/{item-id}</span></span>
| <span data-ttu-id="a3aa0-115">[Obter valores de coluna][Get]</span><span class="sxs-lookup"><span data-stu-id="a3aa0-115">[Get column values][Get]</span></span>       | <span data-ttu-id="a3aa0-116">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="a3aa0-116">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="a3aa0-117">[Obter análises][]</span><span class="sxs-lookup"><span data-stu-id="a3aa0-117">[Get analytics][]</span></span>              | <span data-ttu-id="a3aa0-118">OBTER/Items/{Item-ID}/Analytics</span><span class="sxs-lookup"><span data-stu-id="a3aa0-118">GET /items/{item-id}/analytics</span></span>
| <span data-ttu-id="a3aa0-119">[Obter atividades por intervalo][]</span><span class="sxs-lookup"><span data-stu-id="a3aa0-119">[Get activities by interval][]</span></span> | <span data-ttu-id="a3aa0-120">OBTER/items/{item-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="a3aa0-120">GET /items/{item-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="a3aa0-121">[Create][]</span><span class="sxs-lookup"><span data-stu-id="a3aa0-121">[Create][]</span></span>                     | <span data-ttu-id="a3aa0-122">POST /items</span><span class="sxs-lookup"><span data-stu-id="a3aa0-122">POST /items</span></span>
| <span data-ttu-id="a3aa0-123">[Delete][]</span><span class="sxs-lookup"><span data-stu-id="a3aa0-123">[Delete][]</span></span>                     | <span data-ttu-id="a3aa0-124">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="a3aa0-124">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="a3aa0-125">[Update][]</span><span class="sxs-lookup"><span data-stu-id="a3aa0-125">[Update][]</span></span>                     | <span data-ttu-id="a3aa0-126">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="a3aa0-126">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="a3aa0-127">[Atualizar valores de coluna][Update]</span><span class="sxs-lookup"><span data-stu-id="a3aa0-127">[Update column values][Update]</span></span> | <span data-ttu-id="a3aa0-128">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="a3aa0-128">PATCH /items/{item-id}/fields</span></span>

[Get]: ../api/listitem-get.md
[Obter análises]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[Obter atividades por intervalo]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md
[Create]: ../api/listitem-create.md
[Delete]: ../api/listitem-delete.md
[Update]: ../api/listitem-update.md

## <a name="json-representation"></a><span data-ttu-id="a3aa0-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a3aa0-135">JSON representation</span></span>

<span data-ttu-id="a3aa0-136">Veja a seguir uma representação JSON de um recurso **listItem**.</span><span class="sxs-lookup"><span data-stu-id="a3aa0-136">Here is a JSON representation of a **listItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="a3aa0-137">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a3aa0-137">Properties</span></span>

<span data-ttu-id="a3aa0-138">O recurso **listItem** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="a3aa0-138">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="a3aa0-139">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="a3aa0-139">Property name</span></span> | <span data-ttu-id="a3aa0-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3aa0-140">Type</span></span>                | <span data-ttu-id="a3aa0-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3aa0-141">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="a3aa0-142">contentType</span><span class="sxs-lookup"><span data-stu-id="a3aa0-142">contentType</span></span>   | <span data-ttu-id="a3aa0-143">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="a3aa0-143">[contentTypeInfo][]</span></span> | <span data-ttu-id="a3aa0-144">O tipo de conteúdo deste item de lista</span><span class="sxs-lookup"><span data-stu-id="a3aa0-144">The content type of this list item</span></span>

<span data-ttu-id="a3aa0-145">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="a3aa0-145">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="a3aa0-146">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="a3aa0-146">Property name</span></span>        | <span data-ttu-id="a3aa0-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3aa0-147">Type</span></span>              | <span data-ttu-id="a3aa0-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3aa0-148">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="a3aa0-149">id</span><span class="sxs-lookup"><span data-stu-id="a3aa0-149">id</span></span>                   | <span data-ttu-id="a3aa0-150">string</span><span class="sxs-lookup"><span data-stu-id="a3aa0-150">string</span></span>            | <span data-ttu-id="a3aa0-p102">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a3aa0-p102">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="a3aa0-153">name</span><span class="sxs-lookup"><span data-stu-id="a3aa0-153">name</span></span>                 | <span data-ttu-id="a3aa0-154">string</span><span class="sxs-lookup"><span data-stu-id="a3aa0-154">string</span></span>            | <span data-ttu-id="a3aa0-155">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="a3aa0-155">The name / title of the item.</span></span>
| <span data-ttu-id="a3aa0-156">createdBy</span><span class="sxs-lookup"><span data-stu-id="a3aa0-156">createdBy</span></span>            | <span data-ttu-id="a3aa0-157">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="a3aa0-157">[identitySet][]</span></span>   | <span data-ttu-id="a3aa0-158">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="a3aa0-158">Identity of the creator of this item.</span></span> <span data-ttu-id="a3aa0-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a3aa0-159">Read-only.</span></span>
| <span data-ttu-id="a3aa0-160">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a3aa0-160">createdDateTime</span></span>      | <span data-ttu-id="a3aa0-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3aa0-161">DateTimeOffset</span></span>    | <span data-ttu-id="a3aa0-p104">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a3aa0-p104">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="a3aa0-164">description</span><span class="sxs-lookup"><span data-stu-id="a3aa0-164">description</span></span>          | <span data-ttu-id="a3aa0-165">string</span><span class="sxs-lookup"><span data-stu-id="a3aa0-165">string</span></span>            | <span data-ttu-id="a3aa0-166">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="a3aa0-166">The descriptive text for the item.</span></span>
| <span data-ttu-id="a3aa0-167">eTag</span><span class="sxs-lookup"><span data-stu-id="a3aa0-167">eTag</span></span>                 | <span data-ttu-id="a3aa0-168">string</span><span class="sxs-lookup"><span data-stu-id="a3aa0-168">string</span></span>            | <span data-ttu-id="a3aa0-p105">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a3aa0-p105">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="a3aa0-171">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="a3aa0-171">lastModifiedBy</span></span>       | <span data-ttu-id="a3aa0-172">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="a3aa0-172">[identitySet][]</span></span>   | <span data-ttu-id="a3aa0-173">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="a3aa0-173">Identity of the last modifier of this item.</span></span> <span data-ttu-id="a3aa0-174">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a3aa0-174">Read-only.</span></span>
| <span data-ttu-id="a3aa0-175">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a3aa0-175">lastModifiedDateTime</span></span> | <span data-ttu-id="a3aa0-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3aa0-176">DateTimeOffset</span></span>    | <span data-ttu-id="a3aa0-p107">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a3aa0-p107">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="a3aa0-179">parentReference</span><span class="sxs-lookup"><span data-stu-id="a3aa0-179">parentReference</span></span>      | <span data-ttu-id="a3aa0-180">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="a3aa0-180">[itemReference][]</span></span> | <span data-ttu-id="a3aa0-p108">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="a3aa0-p108">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="a3aa0-183">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="a3aa0-183">sharepointIds</span></span>        | <span data-ttu-id="a3aa0-184">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="a3aa0-184">[sharepointIds][]</span></span> | <span data-ttu-id="a3aa0-p109">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a3aa0-p109">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="a3aa0-187">webUrl</span><span class="sxs-lookup"><span data-stu-id="a3aa0-187">webUrl</span></span>               | <span data-ttu-id="a3aa0-188">string (url)</span><span class="sxs-lookup"><span data-stu-id="a3aa0-188">string (url)</span></span>      | <span data-ttu-id="a3aa0-p110">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a3aa0-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="a3aa0-191">Relações</span><span class="sxs-lookup"><span data-stu-id="a3aa0-191">Relationships</span></span>

 <span data-ttu-id="a3aa0-192">O recurso **listItem** tem as seguintes relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="a3aa0-192">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="a3aa0-193">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="a3aa0-193">Relationship name</span></span> | <span data-ttu-id="a3aa0-194">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3aa0-194">Type</span></span>                           | <span data-ttu-id="a3aa0-195">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3aa0-195">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="a3aa0-196">activities</span><span class="sxs-lookup"><span data-stu-id="a3aa0-196">activities</span></span>        | <span data-ttu-id="a3aa0-197">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="a3aa0-197">[itemActivity][] collection</span></span>    | <span data-ttu-id="a3aa0-198">A lista de atividades recentes que ocorreram neste item.</span><span class="sxs-lookup"><span data-stu-id="a3aa0-198">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="a3aa0-199">análise</span><span class="sxs-lookup"><span data-stu-id="a3aa0-199">analytics</span></span>         | <span data-ttu-id="a3aa0-200">recurso [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="a3aa0-200">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="a3aa0-201">Análise sobre as atividades de visualização que ocorreram neste item.</span><span class="sxs-lookup"><span data-stu-id="a3aa0-201">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="a3aa0-202">driveItem</span><span class="sxs-lookup"><span data-stu-id="a3aa0-202">driveItem</span></span>         | <span data-ttu-id="a3aa0-203">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="a3aa0-203">[driveItem][]</span></span>                  | <span data-ttu-id="a3aa0-204">Para bibliotecas de documentos, a relação **driveItem** expõe listItem como um **[driveItem][]**</span><span class="sxs-lookup"><span data-stu-id="a3aa0-204">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="a3aa0-205">campos</span><span class="sxs-lookup"><span data-stu-id="a3aa0-205">fields</span></span>            | <span data-ttu-id="a3aa0-206">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="a3aa0-206">[fieldValueSet][]</span></span>              | <span data-ttu-id="a3aa0-207">Os valores das colunas definidos neste item de lista.</span><span class="sxs-lookup"><span data-stu-id="a3aa0-207">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="a3aa0-208">versões</span><span class="sxs-lookup"><span data-stu-id="a3aa0-208">versions</span></span>          | <span data-ttu-id="a3aa0-209">coleção [listItemVersion][] </span><span class="sxs-lookup"><span data-stu-id="a3aa0-209">[listItemVersion][] collection</span></span> | <span data-ttu-id="a3aa0-210">A lista de versões anteriores do item de lista.</span><span class="sxs-lookup"><span data-stu-id="a3aa0-210">The list of previous versions of the list item.</span></span>

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


