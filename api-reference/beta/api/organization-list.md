---
title: Listar organização
description: Recupere uma lista de objetos de organização.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a36abc65a574ae1fbb2e47ec1d44e1d288f3df62
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35995605"
---
# <a name="list-organization"></a><span data-ttu-id="34ef5-103">Listar organização</span><span class="sxs-lookup"><span data-stu-id="34ef5-103">List organization</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34ef5-104">Recupere uma lista de objetos de organização.</span><span class="sxs-lookup"><span data-stu-id="34ef5-104">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="34ef5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="34ef5-105">Permissions</span></span>
<span data-ttu-id="34ef5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34ef5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34ef5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34ef5-108">Permission type</span></span>      | <span data-ttu-id="34ef5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="34ef5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34ef5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34ef5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="34ef5-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34ef5-111">Not supported.</span></span>    |
|<span data-ttu-id="34ef5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34ef5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34ef5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34ef5-113">Not supported.</span></span>    |
|<span data-ttu-id="34ef5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34ef5-114">Application</span></span> | <span data-ttu-id="34ef5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34ef5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="34ef5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34ef5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="34ef5-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="34ef5-117">Optional query parameters</span></span>
<span data-ttu-id="34ef5-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="34ef5-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="34ef5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34ef5-119">Request headers</span></span>
| <span data-ttu-id="34ef5-120">Nome</span><span class="sxs-lookup"><span data-stu-id="34ef5-120">Name</span></span>       | <span data-ttu-id="34ef5-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="34ef5-121">Type</span></span> | <span data-ttu-id="34ef5-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="34ef5-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="34ef5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="34ef5-123">Authorization</span></span>  | <span data-ttu-id="34ef5-124">string</span><span class="sxs-lookup"><span data-stu-id="34ef5-124">string</span></span>  | <span data-ttu-id="34ef5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34ef5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="34ef5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34ef5-127">Request body</span></span>
<span data-ttu-id="34ef5-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="34ef5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34ef5-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="34ef5-129">Response</span></span>

<span data-ttu-id="34ef5-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [organization](../resources/organization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34ef5-130">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="34ef5-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34ef5-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="34ef5-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34ef5-132">Request</span></span>
<span data-ttu-id="34ef5-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34ef5-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="34ef5-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="34ef5-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```http
GET https://graph.microsoft.com/beta/organization
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="34ef5-135">C#</span><span class="sxs-lookup"><span data-stu-id="34ef5-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="34ef5-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="34ef5-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="34ef5-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="34ef5-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="34ef5-138">Java</span><span class="sxs-lookup"><span data-stu-id="34ef5-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="34ef5-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="34ef5-139">Response</span></span>
<span data-ttu-id="34ef5-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34ef5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
