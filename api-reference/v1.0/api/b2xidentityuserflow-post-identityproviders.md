---
title: Adicionar identityProvider
description: Adicione um provedor de identidade a um fluxo de usuário B2X.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 9ceefc258d5042877f524c5e882ea8adbdd93180
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882787"
---
# <a name="add-identityprovider"></a><span data-ttu-id="7a784-103">Adicionar identityProvider</span><span class="sxs-lookup"><span data-stu-id="7a784-103">Add identityProvider</span></span>

<span data-ttu-id="7a784-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a784-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7a784-105">Atualize os provedores de identidade em um [objeto b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="7a784-105">Update the identity providers in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a784-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7a784-106">Permissions</span></span>

<span data-ttu-id="7a784-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a784-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a784-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a784-109">Permission type</span></span>      | <span data-ttu-id="7a784-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7a784-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a784-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a784-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7a784-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a784-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="7a784-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a784-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="7a784-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a784-114">Not supported.</span></span>|
|<span data-ttu-id="7a784-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a784-115">Application</span></span>| <span data-ttu-id="7a784-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a784-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="7a784-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="7a784-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="7a784-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="7a784-118">Global administrator</span></span>
* <span data-ttu-id="7a784-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="7a784-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="7a784-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a784-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/b2xUserFlows/{id}/identityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="7a784-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a784-121">Request headers</span></span>

|<span data-ttu-id="7a784-122">Nome</span><span class="sxs-lookup"><span data-stu-id="7a784-122">Name</span></span>|<span data-ttu-id="7a784-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a784-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="7a784-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a784-124">Authorization</span></span>|<span data-ttu-id="7a784-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a784-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7a784-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7a784-127">Content-Type</span></span>|<span data-ttu-id="7a784-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a784-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a784-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a784-130">Request body</span></span>

<span data-ttu-id="7a784-131">No corpo da solicitação, forneça uma representação JSON da `id` [identidadeProvider](../resources/identityprovider.md) que você deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="7a784-131">In the request body, provide a JSON representation of the `id` of the [identityProvider](../resources/identityprovider.md) you want to add.</span></span> <span data-ttu-id="7a784-132">Para fluxos de usuários de autoatendados, os valores podem ser `Google-OAUTH` ou `Facebook-OAUTH` .</span><span class="sxs-lookup"><span data-stu-id="7a784-132">For self-service sign up user flows, the values can be `Google-OAUTH` or `Facebook-OAUTH`.</span></span>

## <a name="response"></a><span data-ttu-id="7a784-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a784-133">Response</span></span>

<span data-ttu-id="7a784-134">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7a784-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="7a784-135">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="7a784-135">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="7a784-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7a784-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a784-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a784-137">Request</span></span>

<span data-ttu-id="7a784-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7a784-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_b2xuserflows_identityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/identityProviders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/v1.0/identityProviders/Facebook-OAUTH"
}
```

### <a name="response"></a><span data-ttu-id="7a784-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a784-139">Response</span></span>

<span data-ttu-id="7a784-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7a784-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
