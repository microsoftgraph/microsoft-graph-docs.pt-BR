---
title: Excluir tokenLifetimePolicy
description: Exclua tokenLifetimePolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 06b6994af764462d91cd9ee818d5b590c0bc620d
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229651"
---
# <a name="delete-tokenlifetimepolicy"></a><span data-ttu-id="b3e93-103">Excluir tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="b3e93-103">Delete tokenLifetimePolicy</span></span>

<span data-ttu-id="b3e93-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3e93-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="b3e93-105">Excluir um objeto [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="b3e93-105">Delete a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3e93-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b3e93-106">Permissions</span></span>

<span data-ttu-id="b3e93-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3e93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b3e93-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3e93-109">Permission type</span></span>                        | <span data-ttu-id="b3e93-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b3e93-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b3e93-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3e93-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b3e93-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="b3e93-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="b3e93-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3e93-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3e93-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3e93-114">Not supported.</span></span> |
| <span data-ttu-id="b3e93-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3e93-115">Application</span></span>                            | <span data-ttu-id="b3e93-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="b3e93-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3e93-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3e93-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/tokenLifetimePolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b3e93-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3e93-118">Request headers</span></span>

| <span data-ttu-id="b3e93-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b3e93-119">Name</span></span>          | <span data-ttu-id="b3e93-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3e93-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b3e93-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3e93-121">Authorization</span></span> | <span data-ttu-id="b3e93-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3e93-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3e93-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3e93-124">Request body</span></span>

<span data-ttu-id="b3e93-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b3e93-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3e93-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3e93-126">Response</span></span>

<span data-ttu-id="b3e93-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b3e93-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b3e93-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b3e93-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b3e93-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3e93-129">Request</span></span>

<span data-ttu-id="b3e93-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3e93-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_tokenlifetimepolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies/{id}
```

### <a name="response"></a><span data-ttu-id="b3e93-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3e93-131">Response</span></span>

<span data-ttu-id="b3e93-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b3e93-132">The following is an example of the response.</span></span>

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
  "description": "Delete tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
