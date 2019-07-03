---
title: Obter organização
description: Recupere as propriedades e os relacionamentos da organização autenticada no momento.
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 124f4a05f30196b622b62ecd82ea15a892e3682b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448330"
---
# <a name="get-organization"></a><span data-ttu-id="af516-103">Obter organização</span><span class="sxs-lookup"><span data-stu-id="af516-103">Get organization</span></span>

<span data-ttu-id="af516-104">Recupere as propriedades e os relacionamentos da organização autenticada no momento.</span><span class="sxs-lookup"><span data-stu-id="af516-104">Retrieve the properties and relationships of currently authenticated organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="af516-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="af516-105">Permissions</span></span>

<span data-ttu-id="af516-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af516-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af516-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af516-108">Permission type</span></span>      | <span data-ttu-id="af516-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="af516-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af516-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af516-110">Delegated (work or school account)</span></span> | <span data-ttu-id="af516-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af516-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="af516-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af516-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af516-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af516-113">Not supported.</span></span>    |
|<span data-ttu-id="af516-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af516-114">Application</span></span> | <span data-ttu-id="af516-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af516-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="af516-116">Observação: os aplicativos que têm a permissão User.Read só conseguem ler as propriedades *id*, *displayName* e *verifiedDomains* da organização.</span><span class="sxs-lookup"><span data-stu-id="af516-116">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="af516-117">Todas as outras propriedades retornarão valores `null`.</span><span class="sxs-lookup"><span data-stu-id="af516-117">All other properties will return with `null` values.</span></span> <span data-ttu-id="af516-118">Para ler todas as propriedades, use Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="af516-118">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="af516-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af516-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization
```

## <a name="optional-query-parameters"></a><span data-ttu-id="af516-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="af516-120">Optional query parameters</span></span>

<span data-ttu-id="af516-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="af516-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="af516-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af516-122">Request headers</span></span>

| <span data-ttu-id="af516-123">Nome</span><span class="sxs-lookup"><span data-stu-id="af516-123">Name</span></span>       | <span data-ttu-id="af516-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="af516-124">Type</span></span> | <span data-ttu-id="af516-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="af516-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="af516-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="af516-126">Authorization</span></span>  | <span data-ttu-id="af516-127">string</span><span class="sxs-lookup"><span data-stu-id="af516-127">string</span></span>  | <span data-ttu-id="af516-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af516-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="af516-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af516-130">Request body</span></span>

<span data-ttu-id="af516-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="af516-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af516-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="af516-132">Response</span></span>

<span data-ttu-id="af516-133">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de um objeto de [organização](../resources/organization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af516-133">If successful, this method returns a `200 OK` response code and a collection of one [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af516-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af516-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="af516-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af516-135">Request</span></span>

<span data-ttu-id="af516-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="af516-136">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="af516-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="af516-137">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->

```http
GET https://graph.microsoft.com/v1.0/organization
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="af516-138">C#</span><span class="sxs-lookup"><span data-stu-id="af516-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="af516-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="af516-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="af516-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="af516-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="af516-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="af516-141">Response</span></span>

<span data-ttu-id="af516-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af516-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 411

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#organization",
  "value": [
    {
      "assignedPlans": [
        {
          "assignedDateTime": "datetime-value",
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
  "description": "Get organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
