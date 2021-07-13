---
title: Listar todos os identityProviders em um b2xIdentityUserFlow (preterido)
description: Listar todos os identityProviders em um b2xIdentityUserFlow (preterido).
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 28265310a7dd0ff111babb89f218797ba194e03f
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53400919"
---
# <a name="list-all-identityproviders-in-a-b2xidentityuserflow-deprecated"></a><span data-ttu-id="70497-103">Listar todos os identityProviders em um b2xIdentityUserFlow (preterido)</span><span class="sxs-lookup"><span data-stu-id="70497-103">List all identityProviders in a b2xIdentityUserFlow (deprecated)</span></span>

<span data-ttu-id="70497-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70497-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="70497-105">Obter os provedores de identidade em um [objeto b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="70497-105">Get the identity providers in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="70497-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="70497-106">Permissions</span></span>

<span data-ttu-id="70497-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70497-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70497-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70497-109">Permission type</span></span>      | <span data-ttu-id="70497-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="70497-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70497-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70497-111">Delegated (work or school account)</span></span>|<span data-ttu-id="70497-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70497-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="70497-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70497-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="70497-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70497-114">Not supported.</span></span>|
|<span data-ttu-id="70497-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="70497-115">Application</span></span>| <span data-ttu-id="70497-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70497-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="70497-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="70497-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="70497-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="70497-118">Global administrator</span></span>
* <span data-ttu-id="70497-119">Administrador de identidade externa Flow usuário</span><span class="sxs-lookup"><span data-stu-id="70497-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="70497-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70497-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows/{id}/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="70497-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70497-121">Request headers</span></span>

|<span data-ttu-id="70497-122">Nome</span><span class="sxs-lookup"><span data-stu-id="70497-122">Name</span></span>|<span data-ttu-id="70497-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="70497-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="70497-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="70497-124">Authorization</span></span>|<span data-ttu-id="70497-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70497-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="70497-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70497-127">Request body</span></span>

<span data-ttu-id="70497-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="70497-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70497-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="70497-129">Response</span></span>

<span data-ttu-id="70497-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` representação JSON dos [identityProviders](../resources/identityprovider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70497-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70497-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70497-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="70497-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70497-132">Request</span></span>

<span data-ttu-id="70497-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="70497-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlow_list_identityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}/identityProviders
```

### <a name="response"></a><span data-ttu-id="70497-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="70497-134">Response</span></span>

<span data-ttu-id="70497-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="70497-135">The following is an example of the response.</span></span>

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
