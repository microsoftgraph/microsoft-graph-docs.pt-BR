---
title: Remover tokenLifetimePolicy
description: Remover um tokenLifetimePolicy de um aplicativo.
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 7e9783001ae0dae7204b2cc4f01c19d03b063a34
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137316"
---
# <a name="remove-tokenlifetimepolicy"></a><span data-ttu-id="b806e-103">Remover tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="b806e-103">Remove tokenLifetimePolicy</span></span>

<span data-ttu-id="b806e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b806e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b806e-105">Remover um [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) de um [aplicativo.](../resources/application.md)</span><span class="sxs-lookup"><span data-stu-id="b806e-105">Remove a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b806e-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="b806e-106">Permissions</span></span>

<span data-ttu-id="b806e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b806e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b806e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b806e-109">Permission type</span></span>                        | <span data-ttu-id="b806e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b806e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b806e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b806e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b806e-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b806e-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="b806e-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b806e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b806e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b806e-114">Not supported.</span></span> |
| <span data-ttu-id="b806e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b806e-115">Application</span></span>                            | <span data-ttu-id="b806e-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b806e-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b806e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b806e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/tokenLifetimePolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="b806e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b806e-118">Request headers</span></span>

| <span data-ttu-id="b806e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b806e-119">Name</span></span>          | <span data-ttu-id="b806e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b806e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b806e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b806e-121">Authorization</span></span> | <span data-ttu-id="b806e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b806e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b806e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b806e-124">Request body</span></span>

<span data-ttu-id="b806e-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b806e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b806e-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="b806e-126">Response</span></span>

<span data-ttu-id="b806e-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b806e-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b806e-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b806e-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b806e-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b806e-129">Request</span></span>

<span data-ttu-id="b806e-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b806e-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b806e-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="b806e-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tokenlifetimepolicy_from_application"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}/tokenLifetimePolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="b806e-132">C#</span><span class="sxs-lookup"><span data-stu-id="b806e-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tokenlifetimepolicy-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b806e-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b806e-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tokenlifetimepolicy-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b806e-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b806e-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tokenlifetimepolicy-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b806e-135">Java</span><span class="sxs-lookup"><span data-stu-id="b806e-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-tokenlifetimepolicy-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b806e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b806e-136">Response</span></span>

<span data-ttu-id="b806e-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b806e-137">The following is an example of the response.</span></span>

> <span data-ttu-id="b806e-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b806e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

