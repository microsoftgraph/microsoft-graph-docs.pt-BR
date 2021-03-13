---
title: Atualizar contrato
description: Atualize as propriedades de um objeto agreement.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 88bab29854bd474221df81241698b57fa94be79a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773925"
---
# <a name="update-agreement"></a><span data-ttu-id="c61b7-103">Atualizar contrato</span><span class="sxs-lookup"><span data-stu-id="c61b7-103">Update agreement</span></span>

<span data-ttu-id="c61b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c61b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c61b7-105">Atualize as propriedades de um [objeto agreement.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="c61b7-105">Update the properties of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c61b7-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="c61b7-106">Permissions</span></span>
<span data-ttu-id="c61b7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c61b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c61b7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c61b7-109">Permission type</span></span>                        | <span data-ttu-id="c61b7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c61b7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c61b7-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c61b7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c61b7-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c61b7-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="c61b7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c61b7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c61b7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c61b7-114">Not supported.</span></span> |
|<span data-ttu-id="c61b7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c61b7-115">Application</span></span>                            | <span data-ttu-id="c61b7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c61b7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c61b7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c61b7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /identityGovernance/termsOfUse/agreements/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c61b7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c61b7-118">Request headers</span></span>
| <span data-ttu-id="c61b7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c61b7-119">Name</span></span>         | <span data-ttu-id="c61b7-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="c61b7-120">Type</span></span>        | <span data-ttu-id="c61b7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c61b7-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c61b7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c61b7-122">Authorization</span></span> | <span data-ttu-id="c61b7-123">string</span><span class="sxs-lookup"><span data-stu-id="c61b7-123">string</span></span> | <span data-ttu-id="c61b7-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c61b7-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c61b7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c61b7-126">Request body</span></span>
<span data-ttu-id="c61b7-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="c61b7-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c61b7-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="c61b7-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c61b7-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="c61b7-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c61b7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c61b7-130">Property</span></span>     | <span data-ttu-id="c61b7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c61b7-131">Type</span></span>        | <span data-ttu-id="c61b7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c61b7-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c61b7-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c61b7-133">displayName</span></span>|<span data-ttu-id="c61b7-134">String</span><span class="sxs-lookup"><span data-stu-id="c61b7-134">String</span></span>|<span data-ttu-id="c61b7-135">Nome de exibição do contrato.</span><span class="sxs-lookup"><span data-stu-id="c61b7-135">Display name of the agreement.</span></span>|
|<span data-ttu-id="c61b7-136">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="c61b7-136">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="c61b7-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="c61b7-137">Boolean</span></span>|<span data-ttu-id="c61b7-138">Se o usuário precisa expandir e exibir o contrato antes de aceitar.</span><span class="sxs-lookup"><span data-stu-id="c61b7-138">Whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="response"></a><span data-ttu-id="c61b7-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c61b7-139">Response</span></span>
<span data-ttu-id="c61b7-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto de [contrato](../resources/agreement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c61b7-140">If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c61b7-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c61b7-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c61b7-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c61b7-142">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c61b7-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="c61b7-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c61b7-144">C#</span><span class="sxs-lookup"><span data-stu-id="c61b7-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c61b7-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c61b7-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c61b7-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c61b7-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c61b7-147">Java</span><span class="sxs-lookup"><span data-stu-id="c61b7-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c61b7-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="c61b7-148">Response</span></span>
><span data-ttu-id="c61b7-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c61b7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


