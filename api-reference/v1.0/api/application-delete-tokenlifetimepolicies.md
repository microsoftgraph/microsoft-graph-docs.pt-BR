---
title: Remover tokenLifetimePolicy
description: Remova um tokenLifetimePolicy de um aplicativo.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 3840de12c08d35629c3d383d3056104d757ce236
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054186"
---
# <a name="remove-tokenlifetimepolicy"></a><span data-ttu-id="52869-103">Remover tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="52869-103">Remove tokenLifetimePolicy</span></span>

<span data-ttu-id="52869-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52869-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="52869-105">Remover um [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) de um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="52869-105">Remove a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="52869-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="52869-106">Permissions</span></span>

<span data-ttu-id="52869-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52869-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="52869-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52869-109">Permission type</span></span>                        | <span data-ttu-id="52869-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52869-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="52869-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52869-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="52869-112">Policy.Read.All e Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration e Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52869-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="52869-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52869-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52869-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52869-114">Not supported.</span></span> |
| <span data-ttu-id="52869-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52869-115">Application</span></span>                            | <span data-ttu-id="52869-116">Policy.Read.All e Application.ReadWrite.OwnedBy, Policy.Read.All e Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration e Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration e Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52869-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="52869-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52869-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/tokenLifetimePolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="52869-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52869-118">Request headers</span></span>

| <span data-ttu-id="52869-119">Nome</span><span class="sxs-lookup"><span data-stu-id="52869-119">Name</span></span>          | <span data-ttu-id="52869-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="52869-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="52869-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="52869-121">Authorization</span></span> | <span data-ttu-id="52869-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52869-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="52869-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52869-124">Request body</span></span>

<span data-ttu-id="52869-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="52869-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52869-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="52869-126">Response</span></span>

<span data-ttu-id="52869-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="52869-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="52869-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="52869-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="52869-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52869-129">Request</span></span>

<span data-ttu-id="52869-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="52869-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="52869-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="52869-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tokenlifetimepolicy_from_application"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}/tokenLifetimePolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="52869-132">C#</span><span class="sxs-lookup"><span data-stu-id="52869-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tokenlifetimepolicy-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="52869-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52869-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tokenlifetimepolicy-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="52869-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52869-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tokenlifetimepolicy-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="52869-135">Java</span><span class="sxs-lookup"><span data-stu-id="52869-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-tokenlifetimepolicy-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="52869-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="52869-136">Response</span></span>

<span data-ttu-id="52869-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="52869-137">The following is an example of the response.</span></span>

> <span data-ttu-id="52869-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="52869-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

