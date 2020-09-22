---
title: Remover tokenIssuancePolicy
description: Remover um tokenIssuancePolicy de um aplicativo.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bb1999c23f16802f71ff7f823b31d352068c1b8f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996966"
---
# <a name="remove-tokenissuancepolicy"></a><span data-ttu-id="ea79a-103">Remover tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="ea79a-103">Remove tokenIssuancePolicy</span></span>

<span data-ttu-id="ea79a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea79a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea79a-105">Remover um [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) de um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="ea79a-105">Remove a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ea79a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ea79a-106">Permissions</span></span>

<span data-ttu-id="ea79a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea79a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ea79a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ea79a-109">Permission type</span></span>                        | <span data-ttu-id="ea79a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ea79a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ea79a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ea79a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ea79a-112">Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ea79a-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="ea79a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ea79a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea79a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea79a-114">Not supported.</span></span> |
| <span data-ttu-id="ea79a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ea79a-115">Application</span></span>                            | <span data-ttu-id="ea79a-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. OwnedBy, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ea79a-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea79a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ea79a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/tokenIssuancePolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="ea79a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ea79a-118">Request headers</span></span>

| <span data-ttu-id="ea79a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ea79a-119">Name</span></span>          | <span data-ttu-id="ea79a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea79a-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ea79a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ea79a-121">Authorization</span></span> | <span data-ttu-id="ea79a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea79a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea79a-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ea79a-124">Request body</span></span>

<span data-ttu-id="ea79a-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ea79a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea79a-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea79a-126">Response</span></span>

<span data-ttu-id="ea79a-127">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ea79a-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ea79a-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ea79a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ea79a-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ea79a-129">Request</span></span>

<span data-ttu-id="ea79a-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ea79a-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ea79a-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea79a-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tokenissuancepolicy_from_application"
}-->

```http
DELETE https://graph.microsoft.com/beta/applications/{id}/tokenIssuancePolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="ea79a-132">C#</span><span class="sxs-lookup"><span data-stu-id="ea79a-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tokenissuancepolicy-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ea79a-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea79a-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tokenissuancepolicy-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ea79a-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea79a-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tokenissuancepolicy-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ea79a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea79a-135">Response</span></span>

<span data-ttu-id="ea79a-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ea79a-136">The following is an example of the response.</span></span>

> <span data-ttu-id="ea79a-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ea79a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


