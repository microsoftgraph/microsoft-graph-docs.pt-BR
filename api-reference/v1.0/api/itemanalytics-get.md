---
author: daspek
ms.author: dspektor
title: Obter o naanalytics
description: Obtenha o naanalytics sobre os modos de exibição que foram colocados sob esse recurso.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 311d7eea81ba3001af6cb94e2a3f837824a67fde
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038470"
---
# <a name="get-itemanalytics"></a><span data-ttu-id="d9d98-103">Obter o naanalytics</span><span class="sxs-lookup"><span data-stu-id="d9d98-103">Get itemAnalytics</span></span>

<span data-ttu-id="d9d98-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9d98-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d9d98-105">Obtenha o [naanalytics][] sobre os modos de exibição que foram colocados sob esse recurso.</span><span class="sxs-lookup"><span data-stu-id="d9d98-105">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="d9d98-106">O recurso do Microsoft **Analytics** é uma maneira conveniente de obter estatísticas de atividades para `allTime` o e o `lastSevenDays` .</span><span class="sxs-lookup"><span data-stu-id="d9d98-106">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="d9d98-107">Para um intervalo ou intervalo de tempo personalizado, use a API [funçãogetactivitiesbyinterval][] .</span><span class="sxs-lookup"><span data-stu-id="d9d98-107">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="d9d98-108">**Observação:** O recurso do **naanalytics** ainda não está disponível em todas as [implantações nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="d9d98-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[Funçãogetactivitiesbyinterval]: ../api/itemactivitystat-getactivitybyinterval.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="permissions"></a><span data-ttu-id="d9d98-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="d9d98-111">Permissions</span></span>

<span data-ttu-id="d9d98-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9d98-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9d98-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9d98-114">Permission type</span></span>                        | <span data-ttu-id="d9d98-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d9d98-115">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="d9d98-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9d98-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="d9d98-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9d98-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="d9d98-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9d98-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9d98-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9d98-119">Not supported.</span></span>
|<span data-ttu-id="d9d98-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9d98-120">Application</span></span>                            | <span data-ttu-id="d9d98-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9d98-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="d9d98-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9d98-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d9d98-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d9d98-123">Optional query parameters</span></span>
<span data-ttu-id="d9d98-124">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d9d98-124">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d9d98-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9d98-125">Request headers</span></span>

| <span data-ttu-id="d9d98-126">Nome</span><span class="sxs-lookup"><span data-stu-id="d9d98-126">Name</span></span>      |<span data-ttu-id="d9d98-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9d98-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d9d98-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9d98-128">Authorization</span></span>  | <span data-ttu-id="d9d98-129">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="d9d98-129">Bearer {code}.</span></span> <span data-ttu-id="d9d98-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9d98-130">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9d98-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9d98-131">Request body</span></span>

<span data-ttu-id="d9d98-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d9d98-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9d98-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9d98-133">Response</span></span> 

<span data-ttu-id="d9d98-134">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objeto do [objectanalytics][] no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9d98-134">If successful, this method returns a `200 OK` response code and a collection of [itemAnalytics][] object in the response body.</span></span> 

## <a name="example"></a><span data-ttu-id="d9d98-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9d98-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9d98-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9d98-136">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d9d98-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9d98-137">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-analytics" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/analytics
```
# <a name="c"></a>[<span data-ttu-id="d9d98-138">C#</span><span class="sxs-lookup"><span data-stu-id="d9d98-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-analytics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9d98-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9d98-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-analytics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9d98-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9d98-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-analytics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d9d98-141">Java</span><span class="sxs-lookup"><span data-stu-id="d9d98-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-analytics-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d9d98-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9d98-142">Response</span></span>

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

