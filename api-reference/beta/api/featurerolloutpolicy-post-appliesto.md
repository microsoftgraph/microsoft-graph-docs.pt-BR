---
title: Atribuir aplica-se
description: Atribua um directoryobject à distribuição de recursos.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b5a01131adb20feccbccd55c2ce4f7e01ea1e214
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062090"
---
# <a name="assign-appliesto"></a><span data-ttu-id="f9b08-103">Atribuir aplica-se</span><span class="sxs-lookup"><span data-stu-id="f9b08-103">Assign appliesTo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9b08-104">Adicione um aplica-se a um objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) para especificar [](../resources/directoryobject.md) o directoryobject ao qual o [featureRolloutPolicy](../resources/featurerolloutpolicy.md) deve ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="f9b08-104">Add an appliesTo on a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object to specify the [directoryObject](../resources/directoryobject.md) to which the [featureRolloutPolicy](../resources/featurerolloutpolicy.md) should be applied to.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9b08-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f9b08-105">Permissions</span></span>

<span data-ttu-id="f9b08-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9b08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f9b08-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9b08-108">Permission type</span></span>                        | <span data-ttu-id="f9b08-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f9b08-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f9b08-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9b08-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f9b08-111">Policy. ReadWrite. FeatureRollout</span><span class="sxs-lookup"><span data-stu-id="f9b08-111">Policy.ReadWrite.FeatureRollout</span></span> |
| <span data-ttu-id="f9b08-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9b08-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9b08-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9b08-113">Not supported.</span></span> |
| <span data-ttu-id="f9b08-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9b08-114">Application</span></span>                            | <span data-ttu-id="f9b08-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9b08-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9b08-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9b08-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directory/featureRolloutPolicies/{id}/appliesTo/$ref
```

## <a name="request-headers"></a><span data-ttu-id="f9b08-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9b08-117">Request headers</span></span>

| <span data-ttu-id="f9b08-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f9b08-118">Name</span></span>          | <span data-ttu-id="f9b08-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9b08-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f9b08-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9b08-120">Authorization</span></span> | <span data-ttu-id="f9b08-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="f9b08-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9b08-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9b08-122">Request body</span></span>

<span data-ttu-id="f9b08-123">No corpo da solicitação, forneça uma representação JSON de um [](../resources/directoryobject.md) objeto directoryobject.</span><span class="sxs-lookup"><span data-stu-id="f9b08-123">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f9b08-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9b08-124">Response</span></span>

<span data-ttu-id="f9b08-125">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [directoryobject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9b08-125">If successful, this method returns a `201 Created` response code and a new [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f9b08-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f9b08-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f9b08-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9b08-127">Request</span></span>

<span data-ttu-id="f9b08-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9b08-128">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f9b08-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9b08-129">Response</span></span>

<span data-ttu-id="f9b08-130">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f9b08-130">The following is an example of the response.</span></span>

> <span data-ttu-id="f9b08-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9b08-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
