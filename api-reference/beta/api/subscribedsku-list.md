---
title: Listar subscribedSkus
description: Recupere a lista de assinaturas comerciais que uma organização adquiriu.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1714be2ed9a26e9e49f4c863cda9a29a7f975857
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36363673"
---
# <a name="list-subscribedskus"></a><span data-ttu-id="48629-103">Listar subscribedSkus</span><span class="sxs-lookup"><span data-stu-id="48629-103">List subscribedSkus</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48629-104">Obtenha a lista de assinaturas comerciais que uma organização adquiriu.</span><span class="sxs-lookup"><span data-stu-id="48629-104">Get the list of commercial subscriptions that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="48629-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="48629-105">Permissions</span></span>
<span data-ttu-id="48629-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48629-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="48629-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48629-108">Permission type</span></span>      | <span data-ttu-id="48629-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="48629-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48629-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48629-110">Delegated (work or school account)</span></span> | <span data-ttu-id="48629-111">Organization. Read. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="48629-111">Organization.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="48629-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48629-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48629-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48629-113">Not supported.</span></span>    |
|<span data-ttu-id="48629-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48629-114">Application</span></span> | <span data-ttu-id="48629-115">Organization. Read. All, Directory. Read. All, Organization. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="48629-115">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="48629-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48629-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus
```
## <a name="optional-query-parameters"></a><span data-ttu-id="48629-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="48629-117">Optional query parameters</span></span>
<span data-ttu-id="48629-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="48629-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="48629-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48629-119">Request headers</span></span>

| <span data-ttu-id="48629-120">Nome</span><span class="sxs-lookup"><span data-stu-id="48629-120">Name</span></span>       | <span data-ttu-id="48629-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="48629-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="48629-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="48629-122">Authorization</span></span>  | <span data-ttu-id="48629-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48629-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48629-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48629-125">Request body</span></span>
<span data-ttu-id="48629-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="48629-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48629-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="48629-127">Response</span></span>

<span data-ttu-id="48629-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [subscribedSku](../resources/subscribedsku.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="48629-128">If successful, this method returns a `200 OK` response code and collection of [subscribedSku](../resources/subscribedsku.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="48629-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="48629-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="48629-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48629-130">Request</span></span>
<span data-ttu-id="48629-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="48629-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="48629-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="48629-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscribedskus"
}-->
```http
GET https://graph.microsoft.com/beta/subscribedSkus
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="48629-133">C#</span><span class="sxs-lookup"><span data-stu-id="48629-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscribedskus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="48629-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48629-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscribedskus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="48629-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="48629-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscribedskus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="48629-136">Java</span><span class="sxs-lookup"><span data-stu-id="48629-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscribedskus-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="48629-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="48629-137">Response</span></span>
<span data-ttu-id="48629-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="48629-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
