---
title: Atribuir aplica-se
description: Atribua um directoryobject à distribuição de recursos.
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d2718ade42805913af1e648c99e5799bb84a80f3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48006717"
---
# <a name="assign-appliesto"></a><span data-ttu-id="4b06d-103">Atribuir aplica-se</span><span class="sxs-lookup"><span data-stu-id="4b06d-103">Assign appliesTo</span></span>

<span data-ttu-id="4b06d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b06d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b06d-105">Adicione um aplica-se a um objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) para especificar o [directoryobject](../resources/directoryobject.md) ao qual o [featureRolloutPolicy](../resources/featurerolloutpolicy.md) deve ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="4b06d-105">Add an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to specify the [directoryObject](../resources/directoryobject.md) to which the [featureRolloutPolicy](../resources/featurerolloutpolicy.md) should be applied to.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b06d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4b06d-106">Permissions</span></span>

<span data-ttu-id="4b06d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b06d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4b06d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b06d-109">Permission type</span></span>                        | <span data-ttu-id="4b06d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4b06d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4b06d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b06d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4b06d-112">Policy.ReadWrite.FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="4b06d-112">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="4b06d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b06d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b06d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b06d-114">Not supported.</span></span> |
| <span data-ttu-id="4b06d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b06d-115">Application</span></span>                            | <span data-ttu-id="4b06d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b06d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b06d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b06d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directory/featureRolloutPolicies/{id}/appliesTo/$ref
```

## <a name="request-headers"></a><span data-ttu-id="4b06d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b06d-118">Request headers</span></span>

| <span data-ttu-id="4b06d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4b06d-119">Name</span></span>          | <span data-ttu-id="4b06d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b06d-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4b06d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b06d-121">Authorization</span></span> | <span data-ttu-id="4b06d-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="4b06d-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b06d-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b06d-123">Request body</span></span>

<span data-ttu-id="4b06d-124">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryobject](../resources/directoryobject.md) .</span><span class="sxs-lookup"><span data-stu-id="4b06d-124">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4b06d-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b06d-125">Response</span></span>

<span data-ttu-id="4b06d-126">Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [directoryobject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b06d-126">If successful, this method returns a `201 Created` response code and a new [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4b06d-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4b06d-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4b06d-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b06d-128">Request</span></span>

<span data-ttu-id="4b06d-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b06d-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4b06d-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b06d-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_featurerolloutpolicy"
}-->

```http
POST https://graph.microsoft.com/beta/directory/featureRolloutPolicies/{id}/appliesTo/$ref
Content-type: application/json

{
  "@odata.id": " https://graph.microsoft.com/beta/directoryObjects/2441b489-4f12-4882-b039-8f6006bd66da"
}
```
# <a name="c"></a>[<span data-ttu-id="4b06d-131">C#</span><span class="sxs-lookup"><span data-stu-id="4b06d-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b06d-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b06d-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b06d-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b06d-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4b06d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b06d-134">Response</span></span>

<span data-ttu-id="4b06d-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4b06d-135">The following is an example of the response.</span></span>

> <span data-ttu-id="4b06d-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4b06d-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


