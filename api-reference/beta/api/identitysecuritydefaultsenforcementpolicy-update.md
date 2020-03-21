---
title: Atualizar identitySecurityDefaultsEnforcementPolicy
description: Atualiza as propriedades de um objeto identitySecurityDefaultsEnforcementPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 48e6cfa2e8499632d8495b9fc77e8e154b53dcc8
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895470"
---
# <a name="update-identitysecuritydefaultsenforcementpolicy"></a><span data-ttu-id="5fbe0-103">Atualizar identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="5fbe0-103">Update identitySecurityDefaultsEnforcementPolicy</span></span>

<span data-ttu-id="5fbe0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fbe0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5fbe0-105">Atualiza as propriedades de um objeto [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="5fbe0-105">Update the properties of an [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5fbe0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5fbe0-106">Permissions</span></span>

<span data-ttu-id="5fbe0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5fbe0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5fbe0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5fbe0-109">Permission type</span></span>                        | <span data-ttu-id="5fbe0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5fbe0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5fbe0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5fbe0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5fbe0-112">Policy. ReadWrite. ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="5fbe0-112">Policy.Readwrite.ConditionalAccess</span></span> |
| <span data-ttu-id="5fbe0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5fbe0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5fbe0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5fbe0-114">Not supported.</span></span> |
| <span data-ttu-id="5fbe0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5fbe0-115">Application</span></span>                            | <span data-ttu-id="5fbe0-116">Policy. ReadWrite. ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="5fbe0-116">Policy.Readwrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="5fbe0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5fbe0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/identitySecurityDefaultsEnforcementPolicy
```

## <a name="request-headers"></a><span data-ttu-id="5fbe0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5fbe0-118">Request headers</span></span>

| <span data-ttu-id="5fbe0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5fbe0-119">Name</span></span>       | <span data-ttu-id="5fbe0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fbe0-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5fbe0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5fbe0-121">Authorization</span></span> | <span data-ttu-id="5fbe0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5fbe0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5fbe0-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="5fbe0-124">Content-type</span></span> | <span data-ttu-id="5fbe0-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5fbe0-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5fbe0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5fbe0-127">Request body</span></span>

<span data-ttu-id="5fbe0-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="5fbe0-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5fbe0-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="5fbe0-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5fbe0-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="5fbe0-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5fbe0-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5fbe0-131">Property</span></span>     | <span data-ttu-id="5fbe0-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="5fbe0-132">Type</span></span>        | <span data-ttu-id="5fbe0-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fbe0-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5fbe0-134">isEnabled</span><span class="sxs-lookup"><span data-stu-id="5fbe0-134">isEnabled</span></span>|<span data-ttu-id="5fbe0-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fbe0-135">Boolean</span></span>|<span data-ttu-id="5fbe0-136">Se definido como true, os padrões de segurança do Active Directory do Azure são habilitados para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5fbe0-136">If set to true, Azure Active Directory security defaults is enabled for the tenant.</span></span>|

## <a name="response"></a><span data-ttu-id="5fbe0-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fbe0-137">Response</span></span>

<span data-ttu-id="5fbe0-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5fbe0-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5fbe0-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5fbe0-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5fbe0-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5fbe0-141">Request</span></span>

<span data-ttu-id="5fbe0-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5fbe0-142">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5fbe0-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fbe0-143">Response</span></span>

<span data-ttu-id="5fbe0-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5fbe0-144">The following is an example of the response.</span></span>

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
