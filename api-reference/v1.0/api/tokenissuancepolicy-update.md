---
title: Atualizar tokenIssuancePolicy
description: Atualize as propriedades do objeto tokenIssuancePolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ce5b85d6a0766d0e62363d1b36cc3dd539db7088
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229658"
---
# <a name="update-tokenissuancepolicy"></a><span data-ttu-id="696a9-103">Atualizar tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="696a9-103">Update tokenIssuancePolicy</span></span>

<span data-ttu-id="696a9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="696a9-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="696a9-105">Atualiza as propriedades de um objeto [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="696a9-105">Update the properties of a [tokenIssuancePolicy](../resources/tokenIssuancePolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="696a9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="696a9-106">Permissions</span></span>

<span data-ttu-id="696a9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="696a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="696a9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="696a9-109">Permission type</span></span>                        | <span data-ttu-id="696a9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="696a9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="696a9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="696a9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="696a9-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="696a9-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="696a9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="696a9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="696a9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="696a9-114">Not supported.</span></span> |
| <span data-ttu-id="696a9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="696a9-115">Application</span></span>                            | <span data-ttu-id="696a9-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="696a9-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="696a9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="696a9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/tokenIssuancePolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="696a9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="696a9-118">Request headers</span></span>

| <span data-ttu-id="696a9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="696a9-119">Name</span></span>       | <span data-ttu-id="696a9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="696a9-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="696a9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="696a9-121">Authorization</span></span> | <span data-ttu-id="696a9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="696a9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="696a9-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="696a9-124">Content-type</span></span> | <span data-ttu-id="696a9-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="696a9-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="696a9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="696a9-127">Request body</span></span>

<span data-ttu-id="696a9-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="696a9-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="696a9-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="696a9-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="696a9-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="696a9-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="696a9-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="696a9-131">Property</span></span>     | <span data-ttu-id="696a9-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="696a9-132">Type</span></span>        | <span data-ttu-id="696a9-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="696a9-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="696a9-134">definir</span><span class="sxs-lookup"><span data-stu-id="696a9-134">definition</span></span>|<span data-ttu-id="696a9-135">String collection</span><span class="sxs-lookup"><span data-stu-id="696a9-135">String collection</span></span>| <span data-ttu-id="696a9-136">Uma coleção de cadeia de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações da política.</span><span class="sxs-lookup"><span data-stu-id="696a9-136">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="696a9-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="696a9-137">Required.</span></span>|
|<span data-ttu-id="696a9-138">description</span><span class="sxs-lookup"><span data-stu-id="696a9-138">description</span></span>|<span data-ttu-id="696a9-139">String</span><span class="sxs-lookup"><span data-stu-id="696a9-139">String</span></span>| <span data-ttu-id="696a9-140">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="696a9-140">Description for this policy.</span></span>|
|<span data-ttu-id="696a9-141">displayName</span><span class="sxs-lookup"><span data-stu-id="696a9-141">displayName</span></span>|<span data-ttu-id="696a9-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="696a9-142">String</span></span>| <span data-ttu-id="696a9-143">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="696a9-143">Display name for this policy.</span></span> <span data-ttu-id="696a9-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="696a9-144">Required.</span></span>|
|<span data-ttu-id="696a9-145">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="696a9-145">isOrganizationDefault</span></span>|<span data-ttu-id="696a9-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="696a9-146">Boolean</span></span>|<span data-ttu-id="696a9-147">Se definido como true, ativa esta política.</span><span class="sxs-lookup"><span data-stu-id="696a9-147">If set to true, activates this policy.</span></span> <span data-ttu-id="696a9-148">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como a organização padrão.</span><span class="sxs-lookup"><span data-stu-id="696a9-148">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="696a9-149">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="696a9-149">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="696a9-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="696a9-150">Response</span></span>

<span data-ttu-id="696a9-p108">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="696a9-p108">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="696a9-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="696a9-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="696a9-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="696a9-154">Request</span></span>

<span data-ttu-id="696a9-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="696a9-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_tokenissuancepolicy"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/tokenIssuancePolicies/{id}
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

### <a name="response"></a><span data-ttu-id="696a9-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="696a9-156">Response</span></span>

<span data-ttu-id="696a9-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="696a9-157">The following is an example of the response.</span></span>

> <span data-ttu-id="696a9-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="696a9-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
