---
title: Excluir identityProvider de um b2cIdentityUserFlow (preterido)
description: Exclua um identityProvider de um b2cIdentityUserFlow. (preterido)
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: a6d825cd474a38176256e0e18dd6b77d1345a64b
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53400989"
---
# <a name="delete-an-identityprovider-from-a-b2cidentityuserflow-deprecated"></a><span data-ttu-id="67ca4-104">Excluir um identityProvider de um b2cIdentityUserFlow (preterido)</span><span class="sxs-lookup"><span data-stu-id="67ca4-104">Delete an identityProvider from a b2cIdentityUserFlow (deprecated)</span></span>

<span data-ttu-id="67ca4-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67ca4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="67ca4-106">Exclua um provedor de identidade de um [objeto b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="67ca4-106">Delete an identity provider from a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span> <span data-ttu-id="67ca4-107">Para obter mais informações sobre provedores de identidade disponíveis para fluxos de usuários, consulte a referência da API [identityProviders.](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="67ca4-107">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityprovider.md) API reference.</span></span>

## <a name="permissions"></a><span data-ttu-id="67ca4-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="67ca4-108">Permissions</span></span>

<span data-ttu-id="67ca4-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67ca4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67ca4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67ca4-111">Permission type</span></span>      | <span data-ttu-id="67ca4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="67ca4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67ca4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67ca4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="67ca4-114">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67ca4-114">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="67ca4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67ca4-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="67ca4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67ca4-116">Not supported.</span></span>|
|<span data-ttu-id="67ca4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67ca4-117">Application</span></span>| <span data-ttu-id="67ca4-118">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67ca4-118">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="67ca4-119">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="67ca4-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="67ca4-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="67ca4-120">Global administrator</span></span>
* <span data-ttu-id="67ca4-121">Administrador de identidade externa Flow usuário</span><span class="sxs-lookup"><span data-stu-id="67ca4-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="67ca4-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67ca4-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/b2cUserFlows/{id}/identityProviders/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="67ca4-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67ca4-123">Request headers</span></span>

|<span data-ttu-id="67ca4-124">Nome</span><span class="sxs-lookup"><span data-stu-id="67ca4-124">Name</span></span>|<span data-ttu-id="67ca4-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="67ca4-125">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="67ca4-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="67ca4-126">Authorization</span></span>|<span data-ttu-id="67ca4-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67ca4-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="67ca4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67ca4-129">Request body</span></span>

<span data-ttu-id="67ca4-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="67ca4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67ca4-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="67ca4-131">Response</span></span>

<span data-ttu-id="67ca4-132">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="67ca4-132">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="67ca4-133">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="67ca4-133">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="67ca4-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67ca4-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="67ca4-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67ca4-135">Request</span></span>

<span data-ttu-id="67ca4-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="67ca4-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_identityProviders_1"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/identityProviders/Facebook-OAUTH/$ref
```

### <a name="response"></a><span data-ttu-id="67ca4-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="67ca4-137">Response</span></span>

<span data-ttu-id="67ca4-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="67ca4-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
