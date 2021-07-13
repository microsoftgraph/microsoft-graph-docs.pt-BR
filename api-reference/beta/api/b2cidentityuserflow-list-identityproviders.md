---
title: Listar todos os identityProviders em um b2cIdentityUserFlow (preterido)
description: Listar todos os identityProviders em um b2cIdentityUserFlow. (preterido)
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 7e83384f009c273197ea8bd8b978e27dd75263a8
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53400975"
---
# <a name="list-all-identityproviders-in-a-b2cidentityuserflow-deprecated"></a><span data-ttu-id="c6b24-104">Listar todos os identityProviders em um b2cIdentityUserFlow (preterido)</span><span class="sxs-lookup"><span data-stu-id="c6b24-104">List all identityProviders in a b2cIdentityUserFlow (deprecated)</span></span>

<span data-ttu-id="c6b24-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6b24-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="c6b24-106">Obter os provedores de identidade em um [objeto b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="c6b24-106">Get the identity providers in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6b24-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c6b24-107">Permissions</span></span>

<span data-ttu-id="c6b24-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6b24-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6b24-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6b24-110">Permission type</span></span>      | <span data-ttu-id="c6b24-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c6b24-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6b24-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6b24-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c6b24-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6b24-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="c6b24-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6b24-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c6b24-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6b24-115">Not supported.</span></span>|
|<span data-ttu-id="c6b24-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6b24-116">Application</span></span>| <span data-ttu-id="c6b24-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6b24-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="c6b24-118">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="c6b24-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="c6b24-119">Administrador global</span><span class="sxs-lookup"><span data-stu-id="c6b24-119">Global administrator</span></span>
* <span data-ttu-id="c6b24-120">Administrador de identidade externa Flow usuário</span><span class="sxs-lookup"><span data-stu-id="c6b24-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="c6b24-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6b24-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2cUserFlows/{id}/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="c6b24-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6b24-122">Request headers</span></span>

|<span data-ttu-id="c6b24-123">Nome</span><span class="sxs-lookup"><span data-stu-id="c6b24-123">Name</span></span>|<span data-ttu-id="c6b24-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6b24-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="c6b24-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6b24-125">Authorization</span></span>|<span data-ttu-id="c6b24-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6b24-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6b24-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6b24-128">Request body</span></span>

<span data-ttu-id="c6b24-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c6b24-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6b24-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6b24-130">Response</span></span>

<span data-ttu-id="c6b24-131">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` representação JSON dos [identityProviders](../resources/identityprovider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6b24-131">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6b24-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6b24-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6b24-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6b24-133">Request</span></span>

<span data-ttu-id="c6b24-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6b24-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_b2cUserFlow_list_identityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/identityProviders
```

### <a name="response"></a><span data-ttu-id="c6b24-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6b24-135">Response</span></span>

<span data-ttu-id="c6b24-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c6b24-136">The following is an example of the response.</span></span>

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
