---
title: Atualizar tokenIssuancePolicy
description: Atualize as propriedades do objeto tokenIssuancePolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c93df515e3ac0038d5134e416b91175ef0846ff5
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591597"
---
# <a name="update-tokenissuancepolicy"></a><span data-ttu-id="6aca4-103">Atualizar tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="6aca4-103">Update tokenIssuancePolicy</span></span>

<span data-ttu-id="6aca4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6aca4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6aca4-105">Atualiza as propriedades de um objeto [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="6aca4-105">Update the properties of a [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6aca4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6aca4-106">Permissions</span></span>

<span data-ttu-id="6aca4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6aca4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6aca4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6aca4-109">Permission type</span></span>                        | <span data-ttu-id="6aca4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6aca4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6aca4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6aca4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6aca4-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="6aca4-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="6aca4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6aca4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6aca4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6aca4-114">Not supported.</span></span> |
| <span data-ttu-id="6aca4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6aca4-115">Application</span></span>                            | <span data-ttu-id="6aca4-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="6aca4-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="6aca4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6aca4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/tokenIssuancePolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6aca4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6aca4-118">Request headers</span></span>

| <span data-ttu-id="6aca4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6aca4-119">Name</span></span>       | <span data-ttu-id="6aca4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6aca4-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6aca4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6aca4-121">Authorization</span></span> | <span data-ttu-id="6aca4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6aca4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6aca4-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="6aca4-124">Content-type</span></span> | <span data-ttu-id="6aca4-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6aca4-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6aca4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6aca4-127">Request body</span></span>

<span data-ttu-id="6aca4-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="6aca4-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="6aca4-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="6aca4-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6aca4-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="6aca4-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6aca4-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6aca4-131">Property</span></span>     | <span data-ttu-id="6aca4-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="6aca4-132">Type</span></span>        | <span data-ttu-id="6aca4-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="6aca4-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6aca4-134">definir</span><span class="sxs-lookup"><span data-stu-id="6aca4-134">definition</span></span>|<span data-ttu-id="6aca4-135">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6aca4-135">String collection</span></span>| <span data-ttu-id="6aca4-136">Uma coleção de cadeia de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações da política.</span><span class="sxs-lookup"><span data-stu-id="6aca4-136">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="6aca4-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6aca4-137">Required.</span></span>|
|<span data-ttu-id="6aca4-138">description</span><span class="sxs-lookup"><span data-stu-id="6aca4-138">description</span></span>|<span data-ttu-id="6aca4-139">String</span><span class="sxs-lookup"><span data-stu-id="6aca4-139">String</span></span>| <span data-ttu-id="6aca4-140">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="6aca4-140">Description for this policy.</span></span>|
|<span data-ttu-id="6aca4-141">displayName</span><span class="sxs-lookup"><span data-stu-id="6aca4-141">displayName</span></span>|<span data-ttu-id="6aca4-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6aca4-142">String</span></span>| <span data-ttu-id="6aca4-143">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="6aca4-143">Display name for this policy.</span></span> <span data-ttu-id="6aca4-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6aca4-144">Required.</span></span>|
|<span data-ttu-id="6aca4-145">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="6aca4-145">isOrganizationDefault</span></span>|<span data-ttu-id="6aca4-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="6aca4-146">Boolean</span></span>|<span data-ttu-id="6aca4-147">Se definido como true, ativa esta política.</span><span class="sxs-lookup"><span data-stu-id="6aca4-147">If set to true, activates this policy.</span></span> <span data-ttu-id="6aca4-148">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como a organização padrão.</span><span class="sxs-lookup"><span data-stu-id="6aca4-148">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="6aca4-149">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="6aca4-149">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="6aca4-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="6aca4-150">Response</span></span>

<span data-ttu-id="6aca4-p108">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6aca4-p108">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6aca4-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6aca4-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="6aca4-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6aca4-154">Request</span></span>

<span data-ttu-id="6aca4-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6aca4-155">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6aca4-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="6aca4-156">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6aca4-157">C#</span><span class="sxs-lookup"><span data-stu-id="6aca4-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tokenissuancepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6aca4-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6aca4-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tokenissuancepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6aca4-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6aca4-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tokenissuancepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="6aca4-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="6aca4-160">Response</span></span>

<span data-ttu-id="6aca4-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6aca4-161">The following is an example of the response.</span></span>

> <span data-ttu-id="6aca4-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6aca4-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
