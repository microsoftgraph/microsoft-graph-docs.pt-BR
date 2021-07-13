---
title: Atualizar um userFlowIdentityProvider
description: Atualize um identityProvider em um b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 61b5ea598b6a82c9ecacf3610792164717b4a965
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401020"
---
# <a name="update-a-userflowidentityprovider"></a><span data-ttu-id="e3992-103">Atualizar um userFlowIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="e3992-103">Update a userFlowIdentityProvider</span></span>

<span data-ttu-id="e3992-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3992-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3992-105">Atualize um provedor de identidade em um [objeto b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="e3992-105">Update an identity providers in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3992-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e3992-106">Permissions</span></span>

<span data-ttu-id="e3992-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3992-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3992-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3992-109">Permission type</span></span>      | <span data-ttu-id="e3992-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e3992-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3992-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3992-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e3992-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3992-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="e3992-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3992-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e3992-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3992-114">Not supported.</span></span>|
|<span data-ttu-id="e3992-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3992-115">Application</span></span>| <span data-ttu-id="e3992-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3992-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="e3992-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="e3992-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="e3992-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="e3992-118">Global administrator</span></span>
* <span data-ttu-id="e3992-119">Administrador de fluxo de usuário de ID externa</span><span class="sxs-lookup"><span data-stu-id="e3992-119">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="e3992-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3992-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/b2xUserFlows/{userflow-id}/userflowIdentityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="e3992-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3992-121">Request headers</span></span>

|<span data-ttu-id="e3992-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e3992-122">Name</span></span>|<span data-ttu-id="e3992-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3992-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="e3992-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3992-124">Authorization</span></span>|<span data-ttu-id="e3992-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3992-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e3992-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e3992-127">Content-Type</span></span>|<span data-ttu-id="e3992-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3992-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3992-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3992-130">Request body</span></span>

<span data-ttu-id="e3992-131">No corpo da solicitação, forneça uma representação JSON com a `id` [identidadeProvider](../resources/identityproviderbase.md) que você deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="e3992-131">In the request body, provide a JSON representation with the `id` of the [identityProvider](../resources/identityproviderbase.md) you want to add.</span></span> <span data-ttu-id="e3992-132">Para fluxos de usuários de autoatendados, os valores podem ser `Google-OAUTH` ou `Facebook-OAUTH` .</span><span class="sxs-lookup"><span data-stu-id="e3992-132">For self-service sign up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="response"></a><span data-ttu-id="e3992-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3992-133">Response</span></span>

<span data-ttu-id="e3992-134">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e3992-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="e3992-135">Se não tiver êxito, `4xx` um erro será retornado com os detalhes de erro específicos.</span><span class="sxs-lookup"><span data-stu-id="e3992-135">If unsuccessful, a `4xx` error is returned with the specific error details.</span></span>

## <a name="example"></a><span data-ttu-id="e3992-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3992-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3992-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3992-137">Request</span></span>

<span data-ttu-id="e3992-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3992-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_b2xuserflows_userflowidentityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Test/userflowIdentityProviders/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/beta/identity/identityProviders/B2X_1_Test"
}
```

### <a name="response"></a><span data-ttu-id="e3992-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3992-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
