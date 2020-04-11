---
title: Atualizar homerealmdiscoverypolicy
description: Atualize as propriedades do objeto homeRealmDiscoveryPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 749ba53714ec49e38012e14afa09b63df49c4a65
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227747"
---
# <a name="update-homerealmdiscoverypolicy"></a><span data-ttu-id="1c416-103">Atualizar homerealmdiscoverypolicy</span><span class="sxs-lookup"><span data-stu-id="1c416-103">Update homerealmdiscoverypolicy</span></span>

<span data-ttu-id="1c416-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c416-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="1c416-105">Atualiza as propriedades de um objeto [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="1c416-105">Update the properties of a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c416-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1c416-106">Permissions</span></span>

<span data-ttu-id="1c416-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c416-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1c416-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c416-109">Permission type</span></span>                        | <span data-ttu-id="1c416-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1c416-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1c416-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c416-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1c416-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c416-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="1c416-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c416-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c416-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c416-114">Not supported.</span></span> |
| <span data-ttu-id="1c416-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c416-115">Application</span></span>                            | <span data-ttu-id="1c416-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c416-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c416-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c416-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/homeRealmDiscoveryPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1c416-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c416-118">Request headers</span></span>

| <span data-ttu-id="1c416-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1c416-119">Name</span></span>       | <span data-ttu-id="1c416-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c416-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1c416-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c416-121">Authorization</span></span> | <span data-ttu-id="1c416-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c416-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1c416-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="1c416-124">Content-type</span></span> | <span data-ttu-id="1c416-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c416-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c416-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c416-127">Request body</span></span>

<span data-ttu-id="1c416-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="1c416-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="1c416-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="1c416-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1c416-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="1c416-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1c416-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1c416-131">Property</span></span>     | <span data-ttu-id="1c416-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c416-132">Type</span></span>        | <span data-ttu-id="1c416-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c416-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1c416-134">definir</span><span class="sxs-lookup"><span data-stu-id="1c416-134">definition</span></span>|<span data-ttu-id="1c416-135">String collection</span><span class="sxs-lookup"><span data-stu-id="1c416-135">String collection</span></span>| <span data-ttu-id="1c416-136">Uma coleção de cadeia de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações da política.</span><span class="sxs-lookup"><span data-stu-id="1c416-136">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="1c416-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c416-137">Required.</span></span>|
|<span data-ttu-id="1c416-138">description</span><span class="sxs-lookup"><span data-stu-id="1c416-138">description</span></span>|<span data-ttu-id="1c416-139">String</span><span class="sxs-lookup"><span data-stu-id="1c416-139">String</span></span>| <span data-ttu-id="1c416-140">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="1c416-140">Description for this policy.</span></span>|
|<span data-ttu-id="1c416-141">displayName</span><span class="sxs-lookup"><span data-stu-id="1c416-141">displayName</span></span>|<span data-ttu-id="1c416-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c416-142">String</span></span>| <span data-ttu-id="1c416-143">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="1c416-143">Display name for this policy.</span></span> <span data-ttu-id="1c416-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c416-144">Required.</span></span>|
|<span data-ttu-id="1c416-145">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="1c416-145">isOrganizationDefault</span></span>|<span data-ttu-id="1c416-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c416-146">Boolean</span></span>|<span data-ttu-id="1c416-147">Se definido como true, ativa esta política.</span><span class="sxs-lookup"><span data-stu-id="1c416-147">If set to true, activates this policy.</span></span> <span data-ttu-id="1c416-148">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como a organização padrão.</span><span class="sxs-lookup"><span data-stu-id="1c416-148">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="1c416-149">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="1c416-149">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="1c416-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c416-150">Response</span></span>

<span data-ttu-id="1c416-p108">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c416-p108">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c416-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c416-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c416-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c416-154">Request</span></span>

<span data-ttu-id="1c416-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c416-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_homerealmdiscoverypolicy"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies/{id}
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

### <a name="response"></a><span data-ttu-id="1c416-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c416-156">Response</span></span>

<span data-ttu-id="1c416-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1c416-157">The following is an example of the response.</span></span>

> <span data-ttu-id="1c416-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c416-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
