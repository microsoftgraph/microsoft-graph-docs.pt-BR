---
title: Remover tokenLifetimePolicy
description: Remover um tokenLifetimePolicy de um aplicativo ou servicePrincipalName.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ac5ed1f9fa221447d1363a7511019bb7c6bfc95e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996959"
---
# <a name="remove-tokenlifetimepolicy"></a><span data-ttu-id="ab7aa-103">Remover tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="ab7aa-103">Remove tokenLifetimePolicy</span></span>

<span data-ttu-id="ab7aa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab7aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab7aa-105">Remover um [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) de um [aplicativo](../resources/application.md) ou [servicePrincipalName](../resources/servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="ab7aa-105">Remove a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) from an [application](../resources/application.md) or [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ab7aa-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ab7aa-106">Permissions</span></span>

<span data-ttu-id="ab7aa-107">Um dos seguintes conjuntos de permissões é necessário para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="ab7aa-107">One of the following sets of permissions is required to call this API.</span></span> <span data-ttu-id="ab7aa-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab7aa-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ab7aa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab7aa-109">Permission type</span></span>                        | <span data-ttu-id="ab7aa-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab7aa-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ab7aa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab7aa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ab7aa-112">Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ab7aa-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="ab7aa-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab7aa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab7aa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab7aa-114">Not supported.</span></span> |
| <span data-ttu-id="ab7aa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab7aa-115">Application</span></span>                            | <span data-ttu-id="ab7aa-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. OwnedBy, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ab7aa-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab7aa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab7aa-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/tokenLifetimePolicies/{id}/$ref
DELETE /servicePrincipals/{id}/tokenLifetimePolicies/{id}$ref
```

## <a name="request-headers"></a><span data-ttu-id="ab7aa-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab7aa-118">Request headers</span></span>

| <span data-ttu-id="ab7aa-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ab7aa-119">Name</span></span>          | <span data-ttu-id="ab7aa-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab7aa-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ab7aa-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab7aa-121">Authorization</span></span> | <span data-ttu-id="ab7aa-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="ab7aa-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab7aa-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab7aa-123">Request body</span></span>

<span data-ttu-id="ab7aa-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ab7aa-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab7aa-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab7aa-125">Response</span></span>

<span data-ttu-id="ab7aa-126">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ab7aa-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ab7aa-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ab7aa-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ab7aa-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab7aa-128">Request</span></span>

<span data-ttu-id="ab7aa-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab7aa-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ab7aa-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab7aa-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tokenlifetimepolicy_from_application"
}-->

```http
DELETE https://graph.microsoft.com/beta/applications/{id}/tokenLifetimePolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="ab7aa-131">C#</span><span class="sxs-lookup"><span data-stu-id="ab7aa-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tokenlifetimepolicy-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ab7aa-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab7aa-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tokenlifetimepolicy-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ab7aa-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ab7aa-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tokenlifetimepolicy-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ab7aa-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab7aa-134">Response</span></span>

<span data-ttu-id="ab7aa-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ab7aa-135">The following is an example of the response.</span></span>

> <span data-ttu-id="ab7aa-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ab7aa-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


