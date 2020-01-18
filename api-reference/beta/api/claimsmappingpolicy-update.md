---
title: Atualizar claimsmappingpolicy
description: Atualize as propriedades do objeto claimsMappingPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d59d9fc29dd7c48e4b65d9551a38b378d2860c89
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234080"
---
# <a name="update-claimsmappingpolicy"></a><span data-ttu-id="8d906-103">Atualizar claimsmappingpolicy</span><span class="sxs-lookup"><span data-stu-id="8d906-103">Update claimsmappingpolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d906-104">Atualiza as propriedades de um objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="8d906-104">Update the properties of a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d906-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8d906-105">Permissions</span></span>

<span data-ttu-id="8d906-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d906-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8d906-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d906-108">Permission type</span></span>                        | <span data-ttu-id="8d906-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8d906-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8d906-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d906-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8d906-111">Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d906-111">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="8d906-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d906-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d906-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d906-113">Not supported.</span></span> |
| <span data-ttu-id="8d906-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d906-114">Application</span></span>                            | <span data-ttu-id="8d906-115">Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d906-115">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d906-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d906-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/claimsMappingPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8d906-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d906-117">Request headers</span></span>

| <span data-ttu-id="8d906-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8d906-118">Name</span></span>       | <span data-ttu-id="8d906-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d906-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8d906-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d906-120">Authorization</span></span> | <span data-ttu-id="8d906-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="8d906-121">Bearer {token}</span></span> |
| <span data-ttu-id="8d906-122">Content-type</span><span class="sxs-lookup"><span data-stu-id="8d906-122">Content-type</span></span> | <span data-ttu-id="8d906-123">application/json</span><span class="sxs-lookup"><span data-stu-id="8d906-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d906-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d906-124">Request body</span></span>

<span data-ttu-id="8d906-125">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="8d906-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8d906-126">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="8d906-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8d906-127">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="8d906-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8d906-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d906-128">Property</span></span>     | <span data-ttu-id="8d906-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d906-129">Type</span></span>        | <span data-ttu-id="8d906-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d906-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8d906-131">definir</span><span class="sxs-lookup"><span data-stu-id="8d906-131">definition</span></span>|<span data-ttu-id="8d906-132">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d906-132">String collection</span></span>| <span data-ttu-id="8d906-133">Uma coleção de cadeia de caracteres que contém uma cadeia de caracteres JSON que define as regras e as configurações da política.</span><span class="sxs-lookup"><span data-stu-id="8d906-133">A string collection containing a JSON string that defines the rules and settings for this policy.</span></span>  <span data-ttu-id="8d906-134">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d906-134">Required.</span></span>|
|<span data-ttu-id="8d906-135">description</span><span class="sxs-lookup"><span data-stu-id="8d906-135">description</span></span>|<span data-ttu-id="8d906-136">String</span><span class="sxs-lookup"><span data-stu-id="8d906-136">String</span></span>| <span data-ttu-id="8d906-137">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="8d906-137">Description for this policy.</span></span>|
|<span data-ttu-id="8d906-138">displayName</span><span class="sxs-lookup"><span data-stu-id="8d906-138">displayName</span></span>|<span data-ttu-id="8d906-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d906-139">String</span></span>| <span data-ttu-id="8d906-140">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="8d906-140">Display name for this policy.</span></span> <span data-ttu-id="8d906-141">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d906-141">Required.</span></span>|
|<span data-ttu-id="8d906-142">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="8d906-142">isOrganizationDefault</span></span>|<span data-ttu-id="8d906-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d906-143">Boolean</span></span>|<span data-ttu-id="8d906-144">Se definido como true, ativa esta política.</span><span class="sxs-lookup"><span data-stu-id="8d906-144">If set to true, activates this policy.</span></span> <span data-ttu-id="8d906-145">Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como a organização padrão.</span><span class="sxs-lookup"><span data-stu-id="8d906-145">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="8d906-146">Opcional, o valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="8d906-146">Optional, default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="8d906-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d906-147">Response</span></span>

<span data-ttu-id="8d906-p106">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d906-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d906-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d906-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d906-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d906-151">Request</span></span>

<span data-ttu-id="8d906-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d906-152">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_claimsmappingpolicy"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/claimsMappingPolicies/{id}
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

### <a name="response"></a><span data-ttu-id="8d906-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d906-153">Response</span></span>

<span data-ttu-id="8d906-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8d906-154">The following is an example of the response.</span></span>

> <span data-ttu-id="8d906-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8d906-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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