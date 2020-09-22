---
title: Remover tokenIssuancePolicy
description: Remover um tokenIssuancePolicy de um aplicativo.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4db42eb738a29660ed7e8779ef94e48f6b736365
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992801"
---
# <a name="remove-tokenissuancepolicy"></a><span data-ttu-id="988e2-103">Remover tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="988e2-103">Remove tokenIssuancePolicy</span></span>

<span data-ttu-id="988e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="988e2-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="988e2-105">Remover um [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) de um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="988e2-105">Remove a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="988e2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="988e2-106">Permissions</span></span>

<span data-ttu-id="988e2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="988e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="988e2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="988e2-109">Permission type</span></span>                        | <span data-ttu-id="988e2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="988e2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="988e2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="988e2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="988e2-112">Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="988e2-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="988e2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="988e2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="988e2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="988e2-114">Not supported.</span></span> |
| <span data-ttu-id="988e2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="988e2-115">Application</span></span>                            | <span data-ttu-id="988e2-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. OwnedBy, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="988e2-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="988e2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="988e2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/tokenIssuancePolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="988e2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="988e2-118">Request headers</span></span>

| <span data-ttu-id="988e2-119">Nome</span><span class="sxs-lookup"><span data-stu-id="988e2-119">Name</span></span>          | <span data-ttu-id="988e2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="988e2-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="988e2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="988e2-121">Authorization</span></span> | <span data-ttu-id="988e2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="988e2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="988e2-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="988e2-124">Request body</span></span>

<span data-ttu-id="988e2-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="988e2-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="988e2-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="988e2-126">Response</span></span>

<span data-ttu-id="988e2-127">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="988e2-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="988e2-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="988e2-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="988e2-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="988e2-129">Request</span></span>

<span data-ttu-id="988e2-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="988e2-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="988e2-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="988e2-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tokenissuancepolicy_from_application"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}/tokenIssuancePolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="988e2-132">C#</span><span class="sxs-lookup"><span data-stu-id="988e2-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tokenissuancepolicy-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="988e2-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="988e2-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tokenissuancepolicy-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="988e2-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="988e2-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tokenissuancepolicy-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="988e2-135">Java</span><span class="sxs-lookup"><span data-stu-id="988e2-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-tokenissuancepolicy-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="988e2-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="988e2-136">Response</span></span>

<span data-ttu-id="988e2-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="988e2-137">The following is an example of the response.</span></span>

> <span data-ttu-id="988e2-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="988e2-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Remove tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

