---
title: Atualizar identitySecurityDefaultsEnforcementPolicy
description: Atualiza as propriedades de um objeto identitySecurityDefaultsEnforcementPolicy.
localization_priority: Normal
author: rohinigoyal1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bf4566e08a07147144993c7b17cacbd22890c54e
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384315"
---
# <a name="update-identitysecuritydefaultsenforcementpolicy"></a><span data-ttu-id="50874-103">Atualizar identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="50874-103">Update identitySecurityDefaultsEnforcementPolicy</span></span>

<span data-ttu-id="50874-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50874-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50874-105">Atualiza as propriedades de um objeto [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="50874-105">Update the properties of an [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="50874-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="50874-106">Permissions</span></span>

<span data-ttu-id="50874-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50874-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="50874-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50874-109">Permission type</span></span>                        | <span data-ttu-id="50874-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="50874-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="50874-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50874-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="50874-112">Policy. Read. All e Policy. ReadWrite. ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="50874-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="50874-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50874-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50874-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50874-114">Not supported.</span></span> |
| <span data-ttu-id="50874-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50874-115">Application</span></span>                            | <span data-ttu-id="50874-116">Policy. Read. All e Policy. ReadWrite. ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="50874-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="50874-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50874-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/identitySecurityDefaultsEnforcementPolicy
```

## <a name="request-headers"></a><span data-ttu-id="50874-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50874-118">Request headers</span></span>

| <span data-ttu-id="50874-119">Nome</span><span class="sxs-lookup"><span data-stu-id="50874-119">Name</span></span>       | <span data-ttu-id="50874-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="50874-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="50874-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="50874-121">Authorization</span></span> | <span data-ttu-id="50874-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50874-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="50874-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="50874-124">Content-type</span></span> | <span data-ttu-id="50874-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50874-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50874-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50874-127">Request body</span></span>

<span data-ttu-id="50874-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="50874-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="50874-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="50874-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="50874-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="50874-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="50874-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50874-131">Property</span></span>     | <span data-ttu-id="50874-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="50874-132">Type</span></span>        | <span data-ttu-id="50874-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="50874-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="50874-134">isEnabled</span><span class="sxs-lookup"><span data-stu-id="50874-134">isEnabled</span></span>|<span data-ttu-id="50874-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="50874-135">Boolean</span></span>|<span data-ttu-id="50874-136">Se definido como true, os padrões de segurança do Active Directory do Azure são habilitados para o locatário.</span><span class="sxs-lookup"><span data-stu-id="50874-136">If set to true, Azure Active Directory security defaults is enabled for the tenant.</span></span>|

## <a name="response"></a><span data-ttu-id="50874-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="50874-137">Response</span></span>

<span data-ttu-id="50874-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50874-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="50874-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="50874-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="50874-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50874-141">Request</span></span>

<span data-ttu-id="50874-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="50874-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="50874-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="50874-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_identitysecuritydefaultsenforcementpolicy"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/identitySecurityDefaultsEnforcementPolicy
Content-type: application/json

{
  "isEnabled": false
}
```
# <a name="c"></a>[<span data-ttu-id="50874-144">C#</span><span class="sxs-lookup"><span data-stu-id="50874-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-identitysecuritydefaultsenforcementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="50874-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50874-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-identitysecuritydefaultsenforcementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="50874-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50874-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-identitysecuritydefaultsenforcementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="50874-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="50874-147">Response</span></span>

<span data-ttu-id="50874-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="50874-148">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identitySecurityDefaultsEnforcementPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update identitysecuritydefaultsenforcementpolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
