---
title: Excluir tokenIssuancePolicy
description: Exclua tokenIssuancePolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ed3f02e1ff6cb566922282548e0b9fb252f6784b
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229693"
---
# <a name="delete-tokenissuancepolicy"></a><span data-ttu-id="03060-103">Excluir tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="03060-103">Delete tokenIssuancePolicy</span></span>

<span data-ttu-id="03060-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03060-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="03060-105">Excluir um objeto [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="03060-105">Delete a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="03060-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="03060-106">Permissions</span></span>

<span data-ttu-id="03060-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03060-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="03060-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03060-109">Permission type</span></span>                        | <span data-ttu-id="03060-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="03060-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="03060-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03060-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="03060-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="03060-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="03060-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03060-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03060-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03060-114">Not supported.</span></span> |
| <span data-ttu-id="03060-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03060-115">Application</span></span>                            | <span data-ttu-id="03060-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="03060-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="03060-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03060-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/tokenIssuancePolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="03060-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03060-118">Request headers</span></span>

| <span data-ttu-id="03060-119">Nome</span><span class="sxs-lookup"><span data-stu-id="03060-119">Name</span></span>          | <span data-ttu-id="03060-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="03060-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="03060-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="03060-121">Authorization</span></span> | <span data-ttu-id="03060-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03060-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="03060-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03060-124">Request body</span></span>

<span data-ttu-id="03060-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="03060-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03060-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="03060-126">Response</span></span>

<span data-ttu-id="03060-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="03060-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="03060-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="03060-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="03060-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03060-129">Request</span></span>

<span data-ttu-id="03060-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="03060-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_tokenissuancepolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/tokenIssuancePolicies/{id}
```

### <a name="response"></a><span data-ttu-id="03060-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="03060-131">Response</span></span>

<span data-ttu-id="03060-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="03060-132">The following is an example of the response.</span></span>

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
  "description": "Delete tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
