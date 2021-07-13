---
title: Excluir identityProvider de b2xIdentityUserFlow (preterido)
description: Exclua um identityProvider de um b2xIdentityUserFlow. (preterido)
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 94310d9c4ffa629638721fd248866ab685b8f506
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53400947"
---
# <a name="delete-identityprovider-from-b2xidentityuserflow-deprecated"></a><span data-ttu-id="8319b-104">Excluir identityProvider de b2xIdentityUserFlow (preterido)</span><span class="sxs-lookup"><span data-stu-id="8319b-104">Delete identityProvider from b2xIdentityUserFlow (deprecated)</span></span>

<span data-ttu-id="8319b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8319b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="8319b-106">Exclua um provedor de identidade de um [objeto b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="8319b-106">Delete an identity provider from a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span> <span data-ttu-id="8319b-107">Para fluxos de usuários de autoatendados, os valores podem ser `Google-OAUTH` ou `Facebook-OAUTH` .</span><span class="sxs-lookup"><span data-stu-id="8319b-107">For self-service sign up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="permissions"></a><span data-ttu-id="8319b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="8319b-108">Permissions</span></span>

<span data-ttu-id="8319b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8319b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8319b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8319b-111">Permission type</span></span>      | <span data-ttu-id="8319b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8319b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8319b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8319b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8319b-114">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8319b-114">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="8319b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8319b-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="8319b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8319b-116">Not supported.</span></span>|
|<span data-ttu-id="8319b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8319b-117">Application</span></span>| <span data-ttu-id="8319b-118">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8319b-118">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="8319b-119">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="8319b-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="8319b-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="8319b-120">Global administrator</span></span>
* <span data-ttu-id="8319b-121">Administrador de identidade externa Flow usuário</span><span class="sxs-lookup"><span data-stu-id="8319b-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="8319b-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8319b-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/b2xUserFlows/{id}/identityProviders/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="8319b-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8319b-123">Request headers</span></span>

|<span data-ttu-id="8319b-124">Nome</span><span class="sxs-lookup"><span data-stu-id="8319b-124">Name</span></span>|<span data-ttu-id="8319b-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="8319b-125">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="8319b-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="8319b-126">Authorization</span></span>|<span data-ttu-id="8319b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8319b-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8319b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8319b-129">Request body</span></span>

<span data-ttu-id="8319b-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8319b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8319b-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8319b-131">Response</span></span>

<span data-ttu-id="8319b-132">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8319b-132">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="8319b-133">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="8319b-133">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="8319b-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8319b-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="8319b-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8319b-135">Request</span></span>

<span data-ttu-id="8319b-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8319b-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_identityProviders_2"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_PartnerSignUp/identityProviders/Facebook-OAUTH/$ref
```

### <a name="response"></a><span data-ttu-id="8319b-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="8319b-137">Response</span></span>

<span data-ttu-id="8319b-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8319b-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
