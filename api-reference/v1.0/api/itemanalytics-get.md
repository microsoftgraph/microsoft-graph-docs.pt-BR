---
author: daspek
ms.author: dspektor
title: Obter o naanalytics
description: Obtenha o naanalytics sobre os modos de exibição que foram colocados sob esse recurso.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: dd8ba2295a84c5ff4612b64c4a1b4485c5a95dbb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023241"
---
# <a name="get-itemanalytics"></a><span data-ttu-id="497f5-103">Obter o naanalytics</span><span class="sxs-lookup"><span data-stu-id="497f5-103">Get itemAnalytics</span></span>

<span data-ttu-id="497f5-104">Obtenha [][] o naanalytics sobre os modos de exibição que foram colocados sob esse recurso.</span><span class="sxs-lookup"><span data-stu-id="497f5-104">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="497f5-105">O recurso do Microsoft **Analytics** é uma maneira conveniente de obter estatísticas de `allTime` atividades para `lastSevenDays`o e o.</span><span class="sxs-lookup"><span data-stu-id="497f5-105">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="497f5-106">Para um intervalo ou intervalo de tempo personalizado, use a API [funçãogetactivitiesbyinterval][] .</span><span class="sxs-lookup"><span data-stu-id="497f5-106">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="497f5-107">**Observação:** O \*\*\*\* recurso do naanalytics ainda não está disponível em todas as implantações [nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="497f5-107">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[Funçãogetactivitiesbyinterval]: ../api/itemactivitystat-getactivitybyinterval.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="permissions"></a><span data-ttu-id="497f5-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="497f5-110">Permissions</span></span>

<span data-ttu-id="497f5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="497f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="497f5-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="497f5-113">Permission type</span></span>                        | <span data-ttu-id="497f5-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="497f5-114">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="497f5-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="497f5-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="497f5-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="497f5-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="497f5-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="497f5-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="497f5-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="497f5-118">Not supported.</span></span>
|<span data-ttu-id="497f5-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="497f5-119">Application</span></span>                            | <span data-ttu-id="497f5-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="497f5-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="497f5-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="497f5-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```
## <a name="optional-query-parameters"></a><span data-ttu-id="497f5-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="497f5-122">Optional query parameters</span></span>
<span data-ttu-id="497f5-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="497f5-123">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="497f5-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="497f5-124">Request headers</span></span>

| <span data-ttu-id="497f5-125">Nome</span><span class="sxs-lookup"><span data-stu-id="497f5-125">Name</span></span>      |<span data-ttu-id="497f5-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="497f5-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="497f5-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="497f5-127">Authorization</span></span>  | <span data-ttu-id="497f5-128">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="497f5-128">Bearer {code}.</span></span> <span data-ttu-id="497f5-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="497f5-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="497f5-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="497f5-130">Request body</span></span>

<span data-ttu-id="497f5-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="497f5-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="497f5-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="497f5-132">Response</span></span> 

<span data-ttu-id="497f5-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objeto do objectanalytics no corpo da resposta. [][]</span><span class="sxs-lookup"><span data-stu-id="497f5-133">If successful, this method returns a `200 OK` response code and a collection of [itemAnalytics][] object in the response body.</span></span> 

## <a name="example"></a><span data-ttu-id="497f5-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="497f5-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="497f5-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="497f5-135">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="497f5-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="497f5-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-analytics" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="497f5-137">C#</span><span class="sxs-lookup"><span data-stu-id="497f5-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-analytics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="497f5-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="497f5-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-analytics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="497f5-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="497f5-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-analytics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="497f5-140">Java</span><span class="sxs-lookup"><span data-stu-id="497f5-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-analytics-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="497f5-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="497f5-141">Response</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "BaseItem/Get analytics",
  "suppressions": [
  ]
}
-->
