---
title: Excluir identityProvider de b2xIdentityUserFlow
description: Exclua um identityProvider de um b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: eb37182bf72d2e1609c3077df5e4c3a1df4a618e
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882864"
---
# <a name="delete-identityprovider-from-b2xidentityuserflow"></a><span data-ttu-id="9f58f-103">Excluir identityProvider de b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="9f58f-103">Delete identityProvider from b2xIdentityUserFlow</span></span>

<span data-ttu-id="9f58f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f58f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9f58f-105">Exclua um provedor de identidade de um [objeto b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="9f58f-105">Delete an identity provider from a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span> <span data-ttu-id="9f58f-106">Para fluxos de usuário de entrada de autoatendados, os valores podem `Google-OAUTH` ser ou `Facebook-OAUTH` .</span><span class="sxs-lookup"><span data-stu-id="9f58f-106">For self-service sign-up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f58f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9f58f-107">Permissions</span></span>

<span data-ttu-id="9f58f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f58f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f58f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f58f-110">Permission type</span></span>      | <span data-ttu-id="9f58f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9f58f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f58f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f58f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9f58f-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f58f-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="9f58f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f58f-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="9f58f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f58f-115">Not supported.</span></span>|
|<span data-ttu-id="9f58f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f58f-116">Application</span></span>| <span data-ttu-id="9f58f-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f58f-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="9f58f-118">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="9f58f-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="9f58f-119">Administrador global</span><span class="sxs-lookup"><span data-stu-id="9f58f-119">Global administrator</span></span>
* <span data-ttu-id="9f58f-120">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="9f58f-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="9f58f-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f58f-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/b2xUserFlows/{id}/identityProviders/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="9f58f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f58f-122">Request headers</span></span>

|<span data-ttu-id="9f58f-123">Nome</span><span class="sxs-lookup"><span data-stu-id="9f58f-123">Name</span></span>|<span data-ttu-id="9f58f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f58f-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="9f58f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f58f-125">Authorization</span></span>|<span data-ttu-id="9f58f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f58f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f58f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f58f-128">Request body</span></span>

<span data-ttu-id="9f58f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9f58f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f58f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f58f-130">Response</span></span>

<span data-ttu-id="9f58f-131">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9f58f-131">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="9f58f-132">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="9f58f-132">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="9f58f-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9f58f-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f58f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f58f-134">Request</span></span>

<span data-ttu-id="9f58f-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f58f-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_identityProviders_2"
}
-->

``` http
DELETE https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_PartnerSignUp/identityProviders/Facebook-OAUTH/$ref
```

### <a name="response"></a><span data-ttu-id="9f58f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f58f-136">Response</span></span>

<span data-ttu-id="9f58f-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9f58f-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
