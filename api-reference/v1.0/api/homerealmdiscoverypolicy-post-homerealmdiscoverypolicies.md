---
title: Criar homeRealmDiscoveryPolicy
description: Criar um novo homeRealmDiscoveryPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 34347b52eead2688b39db55a775e843af807dd6c
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227753"
---
# <a name="create-homerealmdiscoverypolicy"></a><span data-ttu-id="19c7b-103">Criar homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="19c7b-103">Create homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="19c7b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19c7b-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="19c7b-105">Criar um novo objeto [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="19c7b-105">Create a new [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="19c7b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="19c7b-106">Permissions</span></span>

<span data-ttu-id="19c7b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19c7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="19c7b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19c7b-109">Permission type</span></span>                        | <span data-ttu-id="19c7b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="19c7b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="19c7b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19c7b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="19c7b-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="19c7b-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="19c7b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19c7b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19c7b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19c7b-114">Not supported.</span></span> |
| <span data-ttu-id="19c7b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19c7b-115">Application</span></span>                            | <span data-ttu-id="19c7b-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="19c7b-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="19c7b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19c7b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/homeRealmDiscoveryPolicies
```

## <a name="request-headers"></a><span data-ttu-id="19c7b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19c7b-118">Request headers</span></span>

| <span data-ttu-id="19c7b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="19c7b-119">Name</span></span>          | <span data-ttu-id="19c7b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="19c7b-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="19c7b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="19c7b-121">Authorization</span></span> | <span data-ttu-id="19c7b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19c7b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="19c7b-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="19c7b-124">Content-type</span></span> | <span data-ttu-id="19c7b-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19c7b-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19c7b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19c7b-127">Request body</span></span>

<span data-ttu-id="19c7b-128">No corpo da solicitação, forneça uma representação JSON do objeto [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="19c7b-128">In the request body, supply a JSON representation of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="19c7b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="19c7b-129">Response</span></span>

<span data-ttu-id="19c7b-130">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19c7b-130">If successful, this method returns a `201 Created` response code and a new [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="19c7b-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="19c7b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="19c7b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19c7b-132">Request</span></span>

<span data-ttu-id="19c7b-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="19c7b-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_homerealmdiscoverypolicy_from_homerealmdiscoverypolicies"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```

### <a name="response"></a><span data-ttu-id="19c7b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="19c7b-134">Response</span></span>

<span data-ttu-id="19c7b-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="19c7b-135">The following is an example of the response.</span></span>

> <span data-ttu-id="19c7b-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19c7b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy"
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
  "description": "Create homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
