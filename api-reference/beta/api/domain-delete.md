---
title: Excluir domínio
description: Exclui um domínio de um locatário.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 5f00627823d4a9cc571143c8e0e09ba297bd4902
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046535"
---
# <a name="delete-domain"></a><span data-ttu-id="19b21-103">Excluir domínio</span><span class="sxs-lookup"><span data-stu-id="19b21-103">Delete domain</span></span>

<span data-ttu-id="19b21-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19b21-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19b21-105">Exclui um domínio de um locatário.</span><span class="sxs-lookup"><span data-stu-id="19b21-105">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="19b21-106">**Importante:** Domínios excluídos não podem ser recuperados.</span><span class="sxs-lookup"><span data-stu-id="19b21-106">**Important:** Deleted domains are not recoverable.</span></span>

## <a name="permissions"></a><span data-ttu-id="19b21-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="19b21-107">Permissions</span></span>

<span data-ttu-id="19b21-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19b21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="19b21-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19b21-110">Permission type</span></span>      | <span data-ttu-id="19b21-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="19b21-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19b21-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19b21-112">Delegated (work or school account)</span></span> | <span data-ttu-id="19b21-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="19b21-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="19b21-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19b21-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19b21-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19b21-115">Not supported.</span></span>    |
|<span data-ttu-id="19b21-116">Application</span><span class="sxs-lookup"><span data-stu-id="19b21-116">Application</span></span> | <span data-ttu-id="19b21-117">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19b21-117">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="19b21-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19b21-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="19b21-119">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="19b21-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="19b21-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19b21-120">Request headers</span></span>

| <span data-ttu-id="19b21-121">Nome</span><span class="sxs-lookup"><span data-stu-id="19b21-121">Name</span></span>       | <span data-ttu-id="19b21-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="19b21-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="19b21-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="19b21-123">Authorization</span></span>  | <span data-ttu-id="19b21-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19b21-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="19b21-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="19b21-126">Content-Type</span></span>  | <span data-ttu-id="19b21-127">application/json</span><span class="sxs-lookup"><span data-stu-id="19b21-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="19b21-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19b21-128">Request body</span></span>

<span data-ttu-id="19b21-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="19b21-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19b21-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="19b21-130">Response</span></span>

<span data-ttu-id="19b21-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna um corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="19b21-p103">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="19b21-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="19b21-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="19b21-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19b21-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="19b21-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="19b21-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/beta/domains/contoso.com
```
# <a name="c"></a>[<span data-ttu-id="19b21-136">C#</span><span class="sxs-lookup"><span data-stu-id="19b21-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="19b21-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19b21-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="19b21-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19b21-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="19b21-139">Java</span><span class="sxs-lookup"><span data-stu-id="19b21-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-domain-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="19b21-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="19b21-140">Response</span></span>

<span data-ttu-id="19b21-141">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="19b21-141">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


