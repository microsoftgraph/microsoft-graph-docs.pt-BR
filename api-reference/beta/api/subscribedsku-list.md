---
title: Listar subscribedSkus
description: Recupere a lista de assinaturas comerciais que uma organização adquiriu.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0ca68f2a2bc7dd96d22b8bacc5c65b8983b85bb1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453125"
---
# <a name="list-subscribedskus"></a><span data-ttu-id="a23f6-103">Listar subscribedSkus</span><span class="sxs-lookup"><span data-stu-id="a23f6-103">List subscribedSkus</span></span>

<span data-ttu-id="a23f6-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a23f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a23f6-105">Obtenha a lista de assinaturas comerciais que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="a23f6-105">Get the list of commercial subscriptions that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="a23f6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a23f6-106">Permissions</span></span>
<span data-ttu-id="a23f6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a23f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a23f6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a23f6-109">Permission type</span></span>      | <span data-ttu-id="a23f6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a23f6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a23f6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a23f6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a23f6-112">Organization. Read. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="a23f6-112">Organization.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a23f6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a23f6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a23f6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a23f6-114">Not supported.</span></span>    |
|<span data-ttu-id="a23f6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a23f6-115">Application</span></span> | <span data-ttu-id="a23f6-116">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a23f6-116">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a23f6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a23f6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a23f6-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a23f6-118">Optional query parameters</span></span>

<span data-ttu-id="a23f6-119">Este método não oferece suporte aos [parâmetros de consulta OData](/graph//query-parameters) para ajudar a personalizar a`$filter` resposta (não tem suporte).</span><span class="sxs-lookup"><span data-stu-id="a23f6-119">This method does not support the [OData query parameters](/graph//query-parameters) to help customize the response (`$filter` is not supported).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a23f6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a23f6-120">Request headers</span></span>

| <span data-ttu-id="a23f6-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a23f6-121">Name</span></span>       | <span data-ttu-id="a23f6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a23f6-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="a23f6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a23f6-123">Authorization</span></span>  | <span data-ttu-id="a23f6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a23f6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a23f6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a23f6-126">Request body</span></span>
<span data-ttu-id="a23f6-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a23f6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a23f6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a23f6-128">Response</span></span>

<span data-ttu-id="a23f6-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [subscribedSku](../resources/subscribedsku.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a23f6-129">If successful, this method returns a `200 OK` response code and collection of [subscribedSku](../resources/subscribedsku.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a23f6-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a23f6-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a23f6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a23f6-131">Request</span></span>
<span data-ttu-id="a23f6-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a23f6-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a23f6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a23f6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscribedskus"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/subscribedSkus
```
# <a name="c"></a>[<span data-ttu-id="a23f6-134">C#</span><span class="sxs-lookup"><span data-stu-id="a23f6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscribedskus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a23f6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a23f6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscribedskus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a23f6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a23f6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscribedskus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a23f6-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a23f6-137">Response</span></span>
<span data-ttu-id="a23f6-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a23f6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribedSku",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 547

{
  "value": [
    {
      "capabilityStatus": "capabilityStatus-value",
      "consumedUnits": 99,
      "prepaidUnits": {
        "enabled": 99,
        "suspended": 99,
        "warning": 99
      },
      "servicePlans": [
        {
          "servicePlanId": "servicePlanId-value",
          "servicePlanName": "servicePlanName-value",
          "provisioningStatus": "provisioningStatus-value",
          "appliesTo": "appliesTo-value"
        }
      ],
      "skuId": "skuId-value",
      "skuPartNumber": "skuPartNumber-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List subscribedSkus",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
