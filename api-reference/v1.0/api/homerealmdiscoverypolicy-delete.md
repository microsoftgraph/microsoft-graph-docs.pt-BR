---
title: Excluir homeRealmDiscoveryPolicy
description: Exclua homeRealmDiscoveryPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7d1fb3e5aa79a0b9dc056cf57b358628cce2a423
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227748"
---
# <a name="delete-homerealmdiscoverypolicy"></a><span data-ttu-id="69034-103">Excluir homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="69034-103">Delete homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="69034-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69034-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="69034-105">Excluir um objeto [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="69034-105">Delete a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="69034-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="69034-106">Permissions</span></span>

<span data-ttu-id="69034-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69034-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="69034-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="69034-109">Permission type</span></span>                        | <span data-ttu-id="69034-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="69034-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="69034-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="69034-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="69034-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="69034-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="69034-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="69034-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69034-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69034-114">Not supported.</span></span> |
| <span data-ttu-id="69034-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69034-115">Application</span></span>                            | <span data-ttu-id="69034-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="69034-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="69034-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69034-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/homeRealmDiscoveryPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="69034-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69034-118">Request headers</span></span>

| <span data-ttu-id="69034-119">Nome</span><span class="sxs-lookup"><span data-stu-id="69034-119">Name</span></span>          | <span data-ttu-id="69034-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="69034-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="69034-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="69034-121">Authorization</span></span> | <span data-ttu-id="69034-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69034-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="69034-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="69034-124">Request body</span></span>

<span data-ttu-id="69034-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="69034-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69034-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="69034-126">Response</span></span>

<span data-ttu-id="69034-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="69034-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="69034-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="69034-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="69034-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69034-129">Request</span></span>

<span data-ttu-id="69034-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="69034-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies/{id}
```

### <a name="response"></a><span data-ttu-id="69034-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="69034-131">Response</span></span>

<span data-ttu-id="69034-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="69034-132">The following is an example of the response.</span></span>

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
  "description": "Delete homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
