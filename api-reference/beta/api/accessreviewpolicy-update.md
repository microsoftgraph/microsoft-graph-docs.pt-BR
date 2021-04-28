---
title: Atualizar accessReviewPolicy
description: Atualize as propriedades de um objeto accessReviewPolicy.
author: kafen
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 3a4ef900a4dfc88b28dfd3d11f96804655160823
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067279"
---
# <a name="update-accessreviewpolicy"></a><span data-ttu-id="4c2e1-103">Atualizar accessReviewPolicy</span><span class="sxs-lookup"><span data-stu-id="4c2e1-103">Update accessReviewPolicy</span></span>
<span data-ttu-id="4c2e1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c2e1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c2e1-105">Atualize as propriedades de [um objeto accessReviewPolicy.](../resources/accessreviewpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4c2e1-105">Update the properties of an [accessReviewPolicy](../resources/accessreviewpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c2e1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4c2e1-106">Permissions</span></span>
<span data-ttu-id="4c2e1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c2e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c2e1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c2e1-109">Permission type</span></span>|<span data-ttu-id="4c2e1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4c2e1-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c2e1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c2e1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4c2e1-112">Policy.ReadWrite.AccessReviews</span><span class="sxs-lookup"><span data-stu-id="4c2e1-112">Policy.ReadWrite.AccessReviews</span></span>|
|<span data-ttu-id="4c2e1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c2e1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c2e1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c2e1-114">Not supported.</span></span>|
|<span data-ttu-id="4c2e1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c2e1-115">Application</span></span>|<span data-ttu-id="4c2e1-116">Policy.ReadWrite.AccessReviews</span><span class="sxs-lookup"><span data-stu-id="4c2e1-116">Policy.ReadWrite.AccessReviews</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c2e1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c2e1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/accessReviewPolicy
PATCH /identityGovernance/accessReviews/policy
```

## <a name="request-headers"></a><span data-ttu-id="4c2e1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c2e1-118">Request headers</span></span>
|<span data-ttu-id="4c2e1-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4c2e1-119">Name</span></span>|<span data-ttu-id="4c2e1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c2e1-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4c2e1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c2e1-121">Authorization</span></span>|<span data-ttu-id="4c2e1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c2e1-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4c2e1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4c2e1-124">Content-Type</span></span>|<span data-ttu-id="4c2e1-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c2e1-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c2e1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c2e1-127">Request body</span></span>
<span data-ttu-id="4c2e1-128">No corpo da solicitação, fornece uma representação JSON do [objeto accessReviewPolicy.](../resources/accessreviewpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4c2e1-128">In the request body, supply a JSON representation of the [accessReviewPolicy](../resources/accessreviewpolicy.md) object.</span></span>

<span data-ttu-id="4c2e1-129">A tabela a seguir mostra as propriedades que são necessárias ao atualizar [o accessReviewPolicy](../resources/accessreviewpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4c2e1-129">The following table shows the properties that are required when you update the [accessReviewPolicy](../resources/accessreviewpolicy.md).</span></span>

|<span data-ttu-id="4c2e1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4c2e1-130">Property</span></span>|<span data-ttu-id="4c2e1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c2e1-131">Type</span></span>|<span data-ttu-id="4c2e1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c2e1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c2e1-133">isGroupOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="4c2e1-133">isGroupOwnerManagementEnabled</span></span>|<span data-ttu-id="4c2e1-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c2e1-134">Boolean</span></span>|<span data-ttu-id="4c2e1-135">Se `true` , os proprietários do grupo podem criar e gerenciar avaliações de acesso nos grupos que eles próprios têm.</span><span class="sxs-lookup"><span data-stu-id="4c2e1-135">If `true`, group owners can create and manage access reviews on groups they own.</span></span>|



## <a name="response"></a><span data-ttu-id="4c2e1-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c2e1-136">Response</span></span>

<span data-ttu-id="4c2e1-137">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4c2e1-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4c2e1-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4c2e1-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4c2e1-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c2e1-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_accessreviewpolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/accessReviewPolicy
Content-Type: application/json

{
  "isGroupOwnerManagementEnabled": true
}
```

### <a name="response"></a><span data-ttu-id="4c2e1-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c2e1-140">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="request"></a><span data-ttu-id="4c2e1-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c2e1-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_accessreviewpolicy_2"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance/accessReviews/policy
Content-Type: application/json

{
  "isGroupOwnerManagementEnabled": true
}
```

### <a name="response"></a><span data-ttu-id="4c2e1-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c2e1-142">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
