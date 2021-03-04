---
title: Listar b2xIdentityUserFlows
description: Recupere uma lista de objetos b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 672e98257776a0335c3b8691bc934a7641de6ed6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435543"
---
# <a name="list-b2xidentityuserflows"></a><span data-ttu-id="cf425-103">Listar b2xIdentityUserFlows</span><span class="sxs-lookup"><span data-stu-id="cf425-103">List b2xIdentityUserFlows</span></span>

<span data-ttu-id="cf425-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf425-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf425-105">Recupere uma lista de [objetos b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="cf425-105">Retrieve a list of [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf425-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cf425-106">Permissions</span></span>

<span data-ttu-id="cf425-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf425-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf425-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf425-109">Permission type</span></span>      | <span data-ttu-id="cf425-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cf425-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf425-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf425-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cf425-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf425-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="cf425-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf425-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="cf425-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf425-114">Not supported.</span></span>|
|<span data-ttu-id="cf425-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf425-115">Application</span></span>|<span data-ttu-id="cf425-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf425-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="cf425-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="cf425-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="cf425-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="cf425-118">Global administrator</span></span>
* <span data-ttu-id="cf425-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="cf425-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="cf425-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf425-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cf425-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cf425-121">Optional query parameters</span></span>

<span data-ttu-id="cf425-122">Você pode usar para expandir propriedades de fluxo de usuário `$expand` específicas que não são expandidas por padrão.</span><span class="sxs-lookup"><span data-stu-id="cf425-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span>

<span data-ttu-id="cf425-123">Para obter mais informações, consulte [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="cf425-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf425-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf425-124">Request headers</span></span>

|<span data-ttu-id="cf425-125">Nome</span><span class="sxs-lookup"><span data-stu-id="cf425-125">Name</span></span>|<span data-ttu-id="cf425-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf425-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="cf425-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf425-127">Authorization</span></span>|<span data-ttu-id="cf425-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf425-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf425-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf425-130">Request body</span></span>

<span data-ttu-id="cf425-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cf425-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf425-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf425-132">Response</span></span>

<span data-ttu-id="cf425-133">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf425-133">If successful, this method returns a `200 OK` response code and a collection of [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cf425-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cf425-134">Examples</span></span>

### <a name="example-1-list-all-b2xidentityuserflow-objects"></a><span data-ttu-id="cf425-135">Exemplo 1: Listar todos os objetos b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="cf425-135">Example 1: List all b2xIdentityUserFlow objects</span></span>

#### <a name="request"></a><span data-ttu-id="cf425-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf425-136">Request</span></span>

<span data-ttu-id="cf425-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf425-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cf425-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf425-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_b2xUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows
```
# <a name="c"></a>[<span data-ttu-id="cf425-139">C#</span><span class="sxs-lookup"><span data-stu-id="cf425-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-b2xuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cf425-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf425-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-b2xuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cf425-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cf425-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-b2xuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cf425-142">Java</span><span class="sxs-lookup"><span data-stu-id="cf425-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-b2xuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cf425-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf425-143">Response</span></span>

<span data-ttu-id="cf425-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cf425-144">The following is an example of the response.</span></span>

<span data-ttu-id="cf425-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cf425-145">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-list-all-b2xidentityuserflow-objects-and-expand-identityproviders"></a><span data-ttu-id="cf425-146">Exemplo 2: listar todos os objetos b2xIdentityUserFlow e expandir identityProviders</span><span class="sxs-lookup"><span data-stu-id="cf425-146">Example 2: List all b2xIdentityUserFlow objects and expand identityProviders</span></span>

#### <a name="request"></a><span data-ttu-id="cf425-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf425-147">Request</span></span>

<span data-ttu-id="cf425-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf425-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cf425-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf425-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_b2xUserFlows_expand"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows?$expand=identityProviders
```
# <a name="c"></a>[<span data-ttu-id="cf425-150">C#</span><span class="sxs-lookup"><span data-stu-id="cf425-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-b2xuserflows-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cf425-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf425-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-b2xuserflows-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cf425-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cf425-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-b2xuserflows-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cf425-153">Java</span><span class="sxs-lookup"><span data-stu-id="cf425-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-b2xuserflows-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cf425-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf425-154">Response</span></span>

<span data-ttu-id="cf425-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cf425-155">The following is an example of the response.</span></span>

<span data-ttu-id="cf425-156">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cf425-156">**Note:** The response object shown here might be shortened for readability.</span></span>

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


