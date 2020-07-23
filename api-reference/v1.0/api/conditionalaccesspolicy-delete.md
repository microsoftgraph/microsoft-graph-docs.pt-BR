---
title: Excluir conditionalAccessPolicy
description: Excluir um conditionalAccessPolicy.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e1064f54368f4bf4be2f655579da3ed133059d53
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384399"
---
# <a name="delete-conditionalaccesspolicy"></a><span data-ttu-id="400a6-103">Excluir conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="400a6-103">Delete conditionalAccessPolicy</span></span>

<span data-ttu-id="400a6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="400a6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="400a6-105">Excluir um objeto [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="400a6-105">Delete a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="400a6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="400a6-106">Permissions</span></span>

<span data-ttu-id="400a6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="400a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="400a6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="400a6-109">Permission type</span></span>                        | <span data-ttu-id="400a6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="400a6-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
| <span data-ttu-id="400a6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="400a6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="400a6-112">Policy. Read. All e Policy. ReadWrite. ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="400a6-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="400a6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="400a6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="400a6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="400a6-114">Not supported.</span></span> |
| <span data-ttu-id="400a6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="400a6-115">Application</span></span>                            | <span data-ttu-id="400a6-116">Policy. Read. All e Policy. ReadWrite. ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="400a6-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="400a6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="400a6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/conditionalAccess/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="400a6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="400a6-118">Request headers</span></span>

| <span data-ttu-id="400a6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="400a6-119">Name</span></span>          | <span data-ttu-id="400a6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="400a6-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="400a6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="400a6-121">Authorization</span></span> | <span data-ttu-id="400a6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="400a6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="400a6-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="400a6-124">Request body</span></span>

<span data-ttu-id="400a6-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="400a6-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="400a6-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="400a6-126">Response</span></span>

<span data-ttu-id="400a6-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="400a6-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="400a6-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="400a6-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="400a6-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="400a6-130">Request</span></span>

<span data-ttu-id="400a6-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="400a6-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="400a6-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="400a6-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conditionalaccesspolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/identity/conditionalAccess/policies/{id}
```

---

### <a name="response"></a><span data-ttu-id="400a6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="400a6-133">Response</span></span>

<span data-ttu-id="400a6-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="400a6-134">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete conditionalAccessPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
