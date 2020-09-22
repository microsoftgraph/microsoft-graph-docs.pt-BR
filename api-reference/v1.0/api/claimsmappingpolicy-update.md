---
title: Atualizar claimsmappingpolicy
description: Atualize as propriedades do objeto claimsMappingPolicy.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dbc70494077e9d2dea878c2da8657b3cf630aef1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083866"
---
# <a name="update-claimsmappingpolicy"></a><span data-ttu-id="e187e-103">Atualizar claimsmappingpolicy</span><span class="sxs-lookup"><span data-stu-id="e187e-103">Update claimsmappingpolicy</span></span>

<span data-ttu-id="e187e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e187e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e187e-105">Atualiza as propriedades de um objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="e187e-105">Update the properties of a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e187e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e187e-106">Permissions</span></span>

<span data-ttu-id="e187e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e187e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e187e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e187e-109">Permission type</span></span>                        | <span data-ttu-id="e187e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e187e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e187e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e187e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e187e-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="e187e-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="e187e-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e187e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e187e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e187e-114">Not supported.</span></span> |
| <span data-ttu-id="e187e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e187e-115">Application</span></span>                            | <span data-ttu-id="e187e-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="e187e-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="e187e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e187e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/claimsMappingPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e187e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e187e-118">Request headers</span></span>

| <span data-ttu-id="e187e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e187e-119">Name</span></span>       | <span data-ttu-id="e187e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e187e-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e187e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e187e-121">Authorization</span></span> | <span data-ttu-id="e187e-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="e187e-122">Bearer {token}</span></span> |
| <span data-ttu-id="e187e-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="e187e-123">Content-type</span></span> | <span data-ttu-id="e187e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e187e-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e187e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e187e-125">Request body</span></span>

<span data-ttu-id="e187e-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="e187e-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e187e-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="e187e-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e187e-128">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e187e-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e187e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e187e-129">Property</span></span>     | <span data-ttu-id="e187e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e187e-130">Type</span></span>        | <span data-ttu-id="e187e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e187e-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e187e-132">definir</span><span class="sxs-lookup"><span data-stu-id="e187e-132">definition</span></span>|<span data-ttu-id="e187e-133">Coleção String</span><span class="sxs-lookup"><span data-stu-id="e187e-133">String collection</span></span>| <span data-ttu-id="e187e-134">Uma coleção de cadeia de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações da política.</span><span class="sxs-lookup"><span data-stu-id="e187e-134">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="e187e-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e187e-135">Required.</span></span>|
|<span data-ttu-id="e187e-136">description</span><span class="sxs-lookup"><span data-stu-id="e187e-136">description</span></span>|<span data-ttu-id="e187e-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e187e-137">String</span></span>| <span data-ttu-id="e187e-138">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="e187e-138">Description for this policy.</span></span>|
|<span data-ttu-id="e187e-139">displayName</span><span class="sxs-lookup"><span data-stu-id="e187e-139">displayName</span></span>|<span data-ttu-id="e187e-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e187e-140">String</span></span>| <span data-ttu-id="e187e-141">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="e187e-141">Display name for this policy.</span></span> <span data-ttu-id="e187e-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e187e-142">Required.</span></span>|
|<span data-ttu-id="e187e-143">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="e187e-143">isOrganizationDefault</span></span>|<span data-ttu-id="e187e-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="e187e-144">Boolean</span></span>|<span data-ttu-id="e187e-145">Se definido como true, ativa esta política.</span><span class="sxs-lookup"><span data-stu-id="e187e-145">If set to true, activates this policy.</span></span> <span data-ttu-id="e187e-146">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como a organização padrão.</span><span class="sxs-lookup"><span data-stu-id="e187e-146">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="e187e-147">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="e187e-147">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="e187e-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="e187e-148">Response</span></span>

<span data-ttu-id="e187e-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e187e-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e187e-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e187e-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="e187e-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e187e-152">Request</span></span>

<span data-ttu-id="e187e-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e187e-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e187e-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="e187e-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_claimsmappingpolicy"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/{id}
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
# <a name="javascript"></a>[<span data-ttu-id="e187e-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e187e-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-claimsmappingpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e187e-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e187e-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-claimsmappingpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e187e-157">Java</span><span class="sxs-lookup"><span data-stu-id="e187e-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-claimsmappingpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e187e-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="e187e-158">Response</span></span>

<span data-ttu-id="e187e-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e187e-159">The following is an example of the response.</span></span>

> <span data-ttu-id="e187e-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e187e-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsMappingPolicy"
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
  "description": "Update claimsmappingpolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

