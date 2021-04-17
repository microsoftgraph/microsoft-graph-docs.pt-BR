---
title: Obter b2xIdentityUserFlow
description: Recupere as propriedades e as relações de um objeto b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: a498e4a6ab1d652dca3c90afc33649f0c0ada908
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882385"
---
# <a name="get-b2xidentityuserflow"></a><span data-ttu-id="3a15a-103">Obter b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="3a15a-103">Get b2xIdentityUserFlow</span></span>

<span data-ttu-id="3a15a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a15a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3a15a-105">Recupere as propriedades e as relações de um [objeto b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="3a15a-105">Retrieve the properties and relationships of a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a15a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3a15a-106">Permissions</span></span>

<span data-ttu-id="3a15a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a15a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a15a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a15a-109">Permission type</span></span>      | <span data-ttu-id="3a15a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3a15a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a15a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a15a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3a15a-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a15a-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="3a15a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a15a-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="3a15a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a15a-114">Not supported.</span></span>|
|<span data-ttu-id="3a15a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a15a-115">Application</span></span>|<span data-ttu-id="3a15a-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a15a-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="3a15a-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="3a15a-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="3a15a-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="3a15a-118">Global administrator</span></span>
* <span data-ttu-id="3a15a-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="3a15a-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="3a15a-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a15a-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3a15a-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3a15a-121">Optional query parameters</span></span>

<span data-ttu-id="3a15a-122">Você pode usar para expandir propriedades de fluxo de usuário `$expand` específicas que não são expandidas por padrão.</span><span class="sxs-lookup"><span data-stu-id="3a15a-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span> <span data-ttu-id="3a15a-123">Para obter mais informações, consulte [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3a15a-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a15a-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a15a-124">Request headers</span></span>

|<span data-ttu-id="3a15a-125">Nome</span><span class="sxs-lookup"><span data-stu-id="3a15a-125">Name</span></span>|<span data-ttu-id="3a15a-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a15a-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="3a15a-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a15a-127">Authorization</span></span>|<span data-ttu-id="3a15a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a15a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a15a-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a15a-130">Request body</span></span>

<span data-ttu-id="3a15a-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3a15a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a15a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a15a-132">Response</span></span>

<span data-ttu-id="3a15a-133">Se tiver êxito, este método retornará um código de resposta e uma representação JSON do `200 OK` [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a15a-133">If successful, this method returns a `200 OK` response code and a JSON representation of the [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a15a-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a15a-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a15a-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a15a-135">Request</span></span>

<span data-ttu-id="3a15a-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a15a-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_PartnerSignUp
```

### <a name="response"></a><span data-ttu-id="3a15a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a15a-137">Response</span></span>

<span data-ttu-id="3a15a-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3a15a-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "B2X_1_PartnerSignUp",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Get b2xUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: get_b2xUserFlows/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
