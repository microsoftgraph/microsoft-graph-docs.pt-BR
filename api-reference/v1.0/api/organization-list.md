---
title: Listar organização
description: Recupere uma lista de objetos de organização.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e62157fe7fec29df4afd1e4d931a28fa6e3b77f8
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33611658"
---
# <a name="list-organization"></a><span data-ttu-id="0f2c2-103">Listar organização</span><span class="sxs-lookup"><span data-stu-id="0f2c2-103">List organization</span></span>



<span data-ttu-id="0f2c2-104">Recupere uma lista de objetos de organização.</span><span class="sxs-lookup"><span data-stu-id="0f2c2-104">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="0f2c2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0f2c2-105">Permissions</span></span>
<span data-ttu-id="0f2c2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f2c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f2c2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f2c2-108">Permission type</span></span>      | <span data-ttu-id="0f2c2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0f2c2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f2c2-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f2c2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0f2c2-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f2c2-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="0f2c2-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f2c2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f2c2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f2c2-113">Not supported.</span></span>    |
|<span data-ttu-id="0f2c2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f2c2-114">Application</span></span> | <span data-ttu-id="0f2c2-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f2c2-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="0f2c2-116">Observação: os aplicativos que têm a permissão User.Read só conseguem ler as propriedades *id*, *displayName* e *verifiedDomains* da organização.</span><span class="sxs-lookup"><span data-stu-id="0f2c2-116">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="0f2c2-117">Todas as outras propriedades retornarão valores `null`.</span><span class="sxs-lookup"><span data-stu-id="0f2c2-117">All other properties will return with `null` values.</span></span> <span data-ttu-id="0f2c2-118">Para ler todas as propriedades, use Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="0f2c2-118">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="0f2c2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f2c2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0f2c2-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0f2c2-120">Optional query parameters</span></span>
<span data-ttu-id="0f2c2-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0f2c2-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0f2c2-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f2c2-122">Request headers</span></span>
| <span data-ttu-id="0f2c2-123">Nome</span><span class="sxs-lookup"><span data-stu-id="0f2c2-123">Name</span></span>       | <span data-ttu-id="0f2c2-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f2c2-124">Type</span></span> | <span data-ttu-id="0f2c2-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f2c2-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0f2c2-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f2c2-126">Authorization</span></span>  | <span data-ttu-id="0f2c2-127">string</span><span class="sxs-lookup"><span data-stu-id="0f2c2-127">string</span></span>  | <span data-ttu-id="0f2c2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f2c2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f2c2-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f2c2-130">Request body</span></span>
<span data-ttu-id="0f2c2-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0f2c2-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f2c2-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f2c2-132">Response</span></span>

<span data-ttu-id="0f2c2-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [organization](../resources/organization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f2c2-133">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0f2c2-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f2c2-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0f2c2-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f2c2-135">Request</span></span>
<span data-ttu-id="0f2c2-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f2c2-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```http
GET https://graph.microsoft.com/beta/organization
```
##### <a name="response"></a><span data-ttu-id="0f2c2-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f2c2-137">Response</span></span>
<span data-ttu-id="0f2c2-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0f2c2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="0f2c2-141">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="0f2c2-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0f2c2-142">Basic</span><span class="sxs-lookup"><span data-stu-id="0f2c2-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_organization-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0f2c2-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0f2c2-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_organization-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/organization-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/organization-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
