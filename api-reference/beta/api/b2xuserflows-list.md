---
title: Listar b2xUserFlows
description: Recupere uma lista de objetos b2xUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cec5cd2bd05d8c2f6b73002bcd779790ffc34b66
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319630"
---
# <a name="list-b2xuserflows"></a><span data-ttu-id="55346-103">Listar b2xUserFlows</span><span class="sxs-lookup"><span data-stu-id="55346-103">List b2xUserFlows</span></span>

<span data-ttu-id="55346-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55346-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55346-105">Recupere uma lista de objetos [b2xUserFlow](../resources/b2xuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="55346-105">Retrieve a list of [b2xUserFlow](../resources/b2xuserflows.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="55346-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="55346-106">Permissions</span></span>

<span data-ttu-id="55346-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55346-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55346-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55346-109">Permission type</span></span>      | <span data-ttu-id="55346-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="55346-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55346-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55346-111">Delegated (work or school account)</span></span>|<span data-ttu-id="55346-112">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="55346-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="55346-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55346-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="55346-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55346-114">Not supported.</span></span>|
|<span data-ttu-id="55346-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55346-115">Application</span></span>|<span data-ttu-id="55346-116">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="55346-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="55346-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="55346-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="55346-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="55346-118">Global administrator</span></span>
* <span data-ttu-id="55346-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="55346-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="55346-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55346-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows
```

## <a name="optional-query-parameters"></a><span data-ttu-id="55346-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="55346-121">Optional query parameters</span></span>

<span data-ttu-id="55346-122">Você pode usar o `$expand` para expandir Propriedades de fluxo de usuário específicas que não são expandidas por padrão.</span><span class="sxs-lookup"><span data-stu-id="55346-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span>

<span data-ttu-id="55346-123">Para obter mais informações, consulte [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="55346-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="55346-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55346-124">Request headers</span></span>

|<span data-ttu-id="55346-125">Nome</span><span class="sxs-lookup"><span data-stu-id="55346-125">Name</span></span>|<span data-ttu-id="55346-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="55346-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="55346-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="55346-127">Authorization</span></span>|<span data-ttu-id="55346-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55346-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="55346-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55346-130">Request body</span></span>

<span data-ttu-id="55346-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="55346-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55346-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="55346-132">Response</span></span>

<span data-ttu-id="55346-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [b2xUserFlow](../resources/b2xuserflows.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55346-133">If successful, this method returns a `200 OK` response code and a collection of [b2xUserFlow](../resources/b2xuserflows.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="55346-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="55346-134">Examples</span></span>

### <a name="example-1-list-all-b2xuserflows"></a><span data-ttu-id="55346-135">Exemplo 1: listar todos os b2xUserFlows</span><span class="sxs-lookup"><span data-stu-id="55346-135">Example 1: List all b2xUserFlows</span></span>

#### <a name="request"></a><span data-ttu-id="55346-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55346-136">Request</span></span>

<span data-ttu-id="55346-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="55346-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_b2xUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows
```

#### <a name="response"></a><span data-ttu-id="55346-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="55346-138">Response</span></span>

<span data-ttu-id="55346-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="55346-139">The following is an example of the response.</span></span>

<span data-ttu-id="55346-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="55346-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2xUserFlows",
    "value": [
      {
          "id": "B2X_1_PartnerSignUp",
          "userFlowType": "signUpOrSignIn",
          "userFlowTypeVersion": 1
      },
      {
          "id": "B2X_1_ContosoSignUp",
          "userFlowType": "signUpOrSignIn",
          "userFlowTypeVersion": 1
      },
    ]
}
```

### <a name="example-2-list-all-b2xuserflows-and-expand-identityproviders"></a><span data-ttu-id="55346-141">Exemplo 2: listar todos os b2xUserFlows e expandir identityProviders</span><span class="sxs-lookup"><span data-stu-id="55346-141">Example 2: List all b2xUserFlows and expand identityProviders</span></span>

#### <a name="request"></a><span data-ttu-id="55346-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55346-142">Request</span></span>

<span data-ttu-id="55346-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="55346-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_b2xUserFlows_expand"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows?$expand=identityProviders
```

#### <a name="response"></a><span data-ttu-id="55346-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="55346-144">Response</span></span>

<span data-ttu-id="55346-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="55346-145">The following is an example of the response.</span></span>

<span data-ttu-id="55346-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="55346-146">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2xUserFlows(identityProviders)",
    "value": [
      {
          "id": "B2X_1_PartnerSignUp",
          "userFlowType": "signUpOrSignIn",
          "userFlowTypeVersion": 1,
          "identityProviders": [
              {
                "id": "Facebook-OAuth",
                "type": "Facebook",
                "name": "Facebook",
                "clientId": "clientIdFromFacebook",
                "clientSecret": "*******"
              }  
          ]
      },
      {
          "id": "B2X_1_ContosoSignUp",
          "userFlowType": "signUpOrSignIn",
          "userFlowTypeVersion": 1,
          "identityProviders": [
              {
                "id": "Facebook-OAuth",
                "type": "Facebook",
                "name": "Facebook",
                "clientId": "clientIdFromFacebook",
                "clientSecret": "*******"
              }  
          ]
      }
   ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "List b2xUserFlows",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: list_b2xUserFlows/container/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: list_b2xUserFlows_expand/container/userFlowTypeVersion:\r\n    Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
