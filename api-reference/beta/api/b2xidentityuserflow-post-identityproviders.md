---
title: Adicionar identityProvider a um b2xIdentityUserFlow (preterido)
description: Adicione identityProvider em um b2xIdentityUserFlow (preterido).
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 60309219aa24ad4d2aee58b877a324ce1d32aa8b
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53400905"
---
# <a name="add-identityprovider-to-a-b2xidentityuserflow-deprecated"></a><span data-ttu-id="04325-103">Adicionar identityProvider a um b2xIdentityUserFlow (preterido)</span><span class="sxs-lookup"><span data-stu-id="04325-103">Add identityProvider to a b2xIdentityUserFlow (deprecated)</span></span>

<span data-ttu-id="04325-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04325-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="04325-105">Atualize os provedores de identidade em um [objeto b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="04325-105">Update the identity providers in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="04325-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="04325-106">Permissions</span></span>

<span data-ttu-id="04325-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04325-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04325-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04325-109">Permission type</span></span>      | <span data-ttu-id="04325-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="04325-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04325-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04325-111">Delegated (work or school account)</span></span>|<span data-ttu-id="04325-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04325-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="04325-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04325-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="04325-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04325-114">Not supported.</span></span>|
|<span data-ttu-id="04325-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04325-115">Application</span></span>| <span data-ttu-id="04325-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04325-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="04325-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="04325-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="04325-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="04325-118">Global administrator</span></span>
* <span data-ttu-id="04325-119">Administrador de identidade externa Flow usuário</span><span class="sxs-lookup"><span data-stu-id="04325-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="04325-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04325-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2xUserFlows/{id}/identityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="04325-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04325-121">Request headers</span></span>

|<span data-ttu-id="04325-122">Nome</span><span class="sxs-lookup"><span data-stu-id="04325-122">Name</span></span>|<span data-ttu-id="04325-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="04325-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="04325-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="04325-124">Authorization</span></span>|<span data-ttu-id="04325-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04325-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="04325-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="04325-127">Content-Type</span></span>|<span data-ttu-id="04325-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04325-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="04325-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04325-130">Request body</span></span>

<span data-ttu-id="04325-131">No corpo da solicitação, forneça uma representação JSON da `id` [identidadeProvider](../resources/identityprovider.md) que você deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="04325-131">In the request body, provide a JSON representation of the `id` of the [identityProvider](../resources/identityprovider.md) you want to add.</span></span> <span data-ttu-id="04325-132">Para fluxos de usuários de autoatendados, os valores podem ser `Google-OAUTH` ou `Facebook-OAUTH` .</span><span class="sxs-lookup"><span data-stu-id="04325-132">For self-service sign up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="response"></a><span data-ttu-id="04325-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="04325-133">Response</span></span>

<span data-ttu-id="04325-134">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="04325-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="04325-135">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="04325-135">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="04325-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04325-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="04325-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04325-137">Request</span></span>

<span data-ttu-id="04325-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="04325-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_b2xuserflows_identityprovider"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}/identityProviders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/identityProviders/{id}"
}
```

### <a name="response"></a><span data-ttu-id="04325-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="04325-139">Response</span></span>

<span data-ttu-id="04325-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="04325-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
