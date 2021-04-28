---
title: Obter accessReviewPolicy
description: Leia as propriedades e as relações de um objeto accessReviewPolicy.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 05b6cbae21ea3a40b179d646feaeb9ff243f0a81
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067783"
---
# <a name="get-accessreviewpolicy"></a><span data-ttu-id="16142-103">Obter accessReviewPolicy</span><span class="sxs-lookup"><span data-stu-id="16142-103">Get accessReviewPolicy</span></span>
<span data-ttu-id="16142-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16142-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16142-105">Leia as propriedades e as relações de um [objeto accessReviewPolicy.](../resources/accessreviewpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="16142-105">Read the properties and relationships of an [accessReviewPolicy](../resources/accessreviewpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="16142-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="16142-106">Permissions</span></span>
<span data-ttu-id="16142-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16142-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16142-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16142-109">Permission type</span></span>|<span data-ttu-id="16142-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="16142-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16142-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16142-111">Delegated (work or school account)</span></span>|<span data-ttu-id="16142-112">Policy.Read.All, Policy.ReadWrite.AccessReviews</span><span class="sxs-lookup"><span data-stu-id="16142-112">Policy.Read.All, Policy.ReadWrite.AccessReviews</span></span>|
|<span data-ttu-id="16142-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16142-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16142-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16142-114">Not supported.</span></span>|
|<span data-ttu-id="16142-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16142-115">Application</span></span>|<span data-ttu-id="16142-116">Policy.Read.All, Policy.ReadWrite.AccessReviews</span><span class="sxs-lookup"><span data-stu-id="16142-116">Policy.Read.All, Policy.ReadWrite.AccessReviews</span></span>|

## <a name="http-request"></a><span data-ttu-id="16142-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16142-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/accessReviewPolicy
GET /identityGovernance/accessReviews/policy
```

## <a name="request-headers"></a><span data-ttu-id="16142-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16142-118">Request headers</span></span>
|<span data-ttu-id="16142-119">Nome</span><span class="sxs-lookup"><span data-stu-id="16142-119">Name</span></span>|<span data-ttu-id="16142-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="16142-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="16142-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="16142-121">Authorization</span></span>|<span data-ttu-id="16142-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16142-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="16142-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16142-124">Request body</span></span>
<span data-ttu-id="16142-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="16142-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16142-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="16142-126">Response</span></span>

<span data-ttu-id="16142-127">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto accessReviewPolicy](../resources/accessreviewpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16142-127">If successful, this method returns a `200 OK` response code and an [accessReviewPolicy](../resources/accessreviewpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="16142-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="16142-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="16142-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16142-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accessreviewpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/accessReviewPolicy
```


### <a name="response"></a><span data-ttu-id="16142-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="16142-130">Response</span></span>
<span data-ttu-id="16142-131">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="16142-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.accessReviewPolicy",
    "displayName": "Access Review Policy",
    "description": "Policy contains directory-level access review settings.",
    "isGroupOwnerManagementEnabled": false
  }
}
```

### <a name="request"></a><span data-ttu-id="16142-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16142-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accessreviewpolicy_2"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/policy
```


### <a name="response"></a><span data-ttu-id="16142-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="16142-133">Response</span></span>
<span data-ttu-id="16142-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="16142-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.accessReviewPolicy",
    "displayName": "Access Review Policy",
    "description": "Policy contains directory-level access review settings.",
    "isGroupOwnerManagementEnabled": false
  }
}
```
