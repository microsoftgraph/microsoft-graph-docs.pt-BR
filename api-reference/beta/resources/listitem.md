---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListItem
ms.openlocfilehash: 18ba74fd677c83da5f8bfe5d13303f7b18ed43f2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034847"
---
# <a name="listitem-resource"></a><span data-ttu-id="6365f-102">Recurso ListItem</span><span class="sxs-lookup"><span data-stu-id="6365f-102">ListItem resource</span></span>

> <span data-ttu-id="6365f-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6365f-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6365f-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6365f-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6365f-105">Este recurso representa um item em uma **[list][]** do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6365f-105">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="6365f-106">Os valores de coluna na lista estão disponíveis por meio do dicionário `fieldValueSet`.</span><span class="sxs-lookup"><span data-stu-id="6365f-106">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="6365f-107">Tarefas em um listItem</span><span class="sxs-lookup"><span data-stu-id="6365f-107">Tasks on a listItem</span></span>

<span data-ttu-id="6365f-108">As tarefas a seguir estão disponíveis para recursos **listItem**.</span><span class="sxs-lookup"><span data-stu-id="6365f-108">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="6365f-109">Todos os exemplos a seguir referem-se a uma **[list][]**, por exemplo: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="6365f-109">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="6365f-110">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="6365f-110">Common task</span></span>                    | <span data-ttu-id="6365f-111">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="6365f-111">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="6365f-112">[Get][]</span><span class="sxs-lookup"><span data-stu-id="6365f-112">[Get][]</span></span>                        | <span data-ttu-id="6365f-113">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="6365f-113">GET /items/{item-id}</span></span>
| <span data-ttu-id="6365f-114">[Obter valores de coluna][Get]</span><span class="sxs-lookup"><span data-stu-id="6365f-114">[Get column values][Get]</span></span>       | <span data-ttu-id="6365f-115">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="6365f-115">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="6365f-116">[Obtenha a análise][]</span><span class="sxs-lookup"><span data-stu-id="6365f-116">[Get analytics][]</span></span>              | <span data-ttu-id="6365f-117">GET /items/ {id de item} / análise</span><span class="sxs-lookup"><span data-stu-id="6365f-117">GET /items/{item-id}/analytics</span></span>
| <span data-ttu-id="6365f-118">[Fazer atividades pelo intervalo][]</span><span class="sxs-lookup"><span data-stu-id="6365f-118">[Get activities by interval][]</span></span> | <span data-ttu-id="6365f-119">GET /items/ {id de item} / getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="6365f-119">GET /items/{item-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="6365f-120">[Create][]</span><span class="sxs-lookup"><span data-stu-id="6365f-120">[Create][]</span></span>                     | <span data-ttu-id="6365f-121">POST /items</span><span class="sxs-lookup"><span data-stu-id="6365f-121">POST /items</span></span>
| <span data-ttu-id="6365f-122">[Delete][]</span><span class="sxs-lookup"><span data-stu-id="6365f-122">[Delete][]</span></span>                     | <span data-ttu-id="6365f-123">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="6365f-123">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="6365f-124">[Update][]</span><span class="sxs-lookup"><span data-stu-id="6365f-124">[Update][]</span></span>                     | <span data-ttu-id="6365f-125">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="6365f-125">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="6365f-126">[Atualizar valores de coluna][Update]</span><span class="sxs-lookup"><span data-stu-id="6365f-126">[Update column values][Update]</span></span> | <span data-ttu-id="6365f-127">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="6365f-127">PATCH /items/{item-id}/fields</span></span>

[Get]: ../api/listitem-get.md
[Obtenha a análise]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[Fazer atividades pelo intervalo]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md
[Create]: ../api/listitem-create.md
[Delete]: ../api/listitem-delete.md
[Update]: ../api/listitem-update.md

## <a name="json-representation"></a><span data-ttu-id="6365f-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6365f-134">JSON representation</span></span>

<span data-ttu-id="6365f-135">Veja a seguir uma representação JSON de um recurso **listItem**.</span><span class="sxs-lookup"><span data-stu-id="6365f-135">Here is a JSON representation of a **listItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="6365f-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6365f-136">Properties</span></span>

<span data-ttu-id="6365f-137">O recurso **listItem** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="6365f-137">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="6365f-138">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="6365f-138">Property name</span></span> | <span data-ttu-id="6365f-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="6365f-139">Type</span></span>                | <span data-ttu-id="6365f-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="6365f-140">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="6365f-141">contentType</span><span class="sxs-lookup"><span data-stu-id="6365f-141">contentType</span></span>   | <span data-ttu-id="6365f-142">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="6365f-142">[contentTypeInfo][]</span></span> | <span data-ttu-id="6365f-143">O tipo de conteúdo deste item de lista</span><span class="sxs-lookup"><span data-stu-id="6365f-143">The content type of this list item</span></span>

<span data-ttu-id="6365f-144">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="6365f-144">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="6365f-145">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="6365f-145">Property name</span></span>        | <span data-ttu-id="6365f-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="6365f-146">Type</span></span>              | <span data-ttu-id="6365f-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="6365f-147">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="6365f-148">id</span><span class="sxs-lookup"><span data-stu-id="6365f-148">id</span></span>                   | <span data-ttu-id="6365f-149">string</span><span class="sxs-lookup"><span data-stu-id="6365f-149">string</span></span>            | <span data-ttu-id="6365f-p104">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6365f-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="6365f-152">name</span><span class="sxs-lookup"><span data-stu-id="6365f-152">name</span></span>                 | <span data-ttu-id="6365f-153">string</span><span class="sxs-lookup"><span data-stu-id="6365f-153">string</span></span>            | <span data-ttu-id="6365f-154">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="6365f-154">The name / title of the item.</span></span>
| <span data-ttu-id="6365f-155">createdBy</span><span class="sxs-lookup"><span data-stu-id="6365f-155">createdBy</span></span>            | <span data-ttu-id="6365f-156">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="6365f-156">[identitySet][]</span></span>   | <span data-ttu-id="6365f-157">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="6365f-157">Identity of the creator of this item.</span></span> <span data-ttu-id="6365f-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6365f-158">Read-only.</span></span>
| <span data-ttu-id="6365f-159">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6365f-159">createdDateTime</span></span>      | <span data-ttu-id="6365f-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6365f-160">DateTimeOffset</span></span>    | <span data-ttu-id="6365f-p106">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6365f-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="6365f-163">description</span><span class="sxs-lookup"><span data-stu-id="6365f-163">description</span></span>          | <span data-ttu-id="6365f-164">string</span><span class="sxs-lookup"><span data-stu-id="6365f-164">string</span></span>            | <span data-ttu-id="6365f-165">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="6365f-165">The descriptive text for the item.</span></span>
| <span data-ttu-id="6365f-166">eTag</span><span class="sxs-lookup"><span data-stu-id="6365f-166">eTag</span></span>                 | <span data-ttu-id="6365f-167">string</span><span class="sxs-lookup"><span data-stu-id="6365f-167">string</span></span>            | <span data-ttu-id="6365f-p107">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6365f-p107">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="6365f-170">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="6365f-170">lastModifiedBy</span></span>       | <span data-ttu-id="6365f-171">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="6365f-171">[identitySet][]</span></span>   | <span data-ttu-id="6365f-172">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="6365f-172">Identity of the last modifier of this item.</span></span> <span data-ttu-id="6365f-173">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6365f-173">Read-only.</span></span>
| <span data-ttu-id="6365f-174">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6365f-174">lastModifiedDateTime</span></span> | <span data-ttu-id="6365f-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6365f-175">DateTimeOffset</span></span>    | <span data-ttu-id="6365f-p109">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6365f-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="6365f-178">parentReference</span><span class="sxs-lookup"><span data-stu-id="6365f-178">parentReference</span></span>      | <span data-ttu-id="6365f-179">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="6365f-179">[itemReference][]</span></span> | <span data-ttu-id="6365f-p110">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="6365f-p110">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="6365f-182">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="6365f-182">sharepointIds</span></span>        | <span data-ttu-id="6365f-183">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="6365f-183">[sharepointIds][]</span></span> | <span data-ttu-id="6365f-p111">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6365f-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="6365f-186">webUrl</span><span class="sxs-lookup"><span data-stu-id="6365f-186">webUrl</span></span>               | <span data-ttu-id="6365f-187">string (url)</span><span class="sxs-lookup"><span data-stu-id="6365f-187">string (url)</span></span>      | <span data-ttu-id="6365f-p112">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6365f-p112">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="6365f-190">Relações</span><span class="sxs-lookup"><span data-stu-id="6365f-190">Relationships</span></span>

 <span data-ttu-id="6365f-191">O recurso **listItem** tem as seguintes relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="6365f-191">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="6365f-192">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="6365f-192">Relationship name</span></span> | <span data-ttu-id="6365f-193">Tipo</span><span class="sxs-lookup"><span data-stu-id="6365f-193">Type</span></span>                           | <span data-ttu-id="6365f-194">Descrição</span><span class="sxs-lookup"><span data-stu-id="6365f-194">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="6365f-195">activities</span><span class="sxs-lookup"><span data-stu-id="6365f-195">activities</span></span>        | <span data-ttu-id="6365f-196">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="6365f-196">[itemActivity][] collection</span></span>    | <span data-ttu-id="6365f-197">A lista de atividades recentes que ocorreram neste item.</span><span class="sxs-lookup"><span data-stu-id="6365f-197">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="6365f-198">análise</span><span class="sxs-lookup"><span data-stu-id="6365f-198">analytics</span></span>         | <span data-ttu-id="6365f-199">recurso de [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="6365f-199">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="6365f-200">Análise sobre as atividades de modo de exibição que foram realizada neste item.</span><span class="sxs-lookup"><span data-stu-id="6365f-200">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="6365f-201">driveItem</span><span class="sxs-lookup"><span data-stu-id="6365f-201">driveItem</span></span>         | <span data-ttu-id="6365f-202">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="6365f-202">[driveItem][]</span></span>                  | <span data-ttu-id="6365f-203">Para bibliotecas de documentos, a relação **driveItem** expõe listItem como um **[driveItem][]**</span><span class="sxs-lookup"><span data-stu-id="6365f-203">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="6365f-204">campos</span><span class="sxs-lookup"><span data-stu-id="6365f-204">fields</span></span>            | <span data-ttu-id="6365f-205">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="6365f-205">[fieldValueSet][]</span></span>              | <span data-ttu-id="6365f-206">Os valores das colunas definidos neste item de lista.</span><span class="sxs-lookup"><span data-stu-id="6365f-206">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="6365f-207">versions</span><span class="sxs-lookup"><span data-stu-id="6365f-207">versions</span></span>          | <span data-ttu-id="6365f-208">coleção [listItemVersion][]</span><span class="sxs-lookup"><span data-stu-id="6365f-208">[listItemVersion][] collection</span></span> | <span data-ttu-id="6365f-209">Lista de versões anteriores do item da lista.</span><span class="sxs-lookup"><span data-stu-id="6365f-209">The list of previous versions of the list item.</span></span>

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[driveItem]: driveitem.md
[fieldValueSet]: fieldvalueset.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[lista]: list.md
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
