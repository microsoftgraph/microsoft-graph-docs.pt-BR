---
author: daspek
ms.author: dspektor
title: Obter o naanalytics
description: Obtenha o naanalytics sobre os modos de exibição que foram colocados sob esse recurso.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e416c9dbb40984466d279af60c7b6ea20fa68801
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272090"
---
# <a name="get-itemanalytics"></a><span data-ttu-id="ee788-103">Obter o naanalytics</span><span class="sxs-lookup"><span data-stu-id="ee788-103">Get itemAnalytics</span></span>

<span data-ttu-id="ee788-104">Obtenha [][] o naanalytics sobre os modos de exibição que foram colocados sob esse recurso.</span><span class="sxs-lookup"><span data-stu-id="ee788-104">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="ee788-105">O recurso do Microsoft **Analytics** é uma maneira conveniente de obter estatísticas de `allTime` atividades para `lastSevenDays`o e o.</span><span class="sxs-lookup"><span data-stu-id="ee788-105">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="ee788-106">Para um intervalo ou intervalo de tempo personalizado, use a API [funçãogetactivitiesbyinterval][] .</span><span class="sxs-lookup"><span data-stu-id="ee788-106">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="ee788-107">**Observação:** O \*\*\*\* recurso do naanalytics ainda não está disponível em todas as implantações [nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="ee788-107">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[Funçãogetactivitiesbyinterval]: ../api/itemactivitystat-getactivitybyinterval.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="permissions"></a><span data-ttu-id="ee788-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="ee788-110">Permissions</span></span>

<span data-ttu-id="ee788-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee788-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee788-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee788-113">Permission type</span></span>                        | <span data-ttu-id="ee788-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ee788-114">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="ee788-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee788-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="ee788-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee788-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="ee788-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee788-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee788-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee788-118">Not supported.</span></span>
|<span data-ttu-id="ee788-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee788-119">Application</span></span>                            | <span data-ttu-id="ee788-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee788-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="ee788-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee788-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ee788-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ee788-122">Optional query parameters</span></span>
<span data-ttu-id="ee788-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ee788-123">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee788-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee788-124">Request headers</span></span>

| <span data-ttu-id="ee788-125">Nome</span><span class="sxs-lookup"><span data-stu-id="ee788-125">Name</span></span>      |<span data-ttu-id="ee788-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee788-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ee788-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee788-127">Authorization</span></span>  | <span data-ttu-id="ee788-128">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="ee788-128">Bearer {code}.</span></span> <span data-ttu-id="ee788-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee788-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee788-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee788-130">Request body</span></span>

<span data-ttu-id="ee788-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ee788-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee788-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee788-132">Response</span></span> 

<span data-ttu-id="ee788-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objeto do objectanalytics no corpo da resposta. [][]</span><span class="sxs-lookup"><span data-stu-id="ee788-133">If successful, this method returns a `200 OK` response code and a collection of [itemAnalytics][] object in the response body.</span></span> 

## <a name="example"></a><span data-ttu-id="ee788-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee788-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee788-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee788-135">Request</span></span>

<!-- { "blockType": "request", "name": "get-analytics" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
```

### <a name="response"></a><span data-ttu-id="ee788-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee788-136">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.itemAnalytics", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "allTime": {
        "access": {
            "actionCount": 123,
            "actorCount": 89
        }
    },
    "lastSevenDays": {
        "access": {
            "actionCount": 52,
            "actorCount": 41
        }
    }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ee788-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="ee788-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ee788-138">C#</span><span class="sxs-lookup"><span data-stu-id="ee788-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-analytics-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ee788-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="ee788-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-analytics-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ee788-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ee788-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-analytics-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get analytics",
  "suppressions": [
    "Error: /api-reference/v1.0/api/itemanalytics-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/itemanalytics-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/itemanalytics-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
  ]
}
-->
