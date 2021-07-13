---
title: Adicionar identityProvider a um b2cIdentityUserFlow (preterido)
description: Adicione identityProvider a um b2cIdentityUserFlow. (preterido)
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 9b213dd0255984b0ffe99270ec5fa7f69558aabb
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53400961"
---
# <a name="add-identityprovider-to-a-b2cidentityuserflow-deprecated"></a><span data-ttu-id="4f469-104">Adicionar identityProvider a um b2cIdentityUserFlow (preterido)</span><span class="sxs-lookup"><span data-stu-id="4f469-104">Add identityProvider to a b2cIdentityUserFlow (deprecated)</span></span>

<span data-ttu-id="4f469-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f469-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="4f469-106">Adicione provedores de identidade em um [objeto b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="4f469-106">Add identity providers in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f469-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="4f469-107">Permissions</span></span>

<span data-ttu-id="4f469-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f469-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f469-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f469-110">Permission type</span></span>      | <span data-ttu-id="4f469-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4f469-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f469-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f469-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4f469-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f469-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="4f469-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f469-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="4f469-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f469-115">Not supported.</span></span>|
|<span data-ttu-id="4f469-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f469-116">Application</span></span>| <span data-ttu-id="4f469-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f469-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="4f469-118">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="4f469-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="4f469-119">Administrador global</span><span class="sxs-lookup"><span data-stu-id="4f469-119">Global administrator</span></span>
* <span data-ttu-id="4f469-120">Administrador de identidade externa Flow usuário</span><span class="sxs-lookup"><span data-stu-id="4f469-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="4f469-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f469-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2cUserFlows/{id}/identityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="4f469-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f469-122">Request headers</span></span>

|<span data-ttu-id="4f469-123">Nome</span><span class="sxs-lookup"><span data-stu-id="4f469-123">Name</span></span>|<span data-ttu-id="4f469-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f469-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="4f469-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f469-125">Authorization</span></span>|<span data-ttu-id="4f469-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f469-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4f469-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4f469-128">Content-Type</span></span>|<span data-ttu-id="4f469-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f469-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f469-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f469-131">Request body</span></span>

<span data-ttu-id="4f469-132">No corpo da solicitação, forneça uma representação JSON da `id` [identidadeProvider](../resources/identityprovider.md) que você deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="4f469-132">In the request body, provide a JSON representation of the `id` of the [identityProvider](../resources/identityprovider.md) you want to add.</span></span> <span data-ttu-id="4f469-133">Para obter mais informações sobre provedores de identidade disponíveis para fluxos de usuários, consulte a referência da API [identityProviders.](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="4f469-133">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityprovider.md) API reference.</span></span>

## <a name="response"></a><span data-ttu-id="4f469-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f469-134">Response</span></span>

<span data-ttu-id="4f469-135">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4f469-135">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="4f469-136">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="4f469-136">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="4f469-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f469-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f469-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f469-138">Request</span></span>

<span data-ttu-id="4f469-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f469-139">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_b2cuserflows_identityprovider"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/identityProviders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/identityProviders/{id}"
}
```

### <a name="response"></a><span data-ttu-id="4f469-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f469-140">Response</span></span>

<span data-ttu-id="4f469-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4f469-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
