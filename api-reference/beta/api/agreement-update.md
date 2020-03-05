---
title: Atualizar contrato
description: Atualizar as propriedades de um objeto de contrato.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 96835b74e0eea03f9b593a9848bc7946eb23554f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441638"
---
# <a name="update-agreement"></a><span data-ttu-id="bc7ce-103">Atualizar contrato</span><span class="sxs-lookup"><span data-stu-id="bc7ce-103">Update agreement</span></span>

<span data-ttu-id="bc7ce-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bc7ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc7ce-105">Atualizar as propriedades de um objeto de [contrato](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="bc7ce-105">Update the properties of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bc7ce-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bc7ce-106">Permissions</span></span>
<span data-ttu-id="bc7ce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc7ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc7ce-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc7ce-109">Permission type</span></span>                        | <span data-ttu-id="bc7ce-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bc7ce-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc7ce-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc7ce-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bc7ce-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc7ce-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="bc7ce-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc7ce-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc7ce-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc7ce-114">Not supported.</span></span> |
|<span data-ttu-id="bc7ce-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc7ce-115">Application</span></span>                            | <span data-ttu-id="bc7ce-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc7ce-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc7ce-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc7ce-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /agreements/{id}
```
## <a name="request-headers"></a><span data-ttu-id="bc7ce-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc7ce-118">Request headers</span></span>
| <span data-ttu-id="bc7ce-119">Nome</span><span class="sxs-lookup"><span data-stu-id="bc7ce-119">Name</span></span>         | <span data-ttu-id="bc7ce-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc7ce-120">Type</span></span>        | <span data-ttu-id="bc7ce-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc7ce-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="bc7ce-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc7ce-122">Authorization</span></span> | <span data-ttu-id="bc7ce-123">string</span><span class="sxs-lookup"><span data-stu-id="bc7ce-123">string</span></span> | <span data-ttu-id="bc7ce-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc7ce-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc7ce-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc7ce-126">Request body</span></span>
<span data-ttu-id="bc7ce-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="bc7ce-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="bc7ce-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="bc7ce-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="bc7ce-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="bc7ce-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bc7ce-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc7ce-130">Property</span></span>     | <span data-ttu-id="bc7ce-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc7ce-131">Type</span></span>        | <span data-ttu-id="bc7ce-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc7ce-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bc7ce-133">displayName</span><span class="sxs-lookup"><span data-stu-id="bc7ce-133">displayName</span></span>|<span data-ttu-id="bc7ce-134">String</span><span class="sxs-lookup"><span data-stu-id="bc7ce-134">String</span></span>|<span data-ttu-id="bc7ce-135">Nome para exibição do contrato.</span><span class="sxs-lookup"><span data-stu-id="bc7ce-135">Display name of the agreement.</span></span>|
|<span data-ttu-id="bc7ce-136">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="bc7ce-136">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="bc7ce-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc7ce-137">Boolean</span></span>|<span data-ttu-id="bc7ce-138">Se o usuário tem que expandir e exibir o contrato antes de aceitar o.</span><span class="sxs-lookup"><span data-stu-id="bc7ce-138">Whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="response"></a><span data-ttu-id="bc7ce-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc7ce-139">Response</span></span>
<span data-ttu-id="bc7ce-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Agreement](../resources/agreement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc7ce-140">If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bc7ce-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc7ce-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc7ce-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc7ce-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="bc7ce-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc7ce-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_agreement"
}-->
```http
PATCH https://graph.microsoft.com/beta/agreements/{id}
Content-type: application/json
Content-length: 85

{
  "displayName": "displayName-value",
  "isViewingBeforeAcceptanceRequired": true
}
```
# <a name="c"></a>[<span data-ttu-id="bc7ce-144">C#</span><span class="sxs-lookup"><span data-stu-id="bc7ce-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bc7ce-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc7ce-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bc7ce-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bc7ce-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bc7ce-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc7ce-147">Response</span></span>
><span data-ttu-id="bc7ce-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bc7ce-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
