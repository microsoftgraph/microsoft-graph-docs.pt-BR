---
title: Listar organização
description: Recupere uma lista de objetos de organização.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d594c417cbd8e8127b80eed5e57bd5ed70ff7931
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458553"
---
# <a name="list-organization"></a><span data-ttu-id="e99a9-103">Listar organização</span><span class="sxs-lookup"><span data-stu-id="e99a9-103">List organization</span></span>

<span data-ttu-id="e99a9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e99a9-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="e99a9-105">Recupere uma lista de objetos de organização.</span><span class="sxs-lookup"><span data-stu-id="e99a9-105">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="e99a9-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="e99a9-106">Permissions</span></span>
<span data-ttu-id="e99a9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e99a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e99a9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e99a9-109">Permission type</span></span>      | <span data-ttu-id="e99a9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e99a9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e99a9-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e99a9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e99a9-112">User.Read, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e99a9-112">User.Read, Directory.Read.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="e99a9-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e99a9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e99a9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e99a9-114">Not supported.</span></span>    |
|<span data-ttu-id="e99a9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e99a9-115">Application</span></span> | <span data-ttu-id="e99a9-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e99a9-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="e99a9-117">Observação: os aplicativos que têm a permissão User.Read só conseguem ler as propriedades *id*, *displayName* e *verifiedDomains* da organização.</span><span class="sxs-lookup"><span data-stu-id="e99a9-117">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="e99a9-118">Todas as outras propriedades retornarão valores `null`.</span><span class="sxs-lookup"><span data-stu-id="e99a9-118">All other properties will return with `null` values.</span></span> <span data-ttu-id="e99a9-119">Para ler todas as propriedades, use Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="e99a9-119">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="e99a9-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e99a9-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e99a9-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e99a9-121">Optional query parameters</span></span>
<span data-ttu-id="e99a9-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e99a9-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e99a9-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e99a9-123">Request headers</span></span>
| <span data-ttu-id="e99a9-124">Nome</span><span class="sxs-lookup"><span data-stu-id="e99a9-124">Name</span></span>       | <span data-ttu-id="e99a9-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="e99a9-125">Type</span></span> | <span data-ttu-id="e99a9-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="e99a9-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e99a9-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="e99a9-127">Authorization</span></span>  | <span data-ttu-id="e99a9-128">string</span><span class="sxs-lookup"><span data-stu-id="e99a9-128">string</span></span>  | <span data-ttu-id="e99a9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e99a9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e99a9-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e99a9-131">Request body</span></span>
<span data-ttu-id="e99a9-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e99a9-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e99a9-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e99a9-133">Response</span></span>

<span data-ttu-id="e99a9-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [organization](../resources/organization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e99a9-134">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e99a9-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e99a9-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e99a9-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e99a9-136">Request</span></span>
<span data-ttu-id="e99a9-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e99a9-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e99a9-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="e99a9-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization
```
# <a name="c"></a>[<span data-ttu-id="e99a9-139">C#</span><span class="sxs-lookup"><span data-stu-id="e99a9-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e99a9-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e99a9-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e99a9-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e99a9-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e99a9-142">Java</span><span class="sxs-lookup"><span data-stu-id="e99a9-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e99a9-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="e99a9-143">Response</span></span>
<span data-ttu-id="e99a9-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e99a9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
