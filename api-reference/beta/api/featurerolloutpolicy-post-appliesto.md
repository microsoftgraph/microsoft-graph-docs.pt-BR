---
title: Atribuir appliesTo
description: Atribua um directoryObject à atribuição de recursos.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a9eebb3ad1903d92071968149624ac4a2973886f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042286"
---
# <a name="assign-appliesto"></a><span data-ttu-id="154e0-103">Atribuir appliesTo</span><span class="sxs-lookup"><span data-stu-id="154e0-103">Assign appliesTo</span></span>

<span data-ttu-id="154e0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="154e0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="154e0-105">Adicione um appliesTo em um [objeto featureRolloutPolicy](../resources/featurerolloutpolicy.md) para especificar [o directoryObject](../resources/directoryobject.md) ao qual [o featureRolloutPolicy](../resources/featurerolloutpolicy.md) deve ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="154e0-105">Add an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to specify the [directoryObject](../resources/directoryobject.md) to which the [featureRolloutPolicy](../resources/featurerolloutpolicy.md) should be applied.</span></span>

## <a name="permissions"></a><span data-ttu-id="154e0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="154e0-106">Permissions</span></span>

<span data-ttu-id="154e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="154e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="154e0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="154e0-109">Permission type</span></span>                        | <span data-ttu-id="154e0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="154e0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="154e0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="154e0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="154e0-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="154e0-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="154e0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="154e0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="154e0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="154e0-114">Not supported.</span></span> |
| <span data-ttu-id="154e0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="154e0-115">Application</span></span>                            | <span data-ttu-id="154e0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="154e0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="154e0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="154e0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /policies/featureRolloutPolicies/{id}/appliesTo/$ref
```

## <a name="request-headers"></a><span data-ttu-id="154e0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="154e0-118">Request headers</span></span>

| <span data-ttu-id="154e0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="154e0-119">Name</span></span>          | <span data-ttu-id="154e0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="154e0-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="154e0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="154e0-121">Authorization</span></span> | <span data-ttu-id="154e0-122">Portador {token}.</span><span class="sxs-lookup"><span data-stu-id="154e0-122">Bearer {token}.</span></span> <span data-ttu-id="154e0-123">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="154e0-123">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="154e0-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="154e0-124">Request body</span></span>

<span data-ttu-id="154e0-125">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryobject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="154e0-125">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="154e0-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="154e0-126">Response</span></span>

<span data-ttu-id="154e0-127">Se tiver êxito, este método retornará um código `201 Created` de resposta e um novo objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="154e0-127">If successful, this method returns a `201 Created` response code and a new [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="154e0-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="154e0-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="154e0-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="154e0-129">Request</span></span>

<span data-ttu-id="154e0-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="154e0-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="154e0-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="154e0-131">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="154e0-132">C#</span><span class="sxs-lookup"><span data-stu-id="154e0-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-featurerolloutpolicy-policies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="154e0-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="154e0-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-featurerolloutpolicy-policies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="154e0-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="154e0-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-featurerolloutpolicy-policies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="154e0-135">Java</span><span class="sxs-lookup"><span data-stu-id="154e0-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-featurerolloutpolicy-policies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="154e0-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="154e0-136">Response</span></span>

<span data-ttu-id="154e0-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="154e0-137">The following is an example of the response.</span></span>

> <span data-ttu-id="154e0-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="154e0-138">**Note:** The response object shown here might be shortened for readability.</span></span>

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


