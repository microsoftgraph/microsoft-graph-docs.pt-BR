---
title: Excluir activityBasedTimeoutPolicy
description: Exclua activityBasedTimeoutPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8124030da30028e9c3ee9cef67541627e5888292
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227773"
---
# <a name="delete-activitybasedtimeoutpolicy"></a><span data-ttu-id="bd12f-103">Excluir activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="bd12f-103">Delete activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="bd12f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd12f-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="bd12f-105">Excluir um objeto [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="bd12f-105">Delete an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd12f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bd12f-106">Permissions</span></span>

<span data-ttu-id="bd12f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd12f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bd12f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd12f-109">Permission type</span></span>                        | <span data-ttu-id="bd12f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bd12f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bd12f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd12f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd12f-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="bd12f-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="bd12f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd12f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd12f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd12f-114">Not supported.</span></span> |
| <span data-ttu-id="bd12f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd12f-115">Application</span></span>                            | <span data-ttu-id="bd12f-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="bd12f-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd12f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd12f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/activityBasedTimeoutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bd12f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd12f-118">Request headers</span></span>

| <span data-ttu-id="bd12f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="bd12f-119">Name</span></span>          | <span data-ttu-id="bd12f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd12f-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bd12f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd12f-121">Authorization</span></span> | <span data-ttu-id="bd12f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd12f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd12f-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd12f-124">Request body</span></span>

<span data-ttu-id="bd12f-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bd12f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd12f-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd12f-126">Response</span></span>

<span data-ttu-id="bd12f-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bd12f-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="bd12f-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bd12f-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bd12f-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd12f-129">Request</span></span>

<span data-ttu-id="bd12f-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd12f-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_activitybasedtimeoutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/activityBasedTimeoutPolicies/{id}
```

### <a name="response"></a><span data-ttu-id="bd12f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd12f-131">Response</span></span>

<span data-ttu-id="bd12f-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bd12f-132">The following is an example of the response.</span></span>

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
  "description": "Delete activityBasedTimeoutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
