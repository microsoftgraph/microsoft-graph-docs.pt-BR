---
title: Excluir um userflowidentityproviders
description: Exclua um identityProvider de um b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 4ad44addce58e8f18c0b6d582f0fd6f821cfc1c5
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401043"
---
# <a name="delete-a-userflowidentityproviders"></a><span data-ttu-id="16d0a-103">Excluir um userflowidentityproviders</span><span class="sxs-lookup"><span data-stu-id="16d0a-103">Delete a userflowidentityproviders</span></span>

<span data-ttu-id="16d0a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16d0a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16d0a-105">Exclua um provedor de identidade de um [objeto b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="16d0a-105">Delete an identity provider from a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span> <span data-ttu-id="16d0a-106">Para obter mais informações sobre provedores de identidade disponíveis para fluxos de usuários, consulte a referência da API [identityProviders.](../resources/identityproviderbase.md)</span><span class="sxs-lookup"><span data-stu-id="16d0a-106">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityproviderbase.md) API reference.</span></span>

## <a name="permissions"></a><span data-ttu-id="16d0a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="16d0a-107">Permissions</span></span>

<span data-ttu-id="16d0a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16d0a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16d0a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16d0a-110">Permission type</span></span>      | <span data-ttu-id="16d0a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="16d0a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16d0a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16d0a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="16d0a-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16d0a-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="16d0a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16d0a-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="16d0a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16d0a-115">Not supported.</span></span>|
|<span data-ttu-id="16d0a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16d0a-116">Application</span></span>| <span data-ttu-id="16d0a-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16d0a-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="16d0a-118">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="16d0a-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="16d0a-119">Administrador global</span><span class="sxs-lookup"><span data-stu-id="16d0a-119">Global administrator</span></span>
* <span data-ttu-id="16d0a-120">Administrador de fluxo de usuário de ID externa</span><span class="sxs-lookup"><span data-stu-id="16d0a-120">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="16d0a-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16d0a-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/b2cUserFlows/{userflow-id}/userflowIdentityProviders/{identityProvider-id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="16d0a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16d0a-122">Request headers</span></span>

|<span data-ttu-id="16d0a-123">Nome</span><span class="sxs-lookup"><span data-stu-id="16d0a-123">Name</span></span>|<span data-ttu-id="16d0a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="16d0a-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="16d0a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="16d0a-125">Authorization</span></span>|<span data-ttu-id="16d0a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16d0a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="16d0a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16d0a-128">Request body</span></span>

<span data-ttu-id="16d0a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="16d0a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16d0a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="16d0a-130">Response</span></span>

<span data-ttu-id="16d0a-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="16d0a-131">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="16d0a-132">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="16d0a-132">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="16d0a-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="16d0a-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="16d0a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16d0a-134">Request</span></span>

<span data-ttu-id="16d0a-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="16d0a-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows_userflowIdentityProviders"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_test_signin_signup/userflowIdentityProviders/MSA-OIDC/$ref
```

### <a name="response"></a><span data-ttu-id="16d0a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="16d0a-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
