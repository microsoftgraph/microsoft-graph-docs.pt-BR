---
title: 'domain: verify'
description: Valida a propriedade do domínio.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 17d8b150eea52db684f4472bc8d6ea324800a730
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276983"
---
# <a name="domain-verify"></a><span data-ttu-id="b02f9-103">domain: verify</span><span class="sxs-lookup"><span data-stu-id="b02f9-103">domain: verify</span></span>

<span data-ttu-id="b02f9-104">Valida a propriedade do domínio.</span><span class="sxs-lookup"><span data-stu-id="b02f9-104">Validates the ownership of the domain.</span></span>

> <span data-ttu-id="b02f9-p101">**Importante:** Aplica-se somente a um domínio não verificado. Para um domínio não verificado, a propriedade isVerified do [domínio](../resources/domain.md) é falsa.</span><span class="sxs-lookup"><span data-stu-id="b02f9-p101">**Important:** Only applies to an unverified domain. For an unverified domain, the isVerified property of the [domain](../resources/domain.md) is false.</span></span>

## <a name="permissions"></a><span data-ttu-id="b02f9-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b02f9-107">Permissions</span></span>

<span data-ttu-id="b02f9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b02f9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b02f9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b02f9-110">Permission type</span></span>      | <span data-ttu-id="b02f9-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b02f9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b02f9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b02f9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b02f9-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b02f9-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="b02f9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b02f9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b02f9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b02f9-115">Not supported.</span></span>    |
|<span data-ttu-id="b02f9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b02f9-116">Application</span></span> | <span data-ttu-id="b02f9-117">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b02f9-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b02f9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b02f9-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/verify
```

> <span data-ttu-id="b02f9-119">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="b02f9-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b02f9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b02f9-120">Request headers</span></span>

| <span data-ttu-id="b02f9-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b02f9-121">Name</span></span>       | <span data-ttu-id="b02f9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b02f9-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b02f9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b02f9-123">Authorization</span></span>  | <span data-ttu-id="b02f9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b02f9-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="b02f9-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b02f9-126">Content-Type</span></span>  | <span data-ttu-id="b02f9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b02f9-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b02f9-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b02f9-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="b02f9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b02f9-129">Response</span></span>

<span data-ttu-id="b02f9-130">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [domain](../resources/domain.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b02f9-130">If successful, this method returns `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b02f9-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b02f9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b02f9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b02f9-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "domain_verify"
}-->
```http
POST https://graph.microsoft.com/v1.0/domains/{domain-name}/verify
```

##### <a name="response"></a><span data-ttu-id="b02f9-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b02f9-133">Response</span></span>
<span data-ttu-id="b02f9-p104">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b02f9-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "id": "contoso.com"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b02f9-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="b02f9-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b02f9-137">C#</span><span class="sxs-lookup"><span data-stu-id="b02f9-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/domain_verify-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b02f9-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="b02f9-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/domain_verify-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b02f9-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b02f9-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/domain_verify-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: verify",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/domain-verify.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/domain-verify.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/domain-verify.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
