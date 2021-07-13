---
title: Adicionar um userFlowIdentityProvider
description: Adicione um identityProvider a um b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 3c30480e15b836a213a668e0948dcdb3436fbaf1
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401040"
---
# <a name="add-a-userflowidentityprovider"></a><span data-ttu-id="f1f44-103">Adicionar um userFlowIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="f1f44-103">Add a userFlowIdentityProvider</span></span>

<span data-ttu-id="f1f44-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1f44-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1f44-105">Adicione um provedor de identidade em um [objeto b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="f1f44-105">Add an identity providers in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1f44-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1f44-106">Permissions</span></span>

<span data-ttu-id="f1f44-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1f44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1f44-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1f44-109">Permission type</span></span>      | <span data-ttu-id="f1f44-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1f44-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1f44-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1f44-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f1f44-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1f44-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="f1f44-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1f44-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f1f44-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1f44-114">Not supported.</span></span>|
|<span data-ttu-id="f1f44-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1f44-115">Application</span></span>| <span data-ttu-id="f1f44-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1f44-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="f1f44-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="f1f44-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="f1f44-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="f1f44-118">Global administrator</span></span>
* <span data-ttu-id="f1f44-119">Administrador de fluxo de usuário de ID externa</span><span class="sxs-lookup"><span data-stu-id="f1f44-119">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="f1f44-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1f44-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/b2cUserFlows/{userflow-id}/userflowIdentityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="f1f44-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1f44-121">Request headers</span></span>

|<span data-ttu-id="f1f44-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f1f44-122">Name</span></span>|<span data-ttu-id="f1f44-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1f44-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f1f44-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1f44-124">Authorization</span></span>|<span data-ttu-id="f1f44-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1f44-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f1f44-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f1f44-127">Content-Type</span></span>|<span data-ttu-id="f1f44-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1f44-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1f44-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1f44-130">Request body</span></span>

<span data-ttu-id="f1f44-131">No corpo da solicitação, forneça uma representação JSON com a `id` [identidadeProvider](../resources/identityproviderbase.md) que você deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="f1f44-131">In the request body, provide a JSON representation with the `id` of the [identityProvider](../resources/identityproviderbase.md) you want to add.</span></span> <span data-ttu-id="f1f44-132">Para obter mais informações sobre provedores de identidade disponíveis para fluxos de usuários, consulte o [recurso identityProviders.](../resources/identityproviderbase.md)</span><span class="sxs-lookup"><span data-stu-id="f1f44-132">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityproviderbase.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="f1f44-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1f44-133">Response</span></span>

<span data-ttu-id="f1f44-134">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f1f44-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="f1f44-135">Se não tiver êxito, `4xx` um erro será retornado com os detalhes de erro específicos.</span><span class="sxs-lookup"><span data-stu-id="f1f44-135">If unsuccessful, a `4xx` error is returned with the specific error details.</span></span>

## <a name="example"></a><span data-ttu-id="f1f44-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1f44-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1f44-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1f44-137">Request</span></span>

<span data-ttu-id="f1f44-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1f44-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_b2cuserflows_userflowIdentityProviders"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_test_signin_signup/userflowIdentityProviders/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/beta/identity/identityProviders/{id}"
}
```

### <a name="response"></a><span data-ttu-id="f1f44-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1f44-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
