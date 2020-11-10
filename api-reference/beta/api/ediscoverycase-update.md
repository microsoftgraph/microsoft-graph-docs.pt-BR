---
title: Atualizar ediscoverycase
description: Atualiza as propriedades de um objeto ediscoveryCase.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 630beb848fe5fba2636ea4247f84b448f91fb465
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966688"
---
# <a name="update-ediscoverycase"></a><span data-ttu-id="5980a-103">Atualizar ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="5980a-103">Update ediscoveryCase</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5980a-104">Atualiza as propriedades de um objeto [ediscoveryCase](../resources/ediscoverycase.md) .</span><span class="sxs-lookup"><span data-stu-id="5980a-104">Update the properties of an [ediscoveryCase](../resources/ediscoverycase.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5980a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5980a-105">Permissions</span></span>

<span data-ttu-id="5980a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5980a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5980a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5980a-108">Permission type</span></span>                        | <span data-ttu-id="5980a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5980a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5980a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5980a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5980a-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="5980a-111">User.Read</span></span>      |
| <span data-ttu-id="5980a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5980a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5980a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5980a-113">Not supported.</span></span> |
| <span data-ttu-id="5980a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5980a-114">Application</span></span>                            | <span data-ttu-id="5980a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5980a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5980a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5980a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /compliance/ediscovery/cases/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5980a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5980a-117">Request headers</span></span>

| <span data-ttu-id="5980a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="5980a-118">Name</span></span>       | <span data-ttu-id="5980a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="5980a-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5980a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="5980a-120">Authorization</span></span> | <span data-ttu-id="5980a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5980a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5980a-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5980a-123">Request body</span></span>

<span data-ttu-id="5980a-124">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="5980a-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5980a-125">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="5980a-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5980a-126">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="5980a-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5980a-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5980a-127">Property</span></span>     | <span data-ttu-id="5980a-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="5980a-128">Type</span></span>        | <span data-ttu-id="5980a-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="5980a-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5980a-130">description</span><span class="sxs-lookup"><span data-stu-id="5980a-130">description</span></span>|<span data-ttu-id="5980a-131">String</span><span class="sxs-lookup"><span data-stu-id="5980a-131">String</span></span>| <span data-ttu-id="5980a-132">A descrição do caso.</span><span class="sxs-lookup"><span data-stu-id="5980a-132">The case description.</span></span> |
|<span data-ttu-id="5980a-133">displayName</span><span class="sxs-lookup"><span data-stu-id="5980a-133">displayName</span></span>|<span data-ttu-id="5980a-134">String</span><span class="sxs-lookup"><span data-stu-id="5980a-134">String</span></span>| <span data-ttu-id="5980a-135">O nome do caso.</span><span class="sxs-lookup"><span data-stu-id="5980a-135">The case name.</span></span> |
|<span data-ttu-id="5980a-136">externalId</span><span class="sxs-lookup"><span data-stu-id="5980a-136">externalId</span></span>|<span data-ttu-id="5980a-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5980a-137">String</span></span>| <span data-ttu-id="5980a-138">O número do caso externo para referência de cliente.</span><span class="sxs-lookup"><span data-stu-id="5980a-138">The external case number for customer reference.</span></span> |

## <a name="response"></a><span data-ttu-id="5980a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="5980a-139">Response</span></span>

<span data-ttu-id="5980a-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5980a-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5980a-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5980a-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5980a-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5980a-143">Request</span></span>

<span data-ttu-id="5980a-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5980a-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5980a-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="5980a-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_ediscoverycase"
}-->

```http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583
Content-type: application/json

{
  "displayName": "My Case 1 - Renamed",
  "description": "Updated description",
  "externalId": "Updated externalId"
}
```
# <a name="c"></a>[<span data-ttu-id="5980a-146">C#</span><span class="sxs-lookup"><span data-stu-id="5980a-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-ediscoverycase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5980a-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5980a-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-ediscoverycase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5980a-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5980a-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-ediscoverycase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5980a-149">Java</span><span class="sxs-lookup"><span data-stu-id="5980a-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-ediscoverycase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5980a-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="5980a-150">Response</span></span>

<span data-ttu-id="5980a-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5980a-151">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscoveryCase"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update ediscoverycase",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


