---
author: daspek
ms.author: dspektor
title: Obter o naanalytics
description: Obtenha o naanalytics sobre os modos de exibição que foram colocados sob esse recurso.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b6f1da3d02b1a11afc70ca3be51177fb4e193047
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511751"
---
# <a name="get-itemanalytics"></a><span data-ttu-id="b5a6e-103">Obter o naanalytics</span><span class="sxs-lookup"><span data-stu-id="b5a6e-103">Get itemAnalytics</span></span>

<span data-ttu-id="b5a6e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5a6e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b5a6e-105">Obtenha o [naanalytics][] sobre os modos de exibição que foram colocados sob esse recurso.</span><span class="sxs-lookup"><span data-stu-id="b5a6e-105">Get [itemAnalytics][] about the views that took place under this resource.</span></span>
<span data-ttu-id="b5a6e-106">O recurso do Microsoft **Analytics** é uma maneira conveniente de obter estatísticas de `allTime` atividades para `lastSevenDays`o e o.</span><span class="sxs-lookup"><span data-stu-id="b5a6e-106">The **itemAnalytics** resource is a convenient way to get activity stats for `allTime` and the `lastSevenDays`.</span></span>
<span data-ttu-id="b5a6e-107">Para um intervalo ou intervalo de tempo personalizado, use a API [funçãogetactivitiesbyinterval][] .</span><span class="sxs-lookup"><span data-stu-id="b5a6e-107">For a custom time range or interval, use the [getActivitiesByInterval][] API.</span></span>

><span data-ttu-id="b5a6e-108">**Observação:** O recurso do **naanalytics** ainda não está disponível em todas as [implantações nacionais](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="b5a6e-108">**Note:** The **itemAnalytics** resource is not yet available in all [national deployments](/graph/deployments).</span></span>

[itemAnalytics]: ../resources/itemanalytics.md
[Funçãogetactivitiesbyinterval]: ../api/itemactivitystat-getactivitybyinterval.md
[getActivitiesByInterval]: ../api/itemactivitystat-getactivitybyinterval.md

## <a name="permissions"></a><span data-ttu-id="b5a6e-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="b5a6e-111">Permissions</span></span>

<span data-ttu-id="b5a6e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5a6e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5a6e-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5a6e-114">Permission type</span></span>                        | <span data-ttu-id="b5a6e-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b5a6e-115">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="b5a6e-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5a6e-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="b5a6e-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5a6e-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="b5a6e-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5a6e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5a6e-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5a6e-119">Not supported.</span></span>
|<span data-ttu-id="b5a6e-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5a6e-120">Application</span></span>                            | <span data-ttu-id="b5a6e-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5a6e-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="b5a6e-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5a6e-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/analytics
GET /sites/{site-id}/analytics
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/analytics
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b5a6e-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b5a6e-123">Optional query parameters</span></span>
<span data-ttu-id="b5a6e-124">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b5a6e-124">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5a6e-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5a6e-125">Request headers</span></span>

| <span data-ttu-id="b5a6e-126">Nome</span><span class="sxs-lookup"><span data-stu-id="b5a6e-126">Name</span></span>      |<span data-ttu-id="b5a6e-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5a6e-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b5a6e-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5a6e-128">Authorization</span></span>  | <span data-ttu-id="b5a6e-129">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="b5a6e-129">Bearer {code}.</span></span> <span data-ttu-id="b5a6e-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5a6e-130">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5a6e-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5a6e-131">Request body</span></span>

<span data-ttu-id="b5a6e-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b5a6e-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5a6e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5a6e-133">Response</span></span> 

<span data-ttu-id="b5a6e-134">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objeto do [objectanalytics][] no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5a6e-134">If successful, this method returns a `200 OK` response code and a collection of [itemAnalytics][] object in the response body.</span></span> 

## <a name="example"></a><span data-ttu-id="b5a6e-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5a6e-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5a6e-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5a6e-136">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b5a6e-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5a6e-137">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-analytics" } -->

```msgraph-interactive
GET /drives/{drive-id}/items/{item-id}/analytics
```
# <a name="c"></a>[<span data-ttu-id="b5a6e-138">C#</span><span class="sxs-lookup"><span data-stu-id="b5a6e-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-analytics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5a6e-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5a6e-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-analytics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5a6e-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5a6e-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-analytics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b5a6e-141">Java</span><span class="sxs-lookup"><span data-stu-id="b5a6e-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-analytics-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b5a6e-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5a6e-142">Response</span></span>

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
