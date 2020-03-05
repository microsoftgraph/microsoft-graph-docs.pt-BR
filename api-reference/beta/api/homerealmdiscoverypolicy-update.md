---
title: Atualizar homerealmdiscoverypolicy
description: Atualize as propriedades do objeto homeRealmDiscoveryPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2604911f823413ff7e29cb4e90fae5e0273b520e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446524"
---
# <a name="update-homerealmdiscoverypolicy"></a><span data-ttu-id="1e01b-103">Atualizar homerealmdiscoverypolicy</span><span class="sxs-lookup"><span data-stu-id="1e01b-103">Update homerealmdiscoverypolicy</span></span>

<span data-ttu-id="1e01b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1e01b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e01b-105">Atualiza as propriedades de um objeto [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="1e01b-105">Update the properties of a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e01b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1e01b-106">Permissions</span></span>

<span data-ttu-id="1e01b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e01b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1e01b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e01b-109">Permission type</span></span>                        | <span data-ttu-id="1e01b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1e01b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1e01b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e01b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1e01b-112">Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="1e01b-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="1e01b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e01b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e01b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e01b-114">Not supported.</span></span> |
| <span data-ttu-id="1e01b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e01b-115">Application</span></span>                            | <span data-ttu-id="1e01b-116">Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="1e01b-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e01b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e01b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/homeRealmDiscoveryPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1e01b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e01b-118">Request headers</span></span>

| <span data-ttu-id="1e01b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1e01b-119">Name</span></span>       | <span data-ttu-id="1e01b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e01b-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1e01b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e01b-121">Authorization</span></span> | <span data-ttu-id="1e01b-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="1e01b-122">Bearer {token}</span></span> |
| <span data-ttu-id="1e01b-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="1e01b-123">Content-type</span></span> | <span data-ttu-id="1e01b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1e01b-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e01b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e01b-125">Request body</span></span>

<span data-ttu-id="1e01b-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="1e01b-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="1e01b-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="1e01b-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1e01b-128">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="1e01b-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1e01b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e01b-129">Property</span></span>     | <span data-ttu-id="1e01b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e01b-130">Type</span></span>        | <span data-ttu-id="1e01b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e01b-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1e01b-132">definir</span><span class="sxs-lookup"><span data-stu-id="1e01b-132">definition</span></span>|<span data-ttu-id="1e01b-133">String collection</span><span class="sxs-lookup"><span data-stu-id="1e01b-133">String collection</span></span>| <span data-ttu-id="1e01b-134">Uma coleção de cadeia de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações da política.</span><span class="sxs-lookup"><span data-stu-id="1e01b-134">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="1e01b-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e01b-135">Required.</span></span>|
|<span data-ttu-id="1e01b-136">description</span><span class="sxs-lookup"><span data-stu-id="1e01b-136">description</span></span>|<span data-ttu-id="1e01b-137">String</span><span class="sxs-lookup"><span data-stu-id="1e01b-137">String</span></span>| <span data-ttu-id="1e01b-138">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="1e01b-138">Description for this policy.</span></span>|
|<span data-ttu-id="1e01b-139">displayName</span><span class="sxs-lookup"><span data-stu-id="1e01b-139">displayName</span></span>|<span data-ttu-id="1e01b-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e01b-140">String</span></span>| <span data-ttu-id="1e01b-141">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="1e01b-141">Display name for this policy.</span></span> <span data-ttu-id="1e01b-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e01b-142">Required.</span></span>|
|<span data-ttu-id="1e01b-143">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="1e01b-143">isOrganizationDefault</span></span>|<span data-ttu-id="1e01b-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e01b-144">Boolean</span></span>|<span data-ttu-id="1e01b-145">Se definido como true, ativa esta política.</span><span class="sxs-lookup"><span data-stu-id="1e01b-145">If set to true, activates this policy.</span></span> <span data-ttu-id="1e01b-146">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como a organização padrão.</span><span class="sxs-lookup"><span data-stu-id="1e01b-146">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="1e01b-147">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="1e01b-147">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="1e01b-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e01b-148">Response</span></span>

<span data-ttu-id="1e01b-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e01b-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e01b-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e01b-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e01b-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e01b-152">Request</span></span>

<span data-ttu-id="1e01b-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e01b-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1e01b-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="1e01b-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_homerealmdiscoverypolicy"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies/{id}
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
# <a name="javascript"></a>[<span data-ttu-id="1e01b-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1e01b-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-homerealmdiscoverypolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1e01b-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e01b-156">Response</span></span>

<span data-ttu-id="1e01b-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1e01b-157">The following is an example of the response.</span></span>

> <span data-ttu-id="1e01b-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e01b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy"
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
  "description": "Update homerealmdiscoverypolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
