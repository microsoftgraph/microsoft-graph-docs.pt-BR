---
title: Atribuir appliesTo
description: Atribua um directoryObject à atribuição de recursos.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: f845aac0abd8fd8d6f23151ffd4fc99e8b6bdcf3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959295"
---
# <a name="assign-appliesto"></a><span data-ttu-id="cb439-103">Atribuir appliesTo</span><span class="sxs-lookup"><span data-stu-id="cb439-103">Assign appliesTo</span></span>

<span data-ttu-id="cb439-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb439-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb439-105">Adicione um appliesTo em um [objeto featureRolloutPolicy](../resources/featurerolloutpolicy.md) para especificar [o directoryObject](../resources/directoryobject.md) ao qual [o featureRolloutPolicy](../resources/featurerolloutpolicy.md) deve ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="cb439-105">Add an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to specify the [directoryObject](../resources/directoryobject.md) to which the [featureRolloutPolicy](../resources/featurerolloutpolicy.md) should be applied.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb439-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cb439-106">Permissions</span></span>

<span data-ttu-id="cb439-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb439-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cb439-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb439-109">Permission type</span></span>                        | <span data-ttu-id="cb439-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cb439-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cb439-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb439-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb439-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb439-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="cb439-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb439-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb439-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb439-114">Not supported.</span></span> |
| <span data-ttu-id="cb439-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cb439-115">Application</span></span>                            | <span data-ttu-id="cb439-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb439-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb439-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb439-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /policies/featureRolloutPolicies/{id}/appliesTo/$ref
```

## <a name="request-headers"></a><span data-ttu-id="cb439-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb439-118">Request headers</span></span>

| <span data-ttu-id="cb439-119">Nome</span><span class="sxs-lookup"><span data-stu-id="cb439-119">Name</span></span>          | <span data-ttu-id="cb439-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb439-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cb439-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb439-121">Authorization</span></span> | <span data-ttu-id="cb439-122">Portador {token}.</span><span class="sxs-lookup"><span data-stu-id="cb439-122">Bearer {token}.</span></span> <span data-ttu-id="cb439-123">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="cb439-123">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb439-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb439-124">Request body</span></span>

<span data-ttu-id="cb439-125">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryobject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="cb439-125">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cb439-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb439-126">Response</span></span>

<span data-ttu-id="cb439-127">Se tiver êxito, este método retornará um código `201 Created` de resposta e um novo objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb439-127">If successful, this method returns a `201 Created` response code and a new [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cb439-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cb439-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cb439-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb439-129">Request</span></span>

<span data-ttu-id="cb439-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb439-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_featurerolloutpolicy_policies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/featureRolloutPolicies/{id}/appliesTo/$ref
Content-type: application/json

{
  "@odata.id": " https://graph.microsoft.com/beta/directoryObjects/2441b489-4f12-4882-b039-8f6006bd66da"
}
```

### <a name="response"></a><span data-ttu-id="cb439-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb439-131">Response</span></span>

<span data-ttu-id="cb439-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cb439-132">The following is an example of the response.</span></span>

> <span data-ttu-id="cb439-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cb439-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "directoryObject": {
    "id": "2441b489-4f12-4882-b039-8f6006bd66da",
    "objectType": "group"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Assign appliesTo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


