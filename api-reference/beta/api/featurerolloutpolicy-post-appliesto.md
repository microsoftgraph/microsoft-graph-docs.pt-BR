---
title: Atribuir aplica-se
description: Atribua um directoryobject à distribuição de recursos.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f8d81ce37ad64071ef4193a01ad96c0ab0a35314
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2019
ms.locfileid: "36172811"
---
# <a name="assign-appliesto"></a><span data-ttu-id="22985-103">Atribuir aplica-se</span><span class="sxs-lookup"><span data-stu-id="22985-103">Assign appliesTo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22985-104">Adicione um aplica-se a um objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) para especificar [](../resources/directoryobject.md) o directoryobject ao qual o [featureRolloutPolicy](../resources/featurerolloutpolicy.md) deve ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="22985-104">Add an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to specify the [directoryObject](../resources/directoryobject.md) to which the [featureRolloutPolicy](../resources/featurerolloutpolicy.md) should be applied to.</span></span>

## <a name="permissions"></a><span data-ttu-id="22985-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="22985-105">Permissions</span></span>

<span data-ttu-id="22985-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22985-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="22985-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22985-108">Permission type</span></span>                        | <span data-ttu-id="22985-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="22985-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="22985-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22985-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="22985-111">Policy. ReadWrite. FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="22985-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="22985-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22985-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22985-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22985-113">Not supported.</span></span> |
| <span data-ttu-id="22985-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22985-114">Application</span></span>                            | <span data-ttu-id="22985-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22985-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="22985-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22985-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directory/featureRolloutPolicies/{id}/appliesTo/$ref
```

## <a name="request-headers"></a><span data-ttu-id="22985-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22985-117">Request headers</span></span>

| <span data-ttu-id="22985-118">Nome</span><span class="sxs-lookup"><span data-stu-id="22985-118">Name</span></span>          | <span data-ttu-id="22985-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="22985-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="22985-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="22985-120">Authorization</span></span> | <span data-ttu-id="22985-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="22985-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="22985-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22985-122">Request body</span></span>

<span data-ttu-id="22985-123">No corpo da solicitação, forneça uma representação JSON de um [](../resources/directoryobject.md) objeto directoryobject.</span><span class="sxs-lookup"><span data-stu-id="22985-123">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="22985-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="22985-124">Response</span></span>

<span data-ttu-id="22985-125">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [directoryobject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22985-125">If successful, this method returns a `201 Created` response code and a new [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="22985-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="22985-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="22985-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22985-127">Request</span></span>

<span data-ttu-id="22985-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="22985-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="22985-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="22985-129">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="22985-130">C#</span><span class="sxs-lookup"><span data-stu-id="22985-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="22985-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="22985-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="22985-132">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="22985-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="22985-133">Java</span><span class="sxs-lookup"><span data-stu-id="22985-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-featurerolloutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="22985-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="22985-134">Response</span></span>

<span data-ttu-id="22985-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="22985-135">The following is an example of the response.</span></span>

> <span data-ttu-id="22985-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22985-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
