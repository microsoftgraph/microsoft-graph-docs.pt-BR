---
title: Atualizar claimsmappingpolicy
description: Atualize as propriedades do objeto claimsMappingPolicy.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f5434c73f7942a87babe21170bb2d82ca9f15c76
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846194"
---
# <a name="update-claimsmappingpolicy"></a><span data-ttu-id="b5ff5-103">Atualizar claimsmappingpolicy</span><span class="sxs-lookup"><span data-stu-id="b5ff5-103">Update claimsmappingpolicy</span></span>

<span data-ttu-id="b5ff5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5ff5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b5ff5-105">Atualiza as propriedades de um objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="b5ff5-105">Update the properties of a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5ff5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b5ff5-106">Permissions</span></span>

<span data-ttu-id="b5ff5-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="b5ff5-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b5ff5-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5ff5-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b5ff5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5ff5-109">Permission type</span></span>                        | <span data-ttu-id="b5ff5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b5ff5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b5ff5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5ff5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b5ff5-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="b5ff5-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="b5ff5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5ff5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5ff5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5ff5-114">Not supported.</span></span> |
| <span data-ttu-id="b5ff5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5ff5-115">Application</span></span>                            | <span data-ttu-id="b5ff5-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="b5ff5-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5ff5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5ff5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/claimsMappingPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b5ff5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5ff5-118">Request headers</span></span>

| <span data-ttu-id="b5ff5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b5ff5-119">Name</span></span>       | <span data-ttu-id="b5ff5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5ff5-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b5ff5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5ff5-121">Authorization</span></span> | <span data-ttu-id="b5ff5-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="b5ff5-122">Bearer {token}</span></span> |
| <span data-ttu-id="b5ff5-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="b5ff5-123">Content-type</span></span> | <span data-ttu-id="b5ff5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b5ff5-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5ff5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5ff5-125">Request body</span></span>

<span data-ttu-id="b5ff5-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="b5ff5-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b5ff5-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="b5ff5-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b5ff5-128">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b5ff5-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b5ff5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b5ff5-129">Property</span></span>     | <span data-ttu-id="b5ff5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5ff5-130">Type</span></span>        | <span data-ttu-id="b5ff5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5ff5-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b5ff5-132">definir</span><span class="sxs-lookup"><span data-stu-id="b5ff5-132">definition</span></span>|<span data-ttu-id="b5ff5-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5ff5-133">String collection</span></span>| <span data-ttu-id="b5ff5-134">Uma coleção de cadeia de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações da política.</span><span class="sxs-lookup"><span data-stu-id="b5ff5-134">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="b5ff5-135">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5ff5-135">Required.</span></span>|
|<span data-ttu-id="b5ff5-136">description</span><span class="sxs-lookup"><span data-stu-id="b5ff5-136">description</span></span>|<span data-ttu-id="b5ff5-137">String</span><span class="sxs-lookup"><span data-stu-id="b5ff5-137">String</span></span>| <span data-ttu-id="b5ff5-138">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="b5ff5-138">Description for this policy.</span></span>|
|<span data-ttu-id="b5ff5-139">displayName</span><span class="sxs-lookup"><span data-stu-id="b5ff5-139">displayName</span></span>|<span data-ttu-id="b5ff5-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5ff5-140">String</span></span>| <span data-ttu-id="b5ff5-141">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="b5ff5-141">Display name for this policy.</span></span> <span data-ttu-id="b5ff5-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5ff5-142">Required.</span></span>|
|<span data-ttu-id="b5ff5-143">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="b5ff5-143">isOrganizationDefault</span></span>|<span data-ttu-id="b5ff5-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="b5ff5-144">Boolean</span></span>|<span data-ttu-id="b5ff5-145">Se definido como true, ativa esta política.</span><span class="sxs-lookup"><span data-stu-id="b5ff5-145">If set to true, activates this policy.</span></span> <span data-ttu-id="b5ff5-146">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como a organização padrão.</span><span class="sxs-lookup"><span data-stu-id="b5ff5-146">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="b5ff5-147">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="b5ff5-147">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="b5ff5-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5ff5-148">Response</span></span>

<span data-ttu-id="b5ff5-149">If successful, this method returns a `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="b5ff5-149">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="b5ff5-150">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="b5ff5-150">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5ff5-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5ff5-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5ff5-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5ff5-152">Request</span></span>

<span data-ttu-id="b5ff5-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5ff5-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b5ff5-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5ff5-154">HTTP</span></span>](#tab/http)
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

### <a name="response"></a><span data-ttu-id="b5ff5-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5ff5-155">Response</span></span>

<span data-ttu-id="b5ff5-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b5ff5-156">The following is an example of the response.</span></span>

> <span data-ttu-id="b5ff5-157">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="b5ff5-157">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b5ff5-158">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="b5ff5-158">All the properties will be returned from an actual call.</span></span>

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
