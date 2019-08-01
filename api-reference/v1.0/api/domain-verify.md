---
title: 'domain: verify'
description: Valida a propriedade do domínio.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0b6ea87c1d9bc113fa59724deda411dbe18b1bc8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36016507"
---
# <a name="domain-verify"></a><span data-ttu-id="ef41a-103">domain: verify</span><span class="sxs-lookup"><span data-stu-id="ef41a-103">domain: verify</span></span>

<span data-ttu-id="ef41a-104">Valida a propriedade do domínio.</span><span class="sxs-lookup"><span data-stu-id="ef41a-104">Validates the ownership of the domain.</span></span>

> <span data-ttu-id="ef41a-p101">**Importante:** Aplica-se somente a um domínio não verificado. Para um domínio não verificado, a propriedade isVerified do [domínio](../resources/domain.md) é falsa.</span><span class="sxs-lookup"><span data-stu-id="ef41a-p101">**Important:** Only applies to an unverified domain. For an unverified domain, the isVerified property of the [domain](../resources/domain.md) is false.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef41a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ef41a-107">Permissions</span></span>

<span data-ttu-id="ef41a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef41a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ef41a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef41a-110">Permission type</span></span>      | <span data-ttu-id="ef41a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ef41a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef41a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef41a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ef41a-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef41a-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="ef41a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef41a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef41a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef41a-115">Not supported.</span></span>    |
|<span data-ttu-id="ef41a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef41a-116">Application</span></span> | <span data-ttu-id="ef41a-117">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef41a-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef41a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef41a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/verify
```

> <span data-ttu-id="ef41a-119">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="ef41a-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef41a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef41a-120">Request headers</span></span>

| <span data-ttu-id="ef41a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ef41a-121">Name</span></span>       | <span data-ttu-id="ef41a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef41a-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ef41a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef41a-123">Authorization</span></span>  | <span data-ttu-id="ef41a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef41a-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="ef41a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ef41a-126">Content-Type</span></span>  | <span data-ttu-id="ef41a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ef41a-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef41a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef41a-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="ef41a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef41a-129">Response</span></span>

<span data-ttu-id="ef41a-130">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [domain](../resources/domain.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef41a-130">If successful, this method returns `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef41a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef41a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ef41a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef41a-132">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ef41a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef41a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "domain_verify"
}-->
```http
POST https://graph.microsoft.com/v1.0/domains/{domain-name}/verify
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ef41a-134">C#</span><span class="sxs-lookup"><span data-stu-id="ef41a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-verify-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ef41a-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="ef41a-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-verify-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ef41a-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ef41a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-verify-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ef41a-137">Java</span><span class="sxs-lookup"><span data-stu-id="ef41a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/domain-verify-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ef41a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef41a-138">Response</span></span>
<span data-ttu-id="ef41a-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ef41a-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: verify",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
