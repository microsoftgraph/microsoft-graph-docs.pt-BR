---
author: JeremyKelley
description: Este recurso representa um item em uma list do SharePoint.
ms.date: 09/11/2017
title: ListItem
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: ad1e278f31bbeb0bc079f1ad2a6345d9b260cdec
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941463"
---
# <a name="listitem-resource"></a><span data-ttu-id="ff351-103">Recurso ListItem</span><span class="sxs-lookup"><span data-stu-id="ff351-103">ListItem resource</span></span>

<span data-ttu-id="ff351-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff351-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff351-105">Representa um item em uma [lista][] do Microsoft Office SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="ff351-105">Represents an item in a SharePoint [list][].</span></span>

<span data-ttu-id="ff351-106">Todos os itens em uma biblioteca de documentos do Microsoft Office SharePoint Online podem ser representados como um **listItem** ou um r [ecurso driveItem][].</span><span class="sxs-lookup"><span data-stu-id="ff351-106">All items in a SharePoint document library can be represented as a **listItem** or [driveItem][] resource.</span></span>

<span data-ttu-id="ff351-107">Os valores de coluna na lista estão disponíveis por meio do dicionário `fieldValueSet`.</span><span class="sxs-lookup"><span data-stu-id="ff351-107">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="ff351-108">Tarefas em um listItem</span><span class="sxs-lookup"><span data-stu-id="ff351-108">Tasks on a listItem</span></span>

<span data-ttu-id="ff351-109">As tarefas a seguir estão disponíveis para recursos **listItem**.</span><span class="sxs-lookup"><span data-stu-id="ff351-109">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="ff351-110">Todos os exemplos a seguir referem-se a uma **[list][]**, por exemplo: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="ff351-110">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="ff351-111">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="ff351-111">Common task</span></span>                    | <span data-ttu-id="ff351-112">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="ff351-112">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="ff351-113">[Get][]</span><span class="sxs-lookup"><span data-stu-id="ff351-113">[Get][]</span></span>                        | <span data-ttu-id="ff351-114">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="ff351-114">GET /items/{item-id}</span></span>
| <span data-ttu-id="ff351-115">[Obter valores de coluna][Get]</span><span class="sxs-lookup"><span data-stu-id="ff351-115">[Get column values][Get]</span></span>       | <span data-ttu-id="ff351-116">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="ff351-116">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="ff351-117">[Obter análises][]</span><span class="sxs-lookup"><span data-stu-id="ff351-117">[Get analytics][]</span></span>              | <span data-ttu-id="ff351-118">GET /items/{item-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="ff351-118">GET /items/{item-id}/analytics</span></span>
| <span data-ttu-id="ff351-119">[Obter atividades por intervalo][]</span><span class="sxs-lookup"><span data-stu-id="ff351-119">[Get activities by interval][]</span></span> | <span data-ttu-id="ff351-120">GET /items/{item-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="ff351-120">GET /items/{item-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="ff351-121">[Create][]</span><span class="sxs-lookup"><span data-stu-id="ff351-121">[Create][]</span></span>                     | <span data-ttu-id="ff351-122">POST /items</span><span class="sxs-lookup"><span data-stu-id="ff351-122">POST /items</span></span>
| <span data-ttu-id="ff351-123">[Delete][]</span><span class="sxs-lookup"><span data-stu-id="ff351-123">[Delete][]</span></span>                     | <span data-ttu-id="ff351-124">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="ff351-124">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="ff351-125">[Update][]</span><span class="sxs-lookup"><span data-stu-id="ff351-125">[Update][]</span></span>                     | <span data-ttu-id="ff351-126">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="ff351-126">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="ff351-127">[Atualizar valores de coluna][Update]</span><span class="sxs-lookup"><span data-stu-id="ff351-127">[Update column values][Update]</span></span> | <span data-ttu-id="ff351-128">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="ff351-128">PATCH /items/{item-id}/fields</span></span>
| <span data-ttu-id="ff351-129">[createLink][CreateLink]</span><span class="sxs-lookup"><span data-stu-id="ff351-129">[createLink][CreateLink]</span></span>       | <span data-ttu-id="ff351-130">POST /items/{itemId}/createLink</span><span class="sxs-lookup"><span data-stu-id="ff351-130">POST /items/{itemId}/createLink</span></span>

[Obter]: ../api/listitem-get.md
[Get]: ../api/listitem-get.md
[Obter análises]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[Obter atividades por intervalo]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md
[Create]: ../api/listitem-create.md
[Delete]: ../api/listitem-delete.md
[Update]: ../api/listitem-update.md
[CreateLink]: ../api/listitem-createlink.md

## <a name="json-representation"></a><span data-ttu-id="ff351-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ff351-137">JSON representation</span></span>

<span data-ttu-id="ff351-138">Veja a seguir uma representação JSON de um recurso **listItem**.</span><span class="sxs-lookup"><span data-stu-id="ff351-138">Here is a JSON representation of a **listItem** resource.</span></span>

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type&quot;: &quot;microsoft.graph.listItem"
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
  "webUrl&quot;: &quot;url"
}
```

## <a name="properties"></a><span data-ttu-id="ff351-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ff351-139">Properties</span></span>

<span data-ttu-id="ff351-140">O recurso **listItem** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="ff351-140">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="ff351-141">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="ff351-141">Property name</span></span> | <span data-ttu-id="ff351-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff351-142">Type</span></span>                | <span data-ttu-id="ff351-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff351-143">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="ff351-144">contentType</span><span class="sxs-lookup"><span data-stu-id="ff351-144">contentType</span></span>   | <span data-ttu-id="ff351-145">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="ff351-145">[contentTypeInfo][]</span></span> | <span data-ttu-id="ff351-146">O tipo de conteúdo deste item de lista</span><span class="sxs-lookup"><span data-stu-id="ff351-146">The content type of this list item</span></span>

<span data-ttu-id="ff351-147">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="ff351-147">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="ff351-148">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="ff351-148">Property name</span></span>        | <span data-ttu-id="ff351-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff351-149">Type</span></span>              | <span data-ttu-id="ff351-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff351-150">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="ff351-151">id</span><span class="sxs-lookup"><span data-stu-id="ff351-151">id</span></span>                   | <span data-ttu-id="ff351-152">string</span><span class="sxs-lookup"><span data-stu-id="ff351-152">string</span></span>            | <span data-ttu-id="ff351-p102">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff351-p102">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="ff351-155">name</span><span class="sxs-lookup"><span data-stu-id="ff351-155">name</span></span>                 | <span data-ttu-id="ff351-156">string</span><span class="sxs-lookup"><span data-stu-id="ff351-156">string</span></span>            | <span data-ttu-id="ff351-157">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="ff351-157">The name / title of the item.</span></span>
| <span data-ttu-id="ff351-158">createdBy</span><span class="sxs-lookup"><span data-stu-id="ff351-158">createdBy</span></span>            | <span data-ttu-id="ff351-159">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ff351-159">[identitySet][]</span></span>   | <span data-ttu-id="ff351-160">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="ff351-160">Identity of the creator of this item.</span></span> <span data-ttu-id="ff351-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff351-161">Read-only.</span></span>
| <span data-ttu-id="ff351-162">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ff351-162">createdDateTime</span></span>      | <span data-ttu-id="ff351-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff351-163">DateTimeOffset</span></span>    | <span data-ttu-id="ff351-p104">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff351-p104">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="ff351-166">description</span><span class="sxs-lookup"><span data-stu-id="ff351-166">description</span></span>          | <span data-ttu-id="ff351-167">string</span><span class="sxs-lookup"><span data-stu-id="ff351-167">string</span></span>            | <span data-ttu-id="ff351-168">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="ff351-168">The descriptive text for the item.</span></span>
| <span data-ttu-id="ff351-169">eTag</span><span class="sxs-lookup"><span data-stu-id="ff351-169">eTag</span></span>                 | <span data-ttu-id="ff351-170">string</span><span class="sxs-lookup"><span data-stu-id="ff351-170">string</span></span>            | <span data-ttu-id="ff351-p105">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff351-p105">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="ff351-173">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ff351-173">lastModifiedBy</span></span>       | <span data-ttu-id="ff351-174">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ff351-174">[identitySet][]</span></span>   | <span data-ttu-id="ff351-175">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="ff351-175">Identity of the last modifier of this item.</span></span> <span data-ttu-id="ff351-176">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff351-176">Read-only.</span></span>
| <span data-ttu-id="ff351-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff351-177">lastModifiedDateTime</span></span> | <span data-ttu-id="ff351-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff351-178">DateTimeOffset</span></span>    | <span data-ttu-id="ff351-p107">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff351-p107">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="ff351-181">parentReference</span><span class="sxs-lookup"><span data-stu-id="ff351-181">parentReference</span></span>      | <span data-ttu-id="ff351-182">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="ff351-182">[itemReference][]</span></span> | <span data-ttu-id="ff351-p108">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="ff351-p108">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="ff351-185">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="ff351-185">sharepointIds</span></span>        | <span data-ttu-id="ff351-186">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="ff351-186">[sharepointIds][]</span></span> | <span data-ttu-id="ff351-p109">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff351-p109">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="ff351-189">webUrl</span><span class="sxs-lookup"><span data-stu-id="ff351-189">webUrl</span></span>               | <span data-ttu-id="ff351-190">string (url)</span><span class="sxs-lookup"><span data-stu-id="ff351-190">string (url)</span></span>      | <span data-ttu-id="ff351-p110">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff351-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="ff351-193">Relações</span><span class="sxs-lookup"><span data-stu-id="ff351-193">Relationships</span></span>

 <span data-ttu-id="ff351-194">O recurso **listItem** tem as seguintes relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="ff351-194">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="ff351-195">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="ff351-195">Relationship name</span></span> | <span data-ttu-id="ff351-196">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff351-196">Type</span></span>                           | <span data-ttu-id="ff351-197">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff351-197">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="ff351-198">activities</span><span class="sxs-lookup"><span data-stu-id="ff351-198">activities</span></span>        | <span data-ttu-id="ff351-199">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="ff351-199">[itemActivity][] collection</span></span>    | <span data-ttu-id="ff351-200">A lista de atividades recentes que ocorreram neste item.</span><span class="sxs-lookup"><span data-stu-id="ff351-200">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="ff351-201">análise</span><span class="sxs-lookup"><span data-stu-id="ff351-201">analytics</span></span>         | <span data-ttu-id="ff351-202">recurso [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="ff351-202">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="ff351-203">Análise sobre as atividades de visualização que ocorreram neste item.</span><span class="sxs-lookup"><span data-stu-id="ff351-203">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="ff351-204">driveItem</span><span class="sxs-lookup"><span data-stu-id="ff351-204">driveItem</span></span>         | <span data-ttu-id="ff351-205">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="ff351-205">[driveItem][]</span></span>                  | <span data-ttu-id="ff351-206">Para bibliotecas de documentos, a relação **driveItem** expõe listItem como um **[driveItem][]**</span><span class="sxs-lookup"><span data-stu-id="ff351-206">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="ff351-207">campos</span><span class="sxs-lookup"><span data-stu-id="ff351-207">fields</span></span>            | <span data-ttu-id="ff351-208">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="ff351-208">[fieldValueSet][]</span></span>              | <span data-ttu-id="ff351-209">Os valores das colunas definidos neste item de lista.</span><span class="sxs-lookup"><span data-stu-id="ff351-209">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="ff351-210">versões</span><span class="sxs-lookup"><span data-stu-id="ff351-210">versions</span></span>          | <span data-ttu-id="ff351-211">coleção [listItemVersion][] </span><span class="sxs-lookup"><span data-stu-id="ff351-211">[listItemVersion][] collection</span></span> | <span data-ttu-id="ff351-212">A lista de versões anteriores do item de lista.</span><span class="sxs-lookup"><span data-stu-id="ff351-212">The list of previous versions of the list item.</span></span>

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
    "ListItem&quot;: &quot;#"
  },
  "suppressions": []
}
-->


