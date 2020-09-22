---
title: Atualizar tokenIssuancePolicy
description: Atualize as propriedades do objeto tokenIssuancePolicy.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2c3f2453fa803ef890f8d152d724a964b88c9108
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074011"
---
# <a name="update-tokenissuancepolicy"></a><span data-ttu-id="ce5e2-103">Atualizar tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="ce5e2-103">Update tokenIssuancePolicy</span></span>

<span data-ttu-id="ce5e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce5e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce5e2-105">Atualiza as propriedades de um objeto [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="ce5e2-105">Update the properties of a [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce5e2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ce5e2-106">Permissions</span></span>

<span data-ttu-id="ce5e2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce5e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ce5e2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce5e2-109">Permission type</span></span>                        | <span data-ttu-id="ce5e2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ce5e2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ce5e2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce5e2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ce5e2-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="ce5e2-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="ce5e2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce5e2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce5e2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce5e2-114">Not supported.</span></span> |
| <span data-ttu-id="ce5e2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce5e2-115">Application</span></span>                            | <span data-ttu-id="ce5e2-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="ce5e2-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce5e2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce5e2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/tokenIssuancePolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ce5e2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce5e2-118">Request headers</span></span>

| <span data-ttu-id="ce5e2-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ce5e2-119">Name</span></span>       | <span data-ttu-id="ce5e2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce5e2-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ce5e2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce5e2-121">Authorization</span></span> | <span data-ttu-id="ce5e2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce5e2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ce5e2-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="ce5e2-124">Content-type</span></span> | <span data-ttu-id="ce5e2-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce5e2-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce5e2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce5e2-127">Request body</span></span>

<span data-ttu-id="ce5e2-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="ce5e2-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ce5e2-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="ce5e2-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ce5e2-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="ce5e2-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ce5e2-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce5e2-131">Property</span></span>     | <span data-ttu-id="ce5e2-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce5e2-132">Type</span></span>        | <span data-ttu-id="ce5e2-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce5e2-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ce5e2-134">definir</span><span class="sxs-lookup"><span data-stu-id="ce5e2-134">definition</span></span>|<span data-ttu-id="ce5e2-135">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce5e2-135">String collection</span></span>| <span data-ttu-id="ce5e2-136">Uma coleção de cadeia de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações da política.</span><span class="sxs-lookup"><span data-stu-id="ce5e2-136">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="ce5e2-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce5e2-137">Required.</span></span>|
|<span data-ttu-id="ce5e2-138">description</span><span class="sxs-lookup"><span data-stu-id="ce5e2-138">description</span></span>|<span data-ttu-id="ce5e2-139">String</span><span class="sxs-lookup"><span data-stu-id="ce5e2-139">String</span></span>| <span data-ttu-id="ce5e2-140">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="ce5e2-140">Description for this policy.</span></span>|
|<span data-ttu-id="ce5e2-141">displayName</span><span class="sxs-lookup"><span data-stu-id="ce5e2-141">displayName</span></span>|<span data-ttu-id="ce5e2-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce5e2-142">String</span></span>| <span data-ttu-id="ce5e2-143">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="ce5e2-143">Display name for this policy.</span></span> <span data-ttu-id="ce5e2-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce5e2-144">Required.</span></span>|
|<span data-ttu-id="ce5e2-145">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="ce5e2-145">isOrganizationDefault</span></span>|<span data-ttu-id="ce5e2-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="ce5e2-146">Boolean</span></span>|<span data-ttu-id="ce5e2-147">Se definido como true, ativa esta política.</span><span class="sxs-lookup"><span data-stu-id="ce5e2-147">If set to true, activates this policy.</span></span> <span data-ttu-id="ce5e2-148">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como a organização padrão.</span><span class="sxs-lookup"><span data-stu-id="ce5e2-148">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="ce5e2-149">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="ce5e2-149">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="ce5e2-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce5e2-150">Response</span></span>

<span data-ttu-id="ce5e2-p108">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce5e2-p108">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce5e2-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ce5e2-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce5e2-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce5e2-154">Request</span></span>

<span data-ttu-id="ce5e2-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce5e2-155">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ce5e2-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce5e2-156">HTTP</span></span>](#tab/http)
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
  "isOrganizationDefault": true,
  "type": "type-value"
}
```
# <a name="c"></a>[<span data-ttu-id="ce5e2-157">C#</span><span class="sxs-lookup"><span data-stu-id="ce5e2-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tokenissuancepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ce5e2-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce5e2-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tokenissuancepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ce5e2-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce5e2-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tokenissuancepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="ce5e2-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce5e2-160">Response</span></span>

<span data-ttu-id="ce5e2-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ce5e2-161">The following is an example of the response.</span></span>

> <span data-ttu-id="ce5e2-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ce5e2-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


