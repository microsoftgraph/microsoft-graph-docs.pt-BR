---
title: Listar organização
description: Recupere uma lista de objetos de organização.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a56d45fe0570b241156096814792b145b32c579f
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36730110"
---
# <a name="list-organization"></a><span data-ttu-id="e078b-103">Listar organização</span><span class="sxs-lookup"><span data-stu-id="e078b-103">List organization</span></span>



<span data-ttu-id="e078b-104">Recupere uma lista de objetos de organização.</span><span class="sxs-lookup"><span data-stu-id="e078b-104">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="e078b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e078b-105">Permissions</span></span>
<span data-ttu-id="e078b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e078b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e078b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e078b-108">Permission type</span></span>      | <span data-ttu-id="e078b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e078b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e078b-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e078b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e078b-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e078b-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="e078b-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e078b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e078b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e078b-113">Not supported.</span></span>    |
|<span data-ttu-id="e078b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e078b-114">Application</span></span> | <span data-ttu-id="e078b-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e078b-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="e078b-116">Observação: os aplicativos que têm a permissão User.Read só conseguem ler as propriedades *id*, *displayName* e *verifiedDomains* da organização.</span><span class="sxs-lookup"><span data-stu-id="e078b-116">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="e078b-117">Todas as outras propriedades retornarão valores `null`.</span><span class="sxs-lookup"><span data-stu-id="e078b-117">All other properties will return with `null` values.</span></span> <span data-ttu-id="e078b-118">Para ler todas as propriedades, use Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="e078b-118">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="e078b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e078b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e078b-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e078b-120">Optional query parameters</span></span>
<span data-ttu-id="e078b-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e078b-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e078b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e078b-122">Request headers</span></span>
| <span data-ttu-id="e078b-123">Nome</span><span class="sxs-lookup"><span data-stu-id="e078b-123">Name</span></span>       | <span data-ttu-id="e078b-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="e078b-124">Type</span></span> | <span data-ttu-id="e078b-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="e078b-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e078b-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="e078b-126">Authorization</span></span>  | <span data-ttu-id="e078b-127">string</span><span class="sxs-lookup"><span data-stu-id="e078b-127">string</span></span>  | <span data-ttu-id="e078b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e078b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e078b-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e078b-130">Request body</span></span>
<span data-ttu-id="e078b-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e078b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e078b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e078b-132">Response</span></span>

<span data-ttu-id="e078b-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [organization](../resources/organization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e078b-133">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e078b-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e078b-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e078b-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e078b-135">Request</span></span>
<span data-ttu-id="e078b-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e078b-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e078b-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="e078b-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/organization
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e078b-138">C#</span><span class="sxs-lookup"><span data-stu-id="e078b-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e078b-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e078b-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e078b-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e078b-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e078b-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e078b-141">Response</span></span>
<span data-ttu-id="e078b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e078b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
