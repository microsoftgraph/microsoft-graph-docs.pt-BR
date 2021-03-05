---
title: Atualizar contrato
description: Atualize as propriedades de um objeto agreement.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: a134e26f6e2b8d2994d960759d389525a80673e4
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471562"
---
# <a name="update-agreement"></a><span data-ttu-id="26f08-103">Atualizar contrato</span><span class="sxs-lookup"><span data-stu-id="26f08-103">Update agreement</span></span>

<span data-ttu-id="26f08-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26f08-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26f08-105">Atualize as propriedades de um [objeto agreement.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="26f08-105">Update the properties of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="26f08-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="26f08-106">Permissions</span></span>
<span data-ttu-id="26f08-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26f08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26f08-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26f08-109">Permission type</span></span>                        | <span data-ttu-id="26f08-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="26f08-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="26f08-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26f08-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="26f08-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26f08-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="26f08-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26f08-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26f08-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26f08-114">Not supported.</span></span> |
|<span data-ttu-id="26f08-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26f08-115">Application</span></span>                            | <span data-ttu-id="26f08-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26f08-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="26f08-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26f08-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /identityGovernance/termsOfUse/agreements/{id}
```
## <a name="request-headers"></a><span data-ttu-id="26f08-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26f08-118">Request headers</span></span>
| <span data-ttu-id="26f08-119">Nome</span><span class="sxs-lookup"><span data-stu-id="26f08-119">Name</span></span>         | <span data-ttu-id="26f08-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="26f08-120">Type</span></span>        | <span data-ttu-id="26f08-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="26f08-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="26f08-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="26f08-122">Authorization</span></span> | <span data-ttu-id="26f08-123">string</span><span class="sxs-lookup"><span data-stu-id="26f08-123">string</span></span> | <span data-ttu-id="26f08-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26f08-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26f08-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26f08-126">Request body</span></span>
<span data-ttu-id="26f08-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="26f08-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="26f08-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="26f08-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="26f08-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="26f08-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="26f08-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26f08-130">Property</span></span>     | <span data-ttu-id="26f08-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="26f08-131">Type</span></span>        | <span data-ttu-id="26f08-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="26f08-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="26f08-133">displayName</span><span class="sxs-lookup"><span data-stu-id="26f08-133">displayName</span></span>|<span data-ttu-id="26f08-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26f08-134">String</span></span>|<span data-ttu-id="26f08-135">Nome de exibição do contrato.</span><span class="sxs-lookup"><span data-stu-id="26f08-135">Display name of the agreement.</span></span>|
|<span data-ttu-id="26f08-136">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="26f08-136">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="26f08-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="26f08-137">Boolean</span></span>|<span data-ttu-id="26f08-138">Se o usuário precisa expandir e exibir o contrato antes de aceitar.</span><span class="sxs-lookup"><span data-stu-id="26f08-138">Whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="response"></a><span data-ttu-id="26f08-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="26f08-139">Response</span></span>
<span data-ttu-id="26f08-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto de [contrato](../resources/agreement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26f08-140">If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="26f08-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26f08-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="26f08-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26f08-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_agreement"
}-->
```http
PATCH https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements/{id}
Content-type: application/json
Content-length: 85

{
  "displayName": "displayName-value",
  "isViewingBeforeAcceptanceRequired": true
}
```

##### <a name="response"></a><span data-ttu-id="26f08-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="26f08-143">Response</span></span>
><span data-ttu-id="26f08-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="26f08-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 105

{
  "displayName": "displayName-value",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


