---
title: Criar activityBasedTimeoutPolicy
description: Criar um novo activityBasedTimeoutPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b0c9227b363f4f3693fe56e057f66a51498b3fb5
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227767"
---
# <a name="create-activitybasedtimeoutpolicy"></a><span data-ttu-id="54e9a-103">Criar activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="54e9a-103">Create activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="54e9a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54e9a-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="54e9a-105">Criar um novo objeto [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="54e9a-105">Create a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="54e9a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="54e9a-106">Permissions</span></span>

<span data-ttu-id="54e9a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54e9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="54e9a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54e9a-109">Permission type</span></span>                        | <span data-ttu-id="54e9a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="54e9a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="54e9a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54e9a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="54e9a-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="54e9a-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="54e9a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54e9a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54e9a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54e9a-114">Not supported.</span></span> |
| <span data-ttu-id="54e9a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54e9a-115">Application</span></span>                            | <span data-ttu-id="54e9a-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="54e9a-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="54e9a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54e9a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/activityBasedTimeoutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="54e9a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54e9a-118">Request headers</span></span>

| <span data-ttu-id="54e9a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="54e9a-119">Name</span></span>          | <span data-ttu-id="54e9a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="54e9a-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="54e9a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="54e9a-121">Authorization</span></span> | <span data-ttu-id="54e9a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54e9a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="54e9a-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="54e9a-124">Content-type</span></span> | <span data-ttu-id="54e9a-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54e9a-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54e9a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54e9a-127">Request body</span></span>

<span data-ttu-id="54e9a-128">No corpo da solicitação, forneça uma representação JSON de um objeto [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="54e9a-128">In the request body, supply a JSON representation of an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="54e9a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="54e9a-129">Response</span></span>

<span data-ttu-id="54e9a-130">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54e9a-130">If successful, this method returns a `201 Created` response code and a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="54e9a-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="54e9a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="54e9a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54e9a-132">Request</span></span>

<span data-ttu-id="54e9a-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="54e9a-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_activitybasedtimeoutpolicy_from_activitybasedtimeoutpolicies"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/activityBasedTimeoutPolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```

### <a name="response"></a><span data-ttu-id="54e9a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="54e9a-134">Response</span></span>

<span data-ttu-id="54e9a-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="54e9a-135">The following is an example of the response.</span></span>

> <span data-ttu-id="54e9a-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="54e9a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
