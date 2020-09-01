---
title: Obter b2cUserFlows
description: Recupere as propriedades e os relacionamentos de um objeto b2cUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ea558ddd1f8146b33eb5b153dfc0fcb73b21d6b1
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319647"
---
# <a name="get-b2cuserflow"></a><span data-ttu-id="11046-103">Obter b2cUserFlow</span><span class="sxs-lookup"><span data-stu-id="11046-103">Get b2cUserFlow</span></span>

<span data-ttu-id="11046-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11046-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11046-105">Recupere as propriedades e os relacionamentos de um objeto [b2cUserFlow](../resources/b2cuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="11046-105">Retrieve the properties and relationships of a [b2cUserFlow](../resources/b2cuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="11046-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="11046-106">Permissions</span></span>

<span data-ttu-id="11046-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11046-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11046-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11046-109">Permission type</span></span>      | <span data-ttu-id="11046-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="11046-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11046-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11046-111">Delegated (work or school account)</span></span>|<span data-ttu-id="11046-112">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="11046-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="11046-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11046-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="11046-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11046-114">Not supported.</span></span>|
|<span data-ttu-id="11046-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11046-115">Application</span></span>|<span data-ttu-id="11046-116">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="11046-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="11046-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="11046-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="11046-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="11046-118">Global administrator</span></span>
* <span data-ttu-id="11046-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="11046-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="11046-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11046-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2cUserFlows/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="11046-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="11046-121">Optional query parameters</span></span>

<span data-ttu-id="11046-122">Você pode usar o `$expand` para expandir Propriedades de fluxo de usuário específicas que não são expandidas por padrão.</span><span class="sxs-lookup"><span data-stu-id="11046-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span>

<span data-ttu-id="11046-123">Para obter mais informações, consulte [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="11046-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="11046-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11046-124">Request headers</span></span>

|<span data-ttu-id="11046-125">Nome</span><span class="sxs-lookup"><span data-stu-id="11046-125">Name</span></span>|<span data-ttu-id="11046-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="11046-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="11046-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="11046-127">Authorization</span></span>|<span data-ttu-id="11046-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11046-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="11046-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11046-130">Request body</span></span>

<span data-ttu-id="11046-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="11046-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11046-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="11046-132">Response</span></span>

<span data-ttu-id="11046-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma representação JSON do [b2cUserFlow](../resources/b2cuserflows.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11046-133">If successful, this method returns a `200 OK` response code and a JSON representation of the [b2cUserFlow](../resources/b2cuserflows.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11046-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11046-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="11046-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11046-135">Request</span></span>

<span data-ttu-id="11046-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="11046-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_b2cUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}
```

### <a name="response"></a><span data-ttu-id="11046-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="11046-137">Response</span></span>

<span data-ttu-id="11046-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="11046-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cIdentityUserFlow"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "B2C_1_CustomerSignUp",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Get b2cUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: get_b2cUserFlows/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->