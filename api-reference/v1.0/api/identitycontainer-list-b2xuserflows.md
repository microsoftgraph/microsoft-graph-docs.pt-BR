---
title: Listar b2xIdentityUserFlows
description: Recupere uma lista de objetos b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 65d592129e3475a55226199b0c246ad436a0af71
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920114"
---
# <a name="list-b2xidentityuserflows"></a><span data-ttu-id="d6fdd-103">Listar b2xIdentityUserFlows</span><span class="sxs-lookup"><span data-stu-id="d6fdd-103">List b2xIdentityUserFlows</span></span>

<span data-ttu-id="d6fdd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6fdd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d6fdd-105">Recupere uma lista de [objetos b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="d6fdd-105">Retrieve a list of [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6fdd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d6fdd-106">Permissions</span></span>

<span data-ttu-id="d6fdd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6fdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6fdd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6fdd-109">Permission type</span></span>      | <span data-ttu-id="d6fdd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d6fdd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6fdd-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6fdd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d6fdd-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6fdd-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="d6fdd-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6fdd-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="d6fdd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6fdd-114">Not supported.</span></span>|
|<span data-ttu-id="d6fdd-115">Application</span><span class="sxs-lookup"><span data-stu-id="d6fdd-115">Application</span></span>|<span data-ttu-id="d6fdd-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6fdd-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="d6fdd-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="d6fdd-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="d6fdd-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="d6fdd-118">Global administrator</span></span>
* <span data-ttu-id="d6fdd-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="d6fdd-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="d6fdd-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6fdd-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d6fdd-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d6fdd-121">Optional query parameters</span></span>

<span data-ttu-id="d6fdd-122">Você pode usar para expandir propriedades de fluxo de usuário `$expand` específicas que não são expandidas por padrão.</span><span class="sxs-lookup"><span data-stu-id="d6fdd-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span> <span data-ttu-id="d6fdd-123">Para obter mais informações, consulte [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d6fdd-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6fdd-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6fdd-124">Request headers</span></span>

|<span data-ttu-id="d6fdd-125">Nome</span><span class="sxs-lookup"><span data-stu-id="d6fdd-125">Name</span></span>|<span data-ttu-id="d6fdd-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6fdd-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="d6fdd-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6fdd-127">Authorization</span></span>|<span data-ttu-id="d6fdd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6fdd-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6fdd-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6fdd-130">Request body</span></span>

<span data-ttu-id="d6fdd-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d6fdd-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6fdd-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6fdd-132">Response</span></span>

<span data-ttu-id="d6fdd-133">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6fdd-133">If successful, this method returns a `200 OK` response code and a collection of [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d6fdd-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d6fdd-134">Examples</span></span>

### <a name="example-1-list-all-b2xidentityuserflow-objects"></a><span data-ttu-id="d6fdd-135">Exemplo 1: Listar todos os objetos b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="d6fdd-135">Example 1: List all b2xIdentityUserFlow objects</span></span>

#### <a name="request"></a><span data-ttu-id="d6fdd-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6fdd-136">Request</span></span>

<span data-ttu-id="d6fdd-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6fdd-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d6fdd-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6fdd-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_b2xUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows
```
# <a name="c"></a>[<span data-ttu-id="d6fdd-139">C#</span><span class="sxs-lookup"><span data-stu-id="d6fdd-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-b2xuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6fdd-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6fdd-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-b2xuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6fdd-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6fdd-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-b2xuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d6fdd-142">Java</span><span class="sxs-lookup"><span data-stu-id="d6fdd-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-b2xuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d6fdd-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6fdd-143">Response</span></span>

<span data-ttu-id="d6fdd-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d6fdd-144">The following is an example of the response.</span></span>

<span data-ttu-id="d6fdd-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d6fdd-145">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows",
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

### <a name="example-2-list-all-b2xidentityuserflow-objects-and-expand-identityproviders"></a><span data-ttu-id="d6fdd-146">Exemplo 2: listar todos os objetos b2xIdentityUserFlow e expandir identityProviders</span><span class="sxs-lookup"><span data-stu-id="d6fdd-146">Example 2: List all b2xIdentityUserFlow objects and expand identityProviders</span></span>

#### <a name="request"></a><span data-ttu-id="d6fdd-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6fdd-147">Request</span></span>

<span data-ttu-id="d6fdd-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6fdd-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d6fdd-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6fdd-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_b2xUserFlows_expand"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows?$expand=identityProviders
```
# <a name="c"></a>[<span data-ttu-id="d6fdd-150">C#</span><span class="sxs-lookup"><span data-stu-id="d6fdd-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-b2xuserflows-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6fdd-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6fdd-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-b2xuserflows-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6fdd-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6fdd-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-b2xuserflows-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d6fdd-153">Java</span><span class="sxs-lookup"><span data-stu-id="d6fdd-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-b2xuserflows-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d6fdd-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6fdd-154">Response</span></span>

<span data-ttu-id="d6fdd-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d6fdd-155">The following is an example of the response.</span></span>

<span data-ttu-id="d6fdd-156">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d6fdd-156">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows(identityProviders)",
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
