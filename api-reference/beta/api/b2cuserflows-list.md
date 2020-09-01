---
title: Listar b2cUserFlows
description: Recupere uma lista de objetos b2cUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 889f5bc5f3082a8b23b3ed4d64d43a11fdfe3979
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319629"
---
# <a name="list-b2cuserflows"></a><span data-ttu-id="b1c5c-103">Listar b2cUserFlows</span><span class="sxs-lookup"><span data-stu-id="b1c5c-103">List b2cUserFlows</span></span>

<span data-ttu-id="b1c5c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1c5c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1c5c-105">Recupere uma lista de objetos [b2cUserFlow](../resources/b2cuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="b1c5c-105">Retrieve a list of [b2cUserFlow](../resources/b2cuserflows.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1c5c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b1c5c-106">Permissions</span></span>

<span data-ttu-id="b1c5c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1c5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1c5c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1c5c-109">Permission type</span></span>      | <span data-ttu-id="b1c5c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b1c5c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1c5c-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1c5c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b1c5c-112">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b1c5c-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="b1c5c-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1c5c-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="b1c5c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1c5c-114">Not supported.</span></span>|
|<span data-ttu-id="b1c5c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1c5c-115">Application</span></span>|<span data-ttu-id="b1c5c-116">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b1c5c-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="b1c5c-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="b1c5c-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="b1c5c-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="b1c5c-118">Global administrator</span></span>
* <span data-ttu-id="b1c5c-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="b1c5c-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="b1c5c-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1c5c-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2cUserFlows
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b1c5c-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b1c5c-121">Optional query parameters</span></span>

<span data-ttu-id="b1c5c-122">Você pode usar o `$expand` para expandir Propriedades de fluxo de usuário específicas que não são expandidas por padrão.</span><span class="sxs-lookup"><span data-stu-id="b1c5c-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span>

<span data-ttu-id="b1c5c-123">Para obter mais informações, consulte [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b1c5c-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b1c5c-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1c5c-124">Request headers</span></span>

|<span data-ttu-id="b1c5c-125">Nome</span><span class="sxs-lookup"><span data-stu-id="b1c5c-125">Name</span></span>|<span data-ttu-id="b1c5c-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1c5c-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="b1c5c-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1c5c-127">Authorization</span></span>|<span data-ttu-id="b1c5c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1c5c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1c5c-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1c5c-130">Request body</span></span>

<span data-ttu-id="b1c5c-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b1c5c-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1c5c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1c5c-132">Response</span></span>

<span data-ttu-id="b1c5c-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [b2cUserFlow](../resources/b2cuserflows.md)  no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1c5c-133">If successful, this method returns a `200 OK` response code and a collection of [b2cUserFlow](../resources/b2cuserflows.md)  objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b1c5c-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b1c5c-134">Examples</span></span>

### <a name="example-1-list-all-b2cuserflows"></a><span data-ttu-id="b1c5c-135">Exemplo 1: listar todos os b2cUserFlows</span><span class="sxs-lookup"><span data-stu-id="b1c5c-135">Example 1: List all b2cUserFlows</span></span>

#### <a name="request"></a><span data-ttu-id="b1c5c-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1c5c-136">Request</span></span>

<span data-ttu-id="b1c5c-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1c5c-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_b2cUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows
```

#### <a name="response"></a><span data-ttu-id="b1c5c-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1c5c-138">Response</span></span>

<span data-ttu-id="b1c5c-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b1c5c-139">The following is an example of the response.</span></span>

<span data-ttu-id="b1c5c-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b1c5c-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cIdentityUserFlow",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows",
    "value": [
      {
          "id": "B2C_1_CustomerSignUp",
          "userFlowType": "signUp",
          "userFlowTypeVersion": 1
      },
      {
          "id": "B2C_1_CustomerSignIn",
          "userFlowType": "signIn",
          "userFlowTypeVersion": 1
      },
    ]
}
```

### <a name="example-2-list-all-b2cuserflows-and-expand-identityproviders"></a><span data-ttu-id="b1c5c-141">Exemplo 2: listar todos os b2cUserFlows e expandir identityProviders</span><span class="sxs-lookup"><span data-stu-id="b1c5c-141">Example 2: List all b2cUserFlows and expand identityProviders</span></span>

#### <a name="request"></a><span data-ttu-id="b1c5c-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1c5c-142">Request</span></span>

<span data-ttu-id="b1c5c-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1c5c-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_b2cUserFlows_expand"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows?$expand=identityProviders
```

#### <a name="response"></a><span data-ttu-id="b1c5c-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1c5c-144">Response</span></span>

<span data-ttu-id="b1c5c-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b1c5c-145">The following is an example of the response.</span></span>

<span data-ttu-id="b1c5c-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b1c5c-146">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cIdentityUserFlow",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows",
    "value": [
      {
          "id": "B2C_1_CustomerSignUp",
          "userFlowType": "signUp",
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
          "id": "B2C_1_CustomerSignIn",
          "userFlowType": "signIn",
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
  "description": "List b2cUserFlows",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: list_b2cUserFlows/container/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: list_b2cUserFlows_expand/container/userFlowTypeVersion:\r\n    Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
