---
title: Listar subscribedSkus
description: Recupere a lista de assinaturas comerciais que uma organização adquiriu.
localization_priority: Normal
author: SumitParikh
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 416f91448a8bba9852f68bb5587818555ee4ca78
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048964"
---
# <a name="list-subscribedskus"></a><span data-ttu-id="0b0f2-103">Listar subscribedSkus</span><span class="sxs-lookup"><span data-stu-id="0b0f2-103">List subscribedSkus</span></span>

<span data-ttu-id="0b0f2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b0f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b0f2-105">Obtenha a lista de assinaturas comerciais que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="0b0f2-105">Get the list of commercial subscriptions that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b0f2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0b0f2-106">Permissions</span></span>
<span data-ttu-id="0b0f2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b0f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0b0f2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b0f2-109">Permission type</span></span>      | <span data-ttu-id="0b0f2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0b0f2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b0f2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b0f2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0b0f2-112">Organization.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0b0f2-112">Organization.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0b0f2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b0f2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b0f2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b0f2-114">Not supported.</span></span>    |
|<span data-ttu-id="0b0f2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b0f2-115">Application</span></span> | <span data-ttu-id="0b0f2-116">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b0f2-116">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b0f2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b0f2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0b0f2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0b0f2-118">Optional query parameters</span></span>

<span data-ttu-id="0b0f2-119">Esse método não dá suporte aos [parâmetros de consulta OData](/graph//query-parameters) para ajudar a personalizar a resposta ( `$filter` não há suporte).</span><span class="sxs-lookup"><span data-stu-id="0b0f2-119">This method does not support the [OData query parameters](/graph//query-parameters) to help customize the response (`$filter` is not supported).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b0f2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b0f2-120">Request headers</span></span>

| <span data-ttu-id="0b0f2-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0b0f2-121">Name</span></span>       | <span data-ttu-id="0b0f2-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b0f2-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="0b0f2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b0f2-123">Authorization</span></span>  | <span data-ttu-id="0b0f2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b0f2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b0f2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b0f2-126">Request body</span></span>
<span data-ttu-id="0b0f2-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0b0f2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b0f2-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b0f2-128">Response</span></span>

<span data-ttu-id="0b0f2-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [subscribedSku](../resources/subscribedsku.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b0f2-129">If successful, this method returns a `200 OK` response code and collection of [subscribedSku](../resources/subscribedsku.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0b0f2-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b0f2-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0b0f2-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b0f2-131">Request</span></span>
<span data-ttu-id="0b0f2-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b0f2-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0b0f2-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b0f2-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscribedskus"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/subscribedSkus
```
# <a name="c"></a>[<span data-ttu-id="0b0f2-134">C#</span><span class="sxs-lookup"><span data-stu-id="0b0f2-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscribedskus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b0f2-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b0f2-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscribedskus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b0f2-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b0f2-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscribedskus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b0f2-137">Java</span><span class="sxs-lookup"><span data-stu-id="0b0f2-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscribedskus-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0b0f2-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b0f2-138">Response</span></span>
<span data-ttu-id="0b0f2-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b0f2-139">Here is an example of the response.</span></span> <span data-ttu-id="0b0f2-140">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0b0f2-140">Note: The response object shown here might be shortened for readability.</span></span>
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


