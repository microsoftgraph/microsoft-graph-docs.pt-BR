---
title: Atualizar domínio
description: Atualize as propriedades do objeto domain.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: fc400d4790326e79d8ad8dea387d6027baf8f1de
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787300"
---
# <a name="update-domain"></a><span data-ttu-id="d8bd8-103">Atualizar domínio</span><span class="sxs-lookup"><span data-stu-id="d8bd8-103">Update domain</span></span>

<span data-ttu-id="d8bd8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8bd8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d8bd8-105">Atualize as propriedades do objeto domain.</span><span class="sxs-lookup"><span data-stu-id="d8bd8-105">Update the properties of domain object.</span></span>

> <span data-ttu-id="d8bd8-106">**Importante:** Somente domínios verificados podem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="d8bd8-106">**Important:** Only verified domains can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8bd8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d8bd8-107">Permissions</span></span>

<span data-ttu-id="d8bd8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8bd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d8bd8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8bd8-110">Permission type</span></span>      | <span data-ttu-id="d8bd8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d8bd8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8bd8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8bd8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d8bd8-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d8bd8-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d8bd8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8bd8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8bd8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8bd8-115">Not supported.</span></span>    |
|<span data-ttu-id="d8bd8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8bd8-116">Application</span></span> | <span data-ttu-id="d8bd8-117">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8bd8-117">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8bd8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8bd8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="d8bd8-119">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="d8bd8-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d8bd8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8bd8-120">Request headers</span></span>

| <span data-ttu-id="d8bd8-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d8bd8-121">Name</span></span>       | <span data-ttu-id="d8bd8-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8bd8-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d8bd8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8bd8-123">Authorization</span></span>  | <span data-ttu-id="d8bd8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8bd8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d8bd8-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d8bd8-126">Content-Type</span></span>  | <span data-ttu-id="d8bd8-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d8bd8-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8bd8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8bd8-128">Request body</span></span>

<span data-ttu-id="d8bd8-129">No corpo da solicitação, fornece os valores para campos relevantes a serem atualizados.</span><span class="sxs-lookup"><span data-stu-id="d8bd8-129">In the request body, supply the values for relevant fields to be updated.</span></span> <span data-ttu-id="d8bd8-130">As propriedades existentes não incluídas no corpo da solicitação manterão seus valores anteriores ou serão recalculadas com base em alterações em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="d8bd8-130">Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d8bd8-131">Para melhor desempenho, inclua apenas valores alterados.</span><span class="sxs-lookup"><span data-stu-id="d8bd8-131">For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="d8bd8-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8bd8-132">Response</span></span>

<span data-ttu-id="d8bd8-133">Se tiver êxito, este método retornará um `204 No Content` código de resposta e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d8bd8-133">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8bd8-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8bd8-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d8bd8-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8bd8-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d8bd8-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8bd8-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "update_domain"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/domains/contoso.com
Content-type: application/json

{
  "isDefault": true,
  "supportedServices": [
    "Email",
    "OfficeCommunicationsOnline"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="d8bd8-137">C#</span><span class="sxs-lookup"><span data-stu-id="d8bd8-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d8bd8-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8bd8-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d8bd8-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8bd8-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d8bd8-140">Java</span><span class="sxs-lookup"><span data-stu-id="d8bd8-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-domain-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d8bd8-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8bd8-141">Response</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

