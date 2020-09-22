---
title: Listar b2cUserFlows
description: Recupere uma lista de objetos b2cUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 333dc0872e228ab1f2bd66570c780488ba4ee1a6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991457"
---
# <a name="list-b2cuserflows"></a><span data-ttu-id="eb4b4-103">Listar b2cUserFlows</span><span class="sxs-lookup"><span data-stu-id="eb4b4-103">List b2cUserFlows</span></span>

<span data-ttu-id="eb4b4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb4b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb4b4-105">Recupere uma lista de objetos [b2cUserFlow](../resources/b2cuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="eb4b4-105">Retrieve a list of [b2cUserFlow](../resources/b2cuserflows.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb4b4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="eb4b4-106">Permissions</span></span>

<span data-ttu-id="eb4b4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb4b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb4b4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb4b4-109">Permission type</span></span>      | <span data-ttu-id="eb4b4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eb4b4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb4b4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb4b4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eb4b4-112">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="eb4b4-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="eb4b4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb4b4-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="eb4b4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb4b4-114">Not supported.</span></span>|
|<span data-ttu-id="eb4b4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb4b4-115">Application</span></span>|<span data-ttu-id="eb4b4-116">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="eb4b4-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="eb4b4-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="eb4b4-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="eb4b4-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="eb4b4-118">Global administrator</span></span>
* <span data-ttu-id="eb4b4-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="eb4b4-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="eb4b4-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb4b4-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2cUserFlows
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eb4b4-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="eb4b4-121">Optional query parameters</span></span>

<span data-ttu-id="eb4b4-122">Você pode usar o `$expand` para expandir Propriedades de fluxo de usuário específicas que não são expandidas por padrão.</span><span class="sxs-lookup"><span data-stu-id="eb4b4-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span>

<span data-ttu-id="eb4b4-123">Para obter mais informações, consulte [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="eb4b4-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb4b4-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb4b4-124">Request headers</span></span>

|<span data-ttu-id="eb4b4-125">Nome</span><span class="sxs-lookup"><span data-stu-id="eb4b4-125">Name</span></span>|<span data-ttu-id="eb4b4-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb4b4-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="eb4b4-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb4b4-127">Authorization</span></span>|<span data-ttu-id="eb4b4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb4b4-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb4b4-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb4b4-130">Request body</span></span>

<span data-ttu-id="eb4b4-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eb4b4-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb4b4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb4b4-132">Response</span></span>

<span data-ttu-id="eb4b4-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [b2cUserFlow](../resources/b2cuserflows.md)  no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb4b4-133">If successful, this method returns a `200 OK` response code and a collection of [b2cUserFlow](../resources/b2cuserflows.md)  objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eb4b4-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="eb4b4-134">Examples</span></span>

### <a name="example-1-list-all-b2cuserflows"></a><span data-ttu-id="eb4b4-135">Exemplo 1: listar todos os b2cUserFlows</span><span class="sxs-lookup"><span data-stu-id="eb4b4-135">Example 1: List all b2cUserFlows</span></span>

#### <a name="request"></a><span data-ttu-id="eb4b4-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb4b4-136">Request</span></span>

<span data-ttu-id="eb4b4-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb4b4-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="eb4b4-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb4b4-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_b2cUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows
```
# <a name="c"></a>[<span data-ttu-id="eb4b4-139">C#</span><span class="sxs-lookup"><span data-stu-id="eb4b4-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb4b4-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb4b4-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb4b4-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb4b4-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="eb4b4-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb4b4-142">Response</span></span>

<span data-ttu-id="eb4b4-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="eb4b4-143">The following is an example of the response.</span></span>

<span data-ttu-id="eb4b4-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="eb4b4-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-list-all-b2cuserflows-and-expand-identityproviders"></a><span data-ttu-id="eb4b4-145">Exemplo 2: listar todos os b2cUserFlows e expandir identityProviders</span><span class="sxs-lookup"><span data-stu-id="eb4b4-145">Example 2: List all b2cUserFlows and expand identityProviders</span></span>

#### <a name="request"></a><span data-ttu-id="eb4b4-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb4b4-146">Request</span></span>

<span data-ttu-id="eb4b4-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb4b4-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="eb4b4-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb4b4-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_b2cUserFlows_expand"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows?$expand=identityProviders
```
# <a name="c"></a>[<span data-ttu-id="eb4b4-149">C#</span><span class="sxs-lookup"><span data-stu-id="eb4b4-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-b2cuserflows-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb4b4-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb4b4-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-b2cuserflows-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb4b4-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb4b4-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-b2cuserflows-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="eb4b4-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb4b4-152">Response</span></span>

<span data-ttu-id="eb4b4-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="eb4b4-153">The following is an example of the response.</span></span>

<span data-ttu-id="eb4b4-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="eb4b4-154">**Note:** The response object shown here might be shortened for readability.</span></span>

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


