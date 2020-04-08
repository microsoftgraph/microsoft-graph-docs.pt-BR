---
title: Atualizar domínio
description: Atualize as propriedades do objeto Domain.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6c39f488b3d41c099d996023617d726be09a9cdf
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2020
ms.locfileid: "43179840"
---
# <a name="update-domain"></a><span data-ttu-id="83609-103">Atualizar domínio</span><span class="sxs-lookup"><span data-stu-id="83609-103">Update domain</span></span>

<span data-ttu-id="83609-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83609-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83609-105">Atualize as propriedades do objeto Domain.</span><span class="sxs-lookup"><span data-stu-id="83609-105">Update the properties of domain object.</span></span>

> <span data-ttu-id="83609-106">**Importante:** Somente os domínios verificados podem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="83609-106">**Important:** Only verified domains can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="83609-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="83609-107">Permissions</span></span>

<span data-ttu-id="83609-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83609-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="83609-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83609-110">Permission type</span></span>      | <span data-ttu-id="83609-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="83609-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83609-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83609-112">Delegated (work or school account)</span></span> | <span data-ttu-id="83609-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="83609-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="83609-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83609-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83609-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83609-115">Not supported.</span></span>    |
|<span data-ttu-id="83609-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="83609-116">Application</span></span> | <span data-ttu-id="83609-117">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83609-117">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="83609-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83609-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="83609-119">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="83609-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="83609-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83609-120">Request headers</span></span>

| <span data-ttu-id="83609-121">Nome</span><span class="sxs-lookup"><span data-stu-id="83609-121">Name</span></span>       | <span data-ttu-id="83609-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="83609-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="83609-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="83609-123">Authorization</span></span>  | <span data-ttu-id="83609-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83609-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="83609-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="83609-126">Content-Type</span></span>  | <span data-ttu-id="83609-127">application/json</span><span class="sxs-lookup"><span data-stu-id="83609-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="83609-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83609-128">Request body</span></span>

<span data-ttu-id="83609-129">No corpo da solicitação, forneça os valores de campos relevantes a serem atualizados.</span><span class="sxs-lookup"><span data-stu-id="83609-129">In the request body, supply the values for relevant fields to be updated.</span></span> <span data-ttu-id="83609-130">As propriedades existentes não incluídas no corpo da solicitação manterão seus valores anteriores ou serão recalculadas com base nas alterações feitas em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="83609-130">Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="83609-131">Para obter o melhor desempenho, inclua somente valores alterados.</span><span class="sxs-lookup"><span data-stu-id="83609-131">For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="83609-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="83609-132">Response</span></span>

<span data-ttu-id="83609-133">Se tiver êxito, este método retornará `204 No Content` um código de resposta e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="83609-133">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="83609-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83609-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="83609-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83609-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="83609-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="83609-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_domain"
}-->
```http
PATCH https://graph.microsoft.com/beta/domains/contoso.com
Content-type: application/json

{
  "isDefault": true,
  "supportedServices": [
    "Email",
    "OfficeCommunicationsOnline"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="83609-137">C#</span><span class="sxs-lookup"><span data-stu-id="83609-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="83609-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83609-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="83609-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="83609-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="83609-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="83609-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
