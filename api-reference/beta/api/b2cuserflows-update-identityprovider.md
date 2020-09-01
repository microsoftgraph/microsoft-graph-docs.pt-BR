---
title: Adicionar identityprovider a um b2cUserFlow
description: Adicionar identityprovider a um b2cUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d873cb83984e9da8e58e377df4ad7257b8f6531c
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319631"
---
# <a name="add-identityprovider-to-a-b2cuserflow"></a><span data-ttu-id="d4b74-103">Adicionar identityprovider a um b2cUserFlow</span><span class="sxs-lookup"><span data-stu-id="d4b74-103">Add identityProvider to a b2cUserFlow</span></span>

<span data-ttu-id="d4b74-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4b74-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4b74-105">Adicionar provedores de identidade em um objeto [b2cUserFlow](../resources/b2cuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="d4b74-105">Add identity providers in a [b2cUserFlow](../resources/b2cuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4b74-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d4b74-106">Permissions</span></span>

<span data-ttu-id="d4b74-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4b74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4b74-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4b74-109">Permission type</span></span>      | <span data-ttu-id="d4b74-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d4b74-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4b74-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4b74-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d4b74-112">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d4b74-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="d4b74-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4b74-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="d4b74-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4b74-114">Not supported.</span></span>|
|<span data-ttu-id="d4b74-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4b74-115">Application</span></span>| <span data-ttu-id="d4b74-116">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d4b74-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="d4b74-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="d4b74-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="d4b74-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="d4b74-118">Global administrator</span></span>
* <span data-ttu-id="d4b74-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="d4b74-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="d4b74-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4b74-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /b2cUserFlows/{id}/identityProviders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="d4b74-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4b74-121">Request headers</span></span>

|<span data-ttu-id="d4b74-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d4b74-122">Name</span></span>|<span data-ttu-id="d4b74-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4b74-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="d4b74-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4b74-124">Authorization</span></span>|<span data-ttu-id="d4b74-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4b74-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d4b74-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d4b74-127">Content-Type</span></span>|<span data-ttu-id="d4b74-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4b74-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4b74-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4b74-130">Request body</span></span>

<span data-ttu-id="d4b74-131">No corpo da solicitação, forneça uma representação JSON do `id` [identityprovider](../resources/identityprovider.md) que você deseja adicionar.</span><span class="sxs-lookup"><span data-stu-id="d4b74-131">In the request body, provide a JSON representation of the `id` of the [identityProvider](../resources/identityprovider.md) you want to add.</span></span> <span data-ttu-id="d4b74-132">Para obter mais informações sobre provedores de identidade disponíveis para fluxos de usuário, consulte a referência da API [identityProviders](../resources/identityprovider.md) .</span><span class="sxs-lookup"><span data-stu-id="d4b74-132">For more information about identity providers available for user flows, see the [identityProviders](../resources/identityprovider.md) API reference.</span></span>

## <a name="response"></a><span data-ttu-id="d4b74-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4b74-133">Response</span></span>

<span data-ttu-id="d4b74-134">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d4b74-134">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="d4b74-135">Caso não consiga, um `4xx` erro será retornado com detalhes específicos.</span><span class="sxs-lookup"><span data-stu-id="d4b74-135">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="d4b74-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4b74-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4b74-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4b74-137">Request</span></span>

<span data-ttu-id="d4b74-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4b74-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_b2cuserflows_identityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/identityProviders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/identityProviders/{id}"
}
```

### <a name="response"></a><span data-ttu-id="d4b74-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4b74-139">Response</span></span>

<span data-ttu-id="d4b74-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d4b74-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
