---
title: Atualizar conditionalAccessPolicy
description: Atualiza as propriedades de um objeto conditionalAccessPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9ef732cbc58028a8665172cec87a2d079f55925a
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638425"
---
# <a name="update-conditionalaccesspolicy"></a><span data-ttu-id="774a0-103">Atualizar conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="774a0-103">Update conditionalAccessPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="774a0-104">Atualiza as propriedades de um objeto [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="774a0-104">Update the properties of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="774a0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="774a0-105">Permissions</span></span>

<span data-ttu-id="774a0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="774a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="774a0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="774a0-108">Permission type</span></span>                        | <span data-ttu-id="774a0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="774a0-109">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="774a0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="774a0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="774a0-111">Policy. ReadWrite. ConditionalAccess e Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="774a0-111">Policy.ReadWrite.ConditionalAccess and Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="774a0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="774a0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="774a0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="774a0-113">Not supported.</span></span> |
|<span data-ttu-id="774a0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="774a0-114">Application</span></span>                            | <span data-ttu-id="774a0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="774a0-115">Not supported.</span></span> |

>[!NOTE]
><span data-ttu-id="774a0-116">Essa API requer várias permissões.</span><span class="sxs-lookup"><span data-stu-id="774a0-116">This API requires multiple permissions.</span></span> <span data-ttu-id="774a0-117">Para obter detalhes, consulte [known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span><span class="sxs-lookup"><span data-stu-id="774a0-117">For details, see [Known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span></span>

## <a name="http-request"></a><span data-ttu-id="774a0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="774a0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /conditionalAccess/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="774a0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="774a0-119">Request headers</span></span>

| <span data-ttu-id="774a0-120">Nome</span><span class="sxs-lookup"><span data-stu-id="774a0-120">Name</span></span>          | <span data-ttu-id="774a0-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="774a0-121">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="774a0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="774a0-122">Authorization</span></span> | <span data-ttu-id="774a0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="774a0-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="774a0-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="774a0-125">Content-Type</span></span>  | <span data-ttu-id="774a0-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="774a0-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="774a0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="774a0-128">Request body</span></span>

<span data-ttu-id="774a0-129">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="774a0-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="774a0-130">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="774a0-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="774a0-131">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="774a0-131">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="774a0-132">Para obter a lista de propriedades, consulte [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="774a0-132">For the list of properties, see [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md).</span></span>

## <a name="response"></a><span data-ttu-id="774a0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="774a0-133">Response</span></span>

<span data-ttu-id="774a0-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="774a0-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="774a0-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="774a0-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="774a0-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="774a0-137">Request</span></span>

<span data-ttu-id="774a0-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="774a0-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_conditionalaccesspolicy"
}-->

```http
PATCH https://graph.microsoft.com/beta/conditionalAccess/policies/{id}
Content-type: application/json

{
    "conditions": {
        "signInRiskLevels": [
            "high",
            "medium",
            "low",
        ]
    }
}
```

### <a name="response"></a><span data-ttu-id="774a0-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="774a0-139">Response</span></span>

<span data-ttu-id="774a0-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="774a0-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update conditionalaccesspolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
