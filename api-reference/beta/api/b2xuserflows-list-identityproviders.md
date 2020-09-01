---
title: Listar todos os identityProviders em um b2xUserFlow
description: Listar todos os identityProviders em um b2xUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 87e73efb4de6ef6a118d569592d907c2ae9b6910
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319633"
---
# <a name="list-all-identityproviders-in-a-b2xuserflow"></a><span data-ttu-id="77862-103">Listar todos os identityProviders em um b2xUserFlow</span><span class="sxs-lookup"><span data-stu-id="77862-103">List all identityProviders in a b2xUserFlow</span></span>

<span data-ttu-id="77862-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77862-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77862-105">Obtenha os provedores de identidade em um objeto [b2xUserFlow](../resources/b2xuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="77862-105">Get the identity providers in a [b2xUserFlow](../resources/b2xuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="77862-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="77862-106">Permissions</span></span>

<span data-ttu-id="77862-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77862-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77862-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77862-109">Permission type</span></span>      | <span data-ttu-id="77862-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="77862-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77862-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77862-111">Delegated (work or school account)</span></span>|<span data-ttu-id="77862-112">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="77862-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="77862-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77862-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="77862-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77862-114">Not supported.</span></span>|
|<span data-ttu-id="77862-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77862-115">Application</span></span>| <span data-ttu-id="77862-116">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="77862-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="77862-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="77862-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="77862-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="77862-118">Global administrator</span></span>
* <span data-ttu-id="77862-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="77862-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="77862-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77862-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /b2xUserFlows/{id}/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="77862-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77862-121">Request headers</span></span>

|<span data-ttu-id="77862-122">Nome</span><span class="sxs-lookup"><span data-stu-id="77862-122">Name</span></span>|<span data-ttu-id="77862-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="77862-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="77862-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="77862-124">Authorization</span></span>|<span data-ttu-id="77862-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77862-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="77862-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77862-127">Request body</span></span>

<span data-ttu-id="77862-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="77862-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77862-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="77862-129">Response</span></span>

<span data-ttu-id="77862-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma representação JSON do [identityProviders](../resources/identityprovider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77862-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77862-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77862-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="77862-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77862-132">Request</span></span>

<span data-ttu-id="77862-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="77862-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlow_list_identityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}/identityProviders
```

### <a name="response"></a><span data-ttu-id="77862-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="77862-134">Response</span></span>

<span data-ttu-id="77862-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="77862-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProvider"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "Facebook-OAuth",
            "type": "Facebook",
            "name": "Facebook",
            "clientId": "clientIdFromFacebook",
            "clientSecret": "*****"
        },
        {
            "id": "Google-OAuth",
            "type": "Google",
            "name": "Google",
            "clientId": "clientIdFromGoogle",
            "clientSecret": "*****"
        }
    ]
}
```