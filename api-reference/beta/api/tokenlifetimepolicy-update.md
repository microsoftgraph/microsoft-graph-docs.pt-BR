---
title: Atualizar tokenlifetimepolicy
description: Atualize as propriedades do objeto tokenLifetimePolicy.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c64a246df4d1f3fa5cf19aae4457566041e30991
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051750"
---
# <a name="update-tokenlifetimepolicy"></a><span data-ttu-id="6deb7-103">Atualizar tokenlifetimepolicy</span><span class="sxs-lookup"><span data-stu-id="6deb7-103">Update tokenlifetimepolicy</span></span>

<span data-ttu-id="6deb7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6deb7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6deb7-105">Atualize as propriedades de um [objeto tokenLifetimePolicy.](../resources/tokenlifetimepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6deb7-105">Update the properties of a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6deb7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6deb7-106">Permissions</span></span>

<span data-ttu-id="6deb7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6deb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6deb7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6deb7-109">Permission type</span></span>                        | <span data-ttu-id="6deb7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6deb7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6deb7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6deb7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6deb7-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="6deb7-112">Policy.ReadWrite.ApplicationConfiguration</span></span>|
| <span data-ttu-id="6deb7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6deb7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6deb7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6deb7-114">Not supported.</span></span> |
| <span data-ttu-id="6deb7-115">Application</span><span class="sxs-lookup"><span data-stu-id="6deb7-115">Application</span></span>                            | <span data-ttu-id="6deb7-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="6deb7-116">Policy.ReadWrite.ApplicationConfiguration</span></span>|

## <a name="http-request"></a><span data-ttu-id="6deb7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6deb7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/tokenLifetimePolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6deb7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6deb7-118">Request headers</span></span>

| <span data-ttu-id="6deb7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6deb7-119">Name</span></span>       | <span data-ttu-id="6deb7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6deb7-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6deb7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6deb7-121">Authorization</span></span> | <span data-ttu-id="6deb7-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="6deb7-122">Bearer {token}</span></span> |
| <span data-ttu-id="6deb7-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="6deb7-123">Content-type</span></span> | <span data-ttu-id="6deb7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6deb7-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6deb7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6deb7-125">Request body</span></span>

<span data-ttu-id="6deb7-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="6deb7-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="6deb7-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="6deb7-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6deb7-128">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="6deb7-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6deb7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6deb7-129">Property</span></span>     | <span data-ttu-id="6deb7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6deb7-130">Type</span></span>        | <span data-ttu-id="6deb7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6deb7-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6deb7-132">definition</span><span class="sxs-lookup"><span data-stu-id="6deb7-132">definition</span></span>|<span data-ttu-id="6deb7-133">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6deb7-133">String collection</span></span>| <span data-ttu-id="6deb7-134">Uma coleção de cadeias de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações dessa política.</span><span class="sxs-lookup"><span data-stu-id="6deb7-134">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="6deb7-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6deb7-135">Required.</span></span>|
|<span data-ttu-id="6deb7-136">description</span><span class="sxs-lookup"><span data-stu-id="6deb7-136">description</span></span>|<span data-ttu-id="6deb7-137">String</span><span class="sxs-lookup"><span data-stu-id="6deb7-137">String</span></span>| <span data-ttu-id="6deb7-138">Descrição dessa política.</span><span class="sxs-lookup"><span data-stu-id="6deb7-138">Description for this policy.</span></span>|
|<span data-ttu-id="6deb7-139">displayName</span><span class="sxs-lookup"><span data-stu-id="6deb7-139">displayName</span></span>|<span data-ttu-id="6deb7-140">String</span><span class="sxs-lookup"><span data-stu-id="6deb7-140">String</span></span>| <span data-ttu-id="6deb7-141">Nome de exibição para esta política.</span><span class="sxs-lookup"><span data-stu-id="6deb7-141">Display name for this policy.</span></span> <span data-ttu-id="6deb7-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6deb7-142">Required.</span></span>|
|<span data-ttu-id="6deb7-143">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="6deb7-143">isOrganizationDefault</span></span>|<span data-ttu-id="6deb7-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="6deb7-144">Boolean</span></span>|<span data-ttu-id="6deb7-145">Se definido como true, ativa essa política.</span><span class="sxs-lookup"><span data-stu-id="6deb7-145">If set to true, activates this policy.</span></span> <span data-ttu-id="6deb7-146">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como o padrão da organização.</span><span class="sxs-lookup"><span data-stu-id="6deb7-146">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="6deb7-147">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="6deb7-147">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="6deb7-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="6deb7-148">Response</span></span>

<span data-ttu-id="6deb7-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6deb7-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6deb7-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6deb7-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="6deb7-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6deb7-152">Request</span></span>

<span data-ttu-id="6deb7-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6deb7-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6deb7-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="6deb7-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tokenlifetimepolicy"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/{id}
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="javascript"></a>[<span data-ttu-id="6deb7-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6deb7-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tokenlifetimepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="6deb7-156">C#</span><span class="sxs-lookup"><span data-stu-id="6deb7-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tokenlifetimepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6deb7-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6deb7-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tokenlifetimepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6deb7-158">Java</span><span class="sxs-lookup"><span data-stu-id="6deb7-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tokenlifetimepolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6deb7-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="6deb7-159">Response</span></span>

<span data-ttu-id="6deb7-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6deb7-160">The following is an example of the response.</span></span>

> <span data-ttu-id="6deb7-161">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6deb7-161">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy"
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
  "description": "Update tokenlifetimepolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


