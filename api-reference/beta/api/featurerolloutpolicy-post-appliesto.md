---
title: Atribuir aplica-se
description: Atribua um directoryobject à distribuição de recursos.
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dfde14bace860b847449a3d530103e52e8abc27d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954520"
---
# <a name="assign-appliesto"></a><span data-ttu-id="3ce20-103">Atribuir aplica-se</span><span class="sxs-lookup"><span data-stu-id="3ce20-103">Assign appliesTo</span></span>

<span data-ttu-id="3ce20-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ce20-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ce20-105">Adicione um aplica-se a um objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) para especificar o [directoryobject](../resources/directoryobject.md) ao qual o [featureRolloutPolicy](../resources/featurerolloutpolicy.md) deve ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="3ce20-105">Add an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to specify the [directoryObject](../resources/directoryobject.md) to which the [featureRolloutPolicy](../resources/featurerolloutpolicy.md) should be applied to.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ce20-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3ce20-106">Permissions</span></span>

<span data-ttu-id="3ce20-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ce20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3ce20-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3ce20-109">Permission type</span></span>                        | <span data-ttu-id="3ce20-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3ce20-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3ce20-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ce20-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3ce20-112">Policy.ReadWrite.FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="3ce20-112">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="3ce20-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ce20-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ce20-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ce20-114">Not supported.</span></span> |
| <span data-ttu-id="3ce20-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ce20-115">Application</span></span>                            | <span data-ttu-id="3ce20-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ce20-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ce20-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ce20-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directory/featureRolloutPolicies/{id}/appliesTo/$ref
```

## <a name="request-headers"></a><span data-ttu-id="3ce20-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ce20-118">Request headers</span></span>

| <span data-ttu-id="3ce20-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3ce20-119">Name</span></span>          | <span data-ttu-id="3ce20-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ce20-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3ce20-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ce20-121">Authorization</span></span> | <span data-ttu-id="3ce20-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="3ce20-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ce20-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3ce20-123">Request body</span></span>

<span data-ttu-id="3ce20-124">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryobject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="3ce20-124">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3ce20-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ce20-125">Response</span></span>

<span data-ttu-id="3ce20-126">Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [directoryobject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ce20-126">If successful, this method returns a `201 Created` response code and a new [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3ce20-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3ce20-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3ce20-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ce20-128">Request</span></span>

<span data-ttu-id="3ce20-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ce20-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3ce20-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ce20-130">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3ce20-131">C#</span><span class="sxs-lookup"><span data-stu-id="3ce20-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ce20-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ce20-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ce20-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ce20-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3ce20-134">Java</span><span class="sxs-lookup"><span data-stu-id="3ce20-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-featurerolloutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3ce20-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ce20-135">Response</span></span>

<span data-ttu-id="3ce20-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3ce20-136">The following is an example of the response.</span></span>

> <span data-ttu-id="3ce20-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ce20-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


