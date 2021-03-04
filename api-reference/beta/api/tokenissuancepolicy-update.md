---
title: Atualizar tokenIssuancePolicy
description: Atualize as propriedades do objeto tokenIssuancePolicy.
localization_priority: Normal
author: luleonpla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ac961d39c90eca0f00c2a2691a4d4a20a5f157a4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433681"
---
# <a name="update-tokenissuancepolicy"></a><span data-ttu-id="b63d8-103">Atualizar tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="b63d8-103">Update tokenIssuancePolicy</span></span>

<span data-ttu-id="b63d8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b63d8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b63d8-105">Atualize as propriedades de um [objeto tokenIssuancePolicy.](../resources/tokenIssuancePolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b63d8-105">Update the properties of a [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b63d8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b63d8-106">Permissions</span></span>

<span data-ttu-id="b63d8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b63d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b63d8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b63d8-109">Permission type</span></span>                        | <span data-ttu-id="b63d8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b63d8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b63d8-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b63d8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b63d8-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="b63d8-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="b63d8-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b63d8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b63d8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b63d8-114">Not supported.</span></span> |
| <span data-ttu-id="b63d8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b63d8-115">Application</span></span>                            | <span data-ttu-id="b63d8-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="b63d8-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="b63d8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b63d8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/tokenIssuancePolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b63d8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b63d8-118">Request headers</span></span>

| <span data-ttu-id="b63d8-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b63d8-119">Name</span></span>       | <span data-ttu-id="b63d8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b63d8-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b63d8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b63d8-121">Authorization</span></span> | <span data-ttu-id="b63d8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b63d8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b63d8-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="b63d8-124">Content-type</span></span> | <span data-ttu-id="b63d8-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b63d8-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b63d8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b63d8-127">Request body</span></span>

<span data-ttu-id="b63d8-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="b63d8-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b63d8-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="b63d8-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b63d8-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b63d8-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b63d8-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b63d8-131">Property</span></span>     | <span data-ttu-id="b63d8-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="b63d8-132">Type</span></span>        | <span data-ttu-id="b63d8-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="b63d8-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b63d8-134">definition</span><span class="sxs-lookup"><span data-stu-id="b63d8-134">definition</span></span>|<span data-ttu-id="b63d8-135">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b63d8-135">String collection</span></span>| <span data-ttu-id="b63d8-136">Uma coleção de cadeias de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações dessa política.</span><span class="sxs-lookup"><span data-stu-id="b63d8-136">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="b63d8-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b63d8-137">Required.</span></span>|
|<span data-ttu-id="b63d8-138">description</span><span class="sxs-lookup"><span data-stu-id="b63d8-138">description</span></span>|<span data-ttu-id="b63d8-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b63d8-139">String</span></span>| <span data-ttu-id="b63d8-140">Descrição dessa política.</span><span class="sxs-lookup"><span data-stu-id="b63d8-140">Description for this policy.</span></span>|
|<span data-ttu-id="b63d8-141">displayName</span><span class="sxs-lookup"><span data-stu-id="b63d8-141">displayName</span></span>|<span data-ttu-id="b63d8-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b63d8-142">String</span></span>| <span data-ttu-id="b63d8-143">Nome de exibição para esta política.</span><span class="sxs-lookup"><span data-stu-id="b63d8-143">Display name for this policy.</span></span> <span data-ttu-id="b63d8-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b63d8-144">Required.</span></span>|
|<span data-ttu-id="b63d8-145">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="b63d8-145">isOrganizationDefault</span></span>|<span data-ttu-id="b63d8-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b63d8-146">Boolean</span></span>|<span data-ttu-id="b63d8-147">Se definido como true, ativa essa política.</span><span class="sxs-lookup"><span data-stu-id="b63d8-147">If set to true, activates this policy.</span></span> <span data-ttu-id="b63d8-148">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como o padrão da organização.</span><span class="sxs-lookup"><span data-stu-id="b63d8-148">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="b63d8-149">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="b63d8-149">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="b63d8-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="b63d8-150">Response</span></span>

<span data-ttu-id="b63d8-p108">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b63d8-p108">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b63d8-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b63d8-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="b63d8-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b63d8-154">Request</span></span>

<span data-ttu-id="b63d8-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b63d8-155">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b63d8-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="b63d8-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tokenissuancepolicy"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/tokenIssuancePolicies/{id}
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="c"></a>[<span data-ttu-id="b63d8-157">C#</span><span class="sxs-lookup"><span data-stu-id="b63d8-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tokenissuancepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b63d8-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b63d8-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tokenissuancepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b63d8-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b63d8-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tokenissuancepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b63d8-160">Java</span><span class="sxs-lookup"><span data-stu-id="b63d8-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tokenissuancepolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="b63d8-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="b63d8-161">Response</span></span>

<span data-ttu-id="b63d8-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b63d8-162">The following is an example of the response.</span></span>

> <span data-ttu-id="b63d8-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b63d8-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenIssuancePolicy"
} -->

```http
HTTP/1.1 204 No Content
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tokenissuancepolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


