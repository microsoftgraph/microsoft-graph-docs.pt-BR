---
title: Listar organização
description: Recupere uma lista de objetos de organização.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e626e5efc7668f8b4b958979bda5a7ed3a7492ed
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975509"
---
# <a name="list-organization"></a><span data-ttu-id="9fecc-103">Listar organização</span><span class="sxs-lookup"><span data-stu-id="9fecc-103">List organization</span></span>

<span data-ttu-id="9fecc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fecc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fecc-105">Recupere uma lista de objetos de organização.</span><span class="sxs-lookup"><span data-stu-id="9fecc-105">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="9fecc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9fecc-106">Permissions</span></span>
<span data-ttu-id="9fecc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fecc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fecc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9fecc-109">Permission type</span></span>      | <span data-ttu-id="9fecc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9fecc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9fecc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9fecc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9fecc-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fecc-112">Not supported.</span></span>    |
|<span data-ttu-id="9fecc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9fecc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fecc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fecc-114">Not supported.</span></span>    |
|<span data-ttu-id="9fecc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9fecc-115">Application</span></span> | <span data-ttu-id="9fecc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fecc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9fecc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9fecc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9fecc-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9fecc-118">Optional query parameters</span></span>
<span data-ttu-id="9fecc-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9fecc-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9fecc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9fecc-120">Request headers</span></span>
| <span data-ttu-id="9fecc-121">Nome</span><span class="sxs-lookup"><span data-stu-id="9fecc-121">Name</span></span>       | <span data-ttu-id="9fecc-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="9fecc-122">Type</span></span> | <span data-ttu-id="9fecc-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fecc-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9fecc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9fecc-124">Authorization</span></span>  | <span data-ttu-id="9fecc-125">string</span><span class="sxs-lookup"><span data-stu-id="9fecc-125">string</span></span>  | <span data-ttu-id="9fecc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9fecc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9fecc-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9fecc-128">Request body</span></span>
<span data-ttu-id="9fecc-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9fecc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9fecc-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fecc-130">Response</span></span>

<span data-ttu-id="9fecc-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [organization](../resources/organization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9fecc-131">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9fecc-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9fecc-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9fecc-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9fecc-133">Request</span></span>
<span data-ttu-id="9fecc-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9fecc-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9fecc-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9fecc-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/organization
```
# <a name="c"></a>[<span data-ttu-id="9fecc-136">C#</span><span class="sxs-lookup"><span data-stu-id="9fecc-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9fecc-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9fecc-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9fecc-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9fecc-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9fecc-139">Java</span><span class="sxs-lookup"><span data-stu-id="9fecc-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9fecc-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fecc-140">Response</span></span>
<span data-ttu-id="9fecc-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9fecc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 500

{
  "value": [
    {
      "assignedPlans": [
        {
          "assignedDateTime": "2016-10-19T10:37:00Z",
          "capabilityStatus": "capabilityStatus-value",
          "service": "service-value",
          "servicePlanId": "servicePlanId-value"
        }
      ],
      "businessPhones": [
        "businessPhones-value"
      ],
      "city": "city-value",
      "country": "country-value",
      "countryLetterCode": "countryLetterCode-value",
      "displayName": "displayName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
