---
title: Lista identityProviders
description: Listar todos os identityProviders em um b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 01e1e3092c31d3bc9cef921e817da991e9b804cb
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882863"
---
# <a name="list-identityproviders"></a><span data-ttu-id="fdcc1-103">Lista identityProviders</span><span class="sxs-lookup"><span data-stu-id="fdcc1-103">List identityProviders</span></span>

<span data-ttu-id="fdcc1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fdcc1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fdcc1-105">Obter os provedores de identidade em um [objeto b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="fdcc1-105">Get the identity providers in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fdcc1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fdcc1-106">Permissions</span></span>

<span data-ttu-id="fdcc1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdcc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdcc1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fdcc1-109">Permission type</span></span>      | <span data-ttu-id="fdcc1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fdcc1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fdcc1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fdcc1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fdcc1-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdcc1-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="fdcc1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fdcc1-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="fdcc1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdcc1-114">Not supported.</span></span>|
|<span data-ttu-id="fdcc1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fdcc1-115">Application</span></span>| <span data-ttu-id="fdcc1-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdcc1-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="fdcc1-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="fdcc1-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="fdcc1-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="fdcc1-118">Global administrator</span></span>
* <span data-ttu-id="fdcc1-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="fdcc1-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="fdcc1-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fdcc1-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows/{id}/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="fdcc1-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fdcc1-121">Request headers</span></span>

|<span data-ttu-id="fdcc1-122">Nome</span><span class="sxs-lookup"><span data-stu-id="fdcc1-122">Name</span></span>|<span data-ttu-id="fdcc1-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdcc1-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="fdcc1-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fdcc1-124">Authorization</span></span>|<span data-ttu-id="fdcc1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fdcc1-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdcc1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fdcc1-127">Request body</span></span>

<span data-ttu-id="fdcc1-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fdcc1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fdcc1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdcc1-129">Response</span></span>

<span data-ttu-id="fdcc1-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` representação JSON dos [identityProviders](../resources/identityprovider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fdcc1-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdcc1-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fdcc1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fdcc1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fdcc1-132">Request</span></span>

<span data-ttu-id="fdcc1-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fdcc1-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlow_list_identityProviders"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/identityProviders
```

### <a name="response"></a><span data-ttu-id="fdcc1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdcc1-134">Response</span></span>

<span data-ttu-id="fdcc1-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fdcc1-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProvider",
  "isCollection": true
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
 "description": "get_b2xuserflow_list_identityproviders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
