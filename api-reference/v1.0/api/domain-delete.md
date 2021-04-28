---
title: Excluir domínio
description: Exclui um domínio de um locatário.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 0ecaf2cd5c1f8f0ed0281be585a85008e6870a8f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050504"
---
# <a name="delete-domain"></a><span data-ttu-id="43761-103">Excluir domínio</span><span class="sxs-lookup"><span data-stu-id="43761-103">Delete domain</span></span>

<span data-ttu-id="43761-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43761-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="43761-105">Exclui um domínio de um locatário.</span><span class="sxs-lookup"><span data-stu-id="43761-105">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="43761-106">**Importante:**</span><span class="sxs-lookup"><span data-stu-id="43761-106">**Important:**</span></span>
> - <span data-ttu-id="43761-107">Os domínios excluídos não podem ser recuperados.</span><span class="sxs-lookup"><span data-stu-id="43761-107">Deleted domains are not recoverable.</span></span><br />
> - <span data-ttu-id="43761-p101">As tentativas de exclusão falharão se houver objetos ou recursos dependentes no domínio. Você pode encontrar todos os recursos dependentes usando a API [Listar domainNameReferences](domain-list-domainnamereferences.md).</span><span class="sxs-lookup"><span data-stu-id="43761-p101">Attempts to delete will fail if there are any resources or objects still dependent on the domain. You can find all dependent resources by using the [List domainNameReferences](domain-list-domainnamereferences.md) API.</span></span>

## <a name="permissions"></a><span data-ttu-id="43761-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="43761-110">Permissions</span></span>

<span data-ttu-id="43761-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43761-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="43761-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43761-113">Permission type</span></span>      | <span data-ttu-id="43761-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="43761-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43761-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43761-115">Delegated (work or school account)</span></span> | <span data-ttu-id="43761-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="43761-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="43761-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43761-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43761-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43761-118">Not supported.</span></span>    |
|<span data-ttu-id="43761-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43761-119">Application</span></span> | <span data-ttu-id="43761-120">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43761-120">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="43761-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43761-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="43761-122">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="43761-122">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="43761-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43761-123">Request headers</span></span>

| <span data-ttu-id="43761-124">Nome</span><span class="sxs-lookup"><span data-stu-id="43761-124">Name</span></span>       | <span data-ttu-id="43761-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="43761-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="43761-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="43761-126">Authorization</span></span>  | <span data-ttu-id="43761-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43761-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="43761-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="43761-129">Content-Type</span></span>  | <span data-ttu-id="43761-130">application/json</span><span class="sxs-lookup"><span data-stu-id="43761-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="43761-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43761-131">Request body</span></span>

<span data-ttu-id="43761-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="43761-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43761-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="43761-133">Response</span></span>

<span data-ttu-id="43761-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna um corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="43761-p104">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="43761-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="43761-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="43761-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43761-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="43761-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="43761-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/domains/contoso.com
```
# <a name="c"></a>[<span data-ttu-id="43761-139">C#</span><span class="sxs-lookup"><span data-stu-id="43761-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="43761-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="43761-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="43761-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="43761-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="43761-142">Java</span><span class="sxs-lookup"><span data-stu-id="43761-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-domain-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="43761-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="43761-143">Response</span></span>

<span data-ttu-id="43761-144">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="43761-144">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

