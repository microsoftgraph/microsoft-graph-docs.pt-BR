---
title: Listar b2xIdentityUserFlows
description: Recupere uma lista de objetos b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 36b0399c7fd45a90b5bbfb95084f46a15ff65296
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882755"
---
# <a name="list-b2xidentityuserflows"></a><span data-ttu-id="34638-103">Listar b2xIdentityUserFlows</span><span class="sxs-lookup"><span data-stu-id="34638-103">List b2xIdentityUserFlows</span></span>

<span data-ttu-id="34638-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34638-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="34638-105">Recupere uma lista de [objetos b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="34638-105">Retrieve a list of [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="34638-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="34638-106">Permissions</span></span>

<span data-ttu-id="34638-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34638-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34638-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34638-109">Permission type</span></span>      | <span data-ttu-id="34638-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="34638-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34638-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34638-111">Delegated (work or school account)</span></span>|<span data-ttu-id="34638-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34638-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="34638-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34638-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="34638-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34638-114">Not supported.</span></span>|
|<span data-ttu-id="34638-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34638-115">Application</span></span>|<span data-ttu-id="34638-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34638-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="34638-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="34638-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="34638-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="34638-118">Global administrator</span></span>
* <span data-ttu-id="34638-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="34638-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="34638-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34638-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows
```

## <a name="optional-query-parameters"></a><span data-ttu-id="34638-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="34638-121">Optional query parameters</span></span>

<span data-ttu-id="34638-122">Você pode usar para expandir propriedades de fluxo de usuário `$expand` específicas que não são expandidas por padrão.</span><span class="sxs-lookup"><span data-stu-id="34638-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span> <span data-ttu-id="34638-123">Para obter mais informações, consulte [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="34638-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="34638-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34638-124">Request headers</span></span>

|<span data-ttu-id="34638-125">Nome</span><span class="sxs-lookup"><span data-stu-id="34638-125">Name</span></span>|<span data-ttu-id="34638-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="34638-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="34638-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="34638-127">Authorization</span></span>|<span data-ttu-id="34638-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34638-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="34638-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34638-130">Request body</span></span>

<span data-ttu-id="34638-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="34638-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34638-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="34638-132">Response</span></span>

<span data-ttu-id="34638-133">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34638-133">If successful, this method returns a `200 OK` response code and a collection of [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="34638-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="34638-134">Examples</span></span>

### <a name="example-1-list-all-b2xidentityuserflow-objects"></a><span data-ttu-id="34638-135">Exemplo 1: Listar todos os objetos b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="34638-135">Example 1: List all b2xIdentityUserFlow objects</span></span>

#### <a name="request"></a><span data-ttu-id="34638-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34638-136">Request</span></span>

<span data-ttu-id="34638-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="34638-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_b2xUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows
```

#### <a name="response"></a><span data-ttu-id="34638-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="34638-138">Response</span></span>

<span data-ttu-id="34638-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="34638-139">The following is an example of the response.</span></span>

<span data-ttu-id="34638-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="34638-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-list-all-b2xidentityuserflow-objects-and-expand-identityproviders"></a><span data-ttu-id="34638-141">Exemplo 2: listar todos os objetos b2xIdentityUserFlow e expandir identityProviders</span><span class="sxs-lookup"><span data-stu-id="34638-141">Example 2: List all b2xIdentityUserFlow objects and expand identityProviders</span></span>

#### <a name="request"></a><span data-ttu-id="34638-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34638-142">Request</span></span>

<span data-ttu-id="34638-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="34638-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_b2xUserFlows_expand"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows?$expand=identityProviders
```

#### <a name="response"></a><span data-ttu-id="34638-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="34638-144">Response</span></span>

<span data-ttu-id="34638-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="34638-145">The following is an example of the response.</span></span>

<span data-ttu-id="34638-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="34638-146">**Note:** The response object shown here might be shortened for readability.</span></span>

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
