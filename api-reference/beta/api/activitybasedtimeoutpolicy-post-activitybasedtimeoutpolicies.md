---
title: Criar activityBasedTimeoutPolicy
description: Criar um novo activityBasedTimeoutPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: da819249d9ae4ea59eee913af9bed1f6fef4f879
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234059"
---
# <a name="create-activitybasedtimeoutpolicy"></a><span data-ttu-id="480f5-103">Criar activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="480f5-103">Create activityBasedTimeoutPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="480f5-104">Criar um novo objeto [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="480f5-104">Create a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="480f5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="480f5-105">Permissions</span></span>

<span data-ttu-id="480f5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="480f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="480f5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="480f5-108">Permission type</span></span>                        | <span data-ttu-id="480f5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="480f5-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="480f5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="480f5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="480f5-111">Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="480f5-111">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="480f5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="480f5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="480f5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="480f5-113">Not supported.</span></span> |
| <span data-ttu-id="480f5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="480f5-114">Application</span></span>                            | <span data-ttu-id="480f5-115">Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="480f5-115">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="480f5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="480f5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/activityBasedTimeoutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="480f5-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="480f5-117">Request headers</span></span>

| <span data-ttu-id="480f5-118">Nome</span><span class="sxs-lookup"><span data-stu-id="480f5-118">Name</span></span>          | <span data-ttu-id="480f5-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="480f5-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="480f5-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="480f5-120">Authorization</span></span> | <span data-ttu-id="480f5-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="480f5-121">Bearer {token}</span></span> |
| <span data-ttu-id="480f5-122">Content-type</span><span class="sxs-lookup"><span data-stu-id="480f5-122">Content-type</span></span> | <span data-ttu-id="480f5-123">application/json</span><span class="sxs-lookup"><span data-stu-id="480f5-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="480f5-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="480f5-124">Request body</span></span>

<span data-ttu-id="480f5-125">No corpo da solicitação, forneça uma representação JSON do objeto [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="480f5-125">In the request body, supply a JSON representation of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="480f5-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="480f5-126">Response</span></span>

<span data-ttu-id="480f5-127">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="480f5-127">If successful, this method returns a `201 Created` response code and a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="480f5-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="480f5-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="480f5-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="480f5-129">Request</span></span>

<span data-ttu-id="480f5-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="480f5-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_activitybasedtimeoutpolicy_from_activitybasedtimeoutpolicies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/activityBasedTimeoutPolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```

### <a name="response"></a><span data-ttu-id="480f5-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="480f5-131">Response</span></span>

<span data-ttu-id="480f5-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="480f5-132">The following is an example of the response.</span></span>

> <span data-ttu-id="480f5-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="480f5-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create activityBasedTimeoutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->