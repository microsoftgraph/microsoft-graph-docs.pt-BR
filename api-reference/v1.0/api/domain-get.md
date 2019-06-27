---
title: Obter domínio
description: Recupere as propriedades e os relacionamentos do objeto Domain.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 276e7277e20d1454bcb7b619d5219ed471727e7a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272125"
---
# <a name="get-domain"></a><span data-ttu-id="7bc96-103">Obter domínio</span><span class="sxs-lookup"><span data-stu-id="7bc96-103">Get domain</span></span>

<span data-ttu-id="7bc96-104">Recupere as propriedades e os relacionamentos do objeto Domain.</span><span class="sxs-lookup"><span data-stu-id="7bc96-104">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7bc96-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7bc96-105">Permissions</span></span>

<span data-ttu-id="7bc96-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bc96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7bc96-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7bc96-108">Permission type</span></span>      | <span data-ttu-id="7bc96-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7bc96-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7bc96-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7bc96-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7bc96-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7bc96-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="7bc96-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7bc96-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bc96-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7bc96-113">Not supported.</span></span>    |
|<span data-ttu-id="7bc96-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7bc96-114">Application</span></span> | <span data-ttu-id="7bc96-115">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bc96-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7bc96-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7bc96-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="7bc96-117">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="7bc96-117">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="7bc96-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7bc96-118">Optional query parameters</span></span>

<span data-ttu-id="7bc96-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7bc96-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7bc96-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7bc96-120">Request headers</span></span>

| <span data-ttu-id="7bc96-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7bc96-121">Name</span></span>      |<span data-ttu-id="7bc96-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bc96-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7bc96-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7bc96-123">Authorization</span></span>  | <span data-ttu-id="7bc96-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7bc96-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7bc96-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7bc96-126">Content-Type</span></span>  | <span data-ttu-id="7bc96-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7bc96-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7bc96-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7bc96-128">Request body</span></span>
<span data-ttu-id="7bc96-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7bc96-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7bc96-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bc96-130">Response</span></span>

<span data-ttu-id="7bc96-131">Se bem-sucedido, este método retorna o `200 OK` código de resposta e o objeto [Domain](../resources/domain.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7bc96-131">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7bc96-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7bc96-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7bc96-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7bc96-133">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "get_domain"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/contoso.com
```
##### <a name="response"></a><span data-ttu-id="7bc96-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bc96-134">Response</span></span>
<span data-ttu-id="7bc96-p103">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7bc96-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "id": "contoso.com",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7bc96-137">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="7bc96-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7bc96-138">C#</span><span class="sxs-lookup"><span data-stu-id="7bc96-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_domain-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7bc96-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="7bc96-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_domain-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7bc96-140">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7bc96-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_domain-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/domain-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/domain-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/domain-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
