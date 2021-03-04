---
title: 'domain: verify'
description: Valida a propriedade do domínio.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 32e559328e834f1f1bcce025222556d4b22fab7b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436439"
---
# <a name="domain-verify"></a><span data-ttu-id="72444-103">domain: verify</span><span class="sxs-lookup"><span data-stu-id="72444-103">domain: verify</span></span>

<span data-ttu-id="72444-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72444-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72444-105">Valida a propriedade do domínio.</span><span class="sxs-lookup"><span data-stu-id="72444-105">Validates the ownership of the domain.</span></span>

> <span data-ttu-id="72444-p101">**Importante:** Aplica-se somente a um domínio não verificado. Para um domínio não verificado, a propriedade isVerified do [domínio](../resources/domain.md) é falsa.</span><span class="sxs-lookup"><span data-stu-id="72444-p101">**Important:** Only applies to an unverified domain. For an unverified domain, the isVerified property of the [domain](../resources/domain.md) is false.</span></span>

## <a name="permissions"></a><span data-ttu-id="72444-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="72444-108">Permissions</span></span>

<span data-ttu-id="72444-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72444-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="72444-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72444-111">Permission type</span></span>      | <span data-ttu-id="72444-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="72444-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72444-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72444-113">Delegated (work or school account)</span></span> | <span data-ttu-id="72444-114">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="72444-114">Directory.Read.All</span></span>    |
|<span data-ttu-id="72444-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72444-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72444-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72444-116">Not supported.</span></span>    |
|<span data-ttu-id="72444-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72444-117">Application</span></span> | <span data-ttu-id="72444-118">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72444-118">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="72444-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72444-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/verify
```

> <span data-ttu-id="72444-120">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="72444-120">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72444-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72444-121">Request headers</span></span>

| <span data-ttu-id="72444-122">Nome</span><span class="sxs-lookup"><span data-stu-id="72444-122">Name</span></span>       | <span data-ttu-id="72444-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="72444-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="72444-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="72444-124">Authorization</span></span>  | <span data-ttu-id="72444-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72444-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="72444-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="72444-127">Content-Type</span></span>  | <span data-ttu-id="72444-128">application/json</span><span class="sxs-lookup"><span data-stu-id="72444-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="72444-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72444-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="72444-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="72444-130">Response</span></span>

<span data-ttu-id="72444-131">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [domain](../resources/domain.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72444-131">If successful, this method returns `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72444-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72444-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="72444-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72444-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="72444-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="72444-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "domain_verify"
}-->
```http
POST https://graph.microsoft.com/beta/domains/contoso.com/verify
```
# <a name="c"></a>[<span data-ttu-id="72444-135">C#</span><span class="sxs-lookup"><span data-stu-id="72444-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-verify-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72444-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72444-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-verify-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72444-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72444-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-verify-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="72444-138">Java</span><span class="sxs-lookup"><span data-stu-id="72444-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/domain-verify-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="72444-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="72444-139">Response</span></span>
<span data-ttu-id="72444-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72444-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "name": "contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domain: verify",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


