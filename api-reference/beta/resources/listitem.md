---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ListItem
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 435544db272b26e6fe3ac0e09803858eec9d05f6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581616"
---
# <a name="listitem-resource"></a><span data-ttu-id="2df70-102">Recurso ListItem</span><span class="sxs-lookup"><span data-stu-id="2df70-102">ListItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2df70-103">Este recurso representa um item em uma **[list][]** do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2df70-103">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="2df70-104">Os valores de coluna na lista estão disponíveis por meio do dicionário `fieldValueSet`.</span><span class="sxs-lookup"><span data-stu-id="2df70-104">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="2df70-105">Tarefas em um listItem</span><span class="sxs-lookup"><span data-stu-id="2df70-105">Tasks on a listItem</span></span>

<span data-ttu-id="2df70-106">As tarefas a seguir estão disponíveis para recursos **listItem**.</span><span class="sxs-lookup"><span data-stu-id="2df70-106">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="2df70-107">Todos os exemplos a seguir referem-se a uma **[list][]**, por exemplo: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="2df70-107">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="2df70-108">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="2df70-108">Common task</span></span>                    | <span data-ttu-id="2df70-109">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="2df70-109">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="2df70-110">[Get][]</span><span class="sxs-lookup"><span data-stu-id="2df70-110">[Get][]</span></span>                        | <span data-ttu-id="2df70-111">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="2df70-111">GET /items/{item-id}</span></span>
| <span data-ttu-id="2df70-112">[Obter valores de coluna][Get]</span><span class="sxs-lookup"><span data-stu-id="2df70-112">[Get column values][Get]</span></span>       | <span data-ttu-id="2df70-113">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="2df70-113">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="2df70-114">[Obter análises][]</span><span class="sxs-lookup"><span data-stu-id="2df70-114">[Get analytics][]</span></span>              | <span data-ttu-id="2df70-115">OBTER/Items/{Item-ID}/Analytics</span><span class="sxs-lookup"><span data-stu-id="2df70-115">GET /items/{item-id}/analytics</span></span>
| <span data-ttu-id="2df70-116">[Obter atividades por intervalo][]</span><span class="sxs-lookup"><span data-stu-id="2df70-116">[Get activities by interval][]</span></span> | <span data-ttu-id="2df70-117">OBTER/items/{item-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="2df70-117">GET /items/{item-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="2df70-118">[Create][]</span><span class="sxs-lookup"><span data-stu-id="2df70-118">[Create][]</span></span>                     | <span data-ttu-id="2df70-119">POST /items</span><span class="sxs-lookup"><span data-stu-id="2df70-119">POST /items</span></span>
| <span data-ttu-id="2df70-120">[Delete][]</span><span class="sxs-lookup"><span data-stu-id="2df70-120">[Delete][]</span></span>                     | <span data-ttu-id="2df70-121">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="2df70-121">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="2df70-122">[Update][]</span><span class="sxs-lookup"><span data-stu-id="2df70-122">[Update][]</span></span>                     | <span data-ttu-id="2df70-123">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="2df70-123">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="2df70-124">[Atualizar valores de coluna][Update]</span><span class="sxs-lookup"><span data-stu-id="2df70-124">[Update column values][Update]</span></span> | <span data-ttu-id="2df70-125">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="2df70-125">PATCH /items/{item-id}/fields</span></span>

[Get]: ../api/listitem-get.md
[Obter análises]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[Obter atividades por intervalo]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md
[Create]: ../api/listitem-create.md
[Excluir]: ../api/listitem-delete.md
[Delete]: ../api/listitem-delete.md
[Update]: ../api/listitem-update.md

## <a name="json-representation"></a><span data-ttu-id="2df70-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2df70-132">JSON representation</span></span>

<span data-ttu-id="2df70-133">Veja a seguir uma representação JSON de um recurso **listItem**.</span><span class="sxs-lookup"><span data-stu-id="2df70-133">Here is a JSON representation of a **listItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="2df70-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2df70-134">Properties</span></span>

<span data-ttu-id="2df70-135">O recurso **listItem** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="2df70-135">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="2df70-136">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="2df70-136">Property name</span></span> | <span data-ttu-id="2df70-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="2df70-137">Type</span></span>                | <span data-ttu-id="2df70-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="2df70-138">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="2df70-139">contentType</span><span class="sxs-lookup"><span data-stu-id="2df70-139">contentType</span></span>   | <span data-ttu-id="2df70-140">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="2df70-140">[contentTypeInfo][]</span></span> | <span data-ttu-id="2df70-141">O tipo de conteúdo deste item de lista</span><span class="sxs-lookup"><span data-stu-id="2df70-141">The content type of this list item</span></span>

<span data-ttu-id="2df70-142">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="2df70-142">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="2df70-143">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="2df70-143">Property name</span></span>        | <span data-ttu-id="2df70-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="2df70-144">Type</span></span>              | <span data-ttu-id="2df70-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="2df70-145">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="2df70-146">id</span><span class="sxs-lookup"><span data-stu-id="2df70-146">id</span></span>                   | <span data-ttu-id="2df70-147">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2df70-147">string</span></span>            | <span data-ttu-id="2df70-p103">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2df70-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="2df70-150">name</span><span class="sxs-lookup"><span data-stu-id="2df70-150">name</span></span>                 | <span data-ttu-id="2df70-151">string</span><span class="sxs-lookup"><span data-stu-id="2df70-151">string</span></span>            | <span data-ttu-id="2df70-152">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="2df70-152">The name / title of the item.</span></span>
| <span data-ttu-id="2df70-153">createdBy</span><span class="sxs-lookup"><span data-stu-id="2df70-153">createdBy</span></span>            | <span data-ttu-id="2df70-154">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="2df70-154">[identitySet][]</span></span>   | <span data-ttu-id="2df70-155">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="2df70-155">Identity of the creator of this item.</span></span> <span data-ttu-id="2df70-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2df70-156">Read-only.</span></span>
| <span data-ttu-id="2df70-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2df70-157">createdDateTime</span></span>      | <span data-ttu-id="2df70-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2df70-158">DateTimeOffset</span></span>    | <span data-ttu-id="2df70-p105">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2df70-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="2df70-161">description</span><span class="sxs-lookup"><span data-stu-id="2df70-161">description</span></span>          | <span data-ttu-id="2df70-162">string</span><span class="sxs-lookup"><span data-stu-id="2df70-162">string</span></span>            | <span data-ttu-id="2df70-163">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="2df70-163">The descriptive text for the item.</span></span>
| <span data-ttu-id="2df70-164">eTag</span><span class="sxs-lookup"><span data-stu-id="2df70-164">eTag</span></span>                 | <span data-ttu-id="2df70-165">string</span><span class="sxs-lookup"><span data-stu-id="2df70-165">string</span></span>            | <span data-ttu-id="2df70-p106">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2df70-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="2df70-168">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="2df70-168">lastModifiedBy</span></span>       | <span data-ttu-id="2df70-169">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="2df70-169">[identitySet][]</span></span>   | <span data-ttu-id="2df70-170">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="2df70-170">Identity of the last modifier of this item.</span></span> <span data-ttu-id="2df70-171">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2df70-171">Read-only.</span></span>
| <span data-ttu-id="2df70-172">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2df70-172">lastModifiedDateTime</span></span> | <span data-ttu-id="2df70-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2df70-173">DateTimeOffset</span></span>    | <span data-ttu-id="2df70-p108">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2df70-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="2df70-176">parentReference</span><span class="sxs-lookup"><span data-stu-id="2df70-176">parentReference</span></span>      | <span data-ttu-id="2df70-177">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="2df70-177">[itemReference][]</span></span> | <span data-ttu-id="2df70-p109">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="2df70-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="2df70-180">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="2df70-180">sharepointIds</span></span>        | <span data-ttu-id="2df70-181">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="2df70-181">[sharepointIds][]</span></span> | <span data-ttu-id="2df70-p110">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2df70-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="2df70-184">webUrl</span><span class="sxs-lookup"><span data-stu-id="2df70-184">webUrl</span></span>               | <span data-ttu-id="2df70-185">string (url)</span><span class="sxs-lookup"><span data-stu-id="2df70-185">string (url)</span></span>      | <span data-ttu-id="2df70-p111">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2df70-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="2df70-188">Relações</span><span class="sxs-lookup"><span data-stu-id="2df70-188">Relationships</span></span>

 <span data-ttu-id="2df70-189">O recurso **listItem** tem as seguintes relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="2df70-189">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="2df70-190">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="2df70-190">Relationship name</span></span> | <span data-ttu-id="2df70-191">Tipo</span><span class="sxs-lookup"><span data-stu-id="2df70-191">Type</span></span>                           | <span data-ttu-id="2df70-192">Descrição</span><span class="sxs-lookup"><span data-stu-id="2df70-192">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="2df70-193">activities</span><span class="sxs-lookup"><span data-stu-id="2df70-193">activities</span></span>        | <span data-ttu-id="2df70-194">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="2df70-194">[itemActivity][] collection</span></span>    | <span data-ttu-id="2df70-195">A lista de atividades recentes que ocorreram neste item.</span><span class="sxs-lookup"><span data-stu-id="2df70-195">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="2df70-196">analytics</span><span class="sxs-lookup"><span data-stu-id="2df70-196">analytics</span></span>         | <span data-ttu-id="2df70-197">[itemAnalytics][] resource</span><span class="sxs-lookup"><span data-stu-id="2df70-197">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="2df70-198">Análise sobre as atividades de exibição que ocorreram neste item.</span><span class="sxs-lookup"><span data-stu-id="2df70-198">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="2df70-199">driveItem</span><span class="sxs-lookup"><span data-stu-id="2df70-199">driveItem</span></span>         | <span data-ttu-id="2df70-200">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="2df70-200">[driveItem][]</span></span>                  | <span data-ttu-id="2df70-201">Para bibliotecas de documentos, a relação **driveItem** expõe listItem como um **[driveItem][]**</span><span class="sxs-lookup"><span data-stu-id="2df70-201">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="2df70-202">campos</span><span class="sxs-lookup"><span data-stu-id="2df70-202">fields</span></span>            | <span data-ttu-id="2df70-203">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="2df70-203">[fieldValueSet][]</span></span>              | <span data-ttu-id="2df70-204">Os valores das colunas definidos neste item de lista.</span><span class="sxs-lookup"><span data-stu-id="2df70-204">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="2df70-205">versões</span><span class="sxs-lookup"><span data-stu-id="2df70-205">versions</span></span>          | <span data-ttu-id="2df70-206">coleção [listItemVersion][] </span><span class="sxs-lookup"><span data-stu-id="2df70-206">[listItemVersion][] collection</span></span> | <span data-ttu-id="2df70-207">A lista de versões anteriores do item de lista.</span><span class="sxs-lookup"><span data-stu-id="2df70-207">The list of previous versions of the list item.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/listitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
