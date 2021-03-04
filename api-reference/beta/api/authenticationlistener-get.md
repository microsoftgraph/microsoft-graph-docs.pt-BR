---
title: Obter authenticationListener
description: Leia as propriedades e as relações de um objeto authenticationListener.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e6cacb31a31963457c2e37fd9a63d1c0eeea2c6c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438481"
---
# <a name="get-authenticationlistener"></a><span data-ttu-id="cd3da-103">Obter authenticationListener</span><span class="sxs-lookup"><span data-stu-id="cd3da-103">Get authenticationListener</span></span>

<span data-ttu-id="cd3da-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd3da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd3da-105">Obter a autenticação [especificadaListener definida](../resources/authenticationlistener.md) para o evento onSignupStart no pipeline de autenticação.</span><span class="sxs-lookup"><span data-stu-id="cd3da-105">Get the specified [authenticationListener](../resources/authenticationlistener.md) defined for the onSignupStart event in the authentication pipeline.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd3da-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cd3da-106">Permissions</span></span>

<span data-ttu-id="cd3da-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd3da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd3da-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cd3da-109">Permission type</span></span>|<span data-ttu-id="cd3da-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cd3da-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd3da-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cd3da-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cd3da-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="cd3da-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span>|
|<span data-ttu-id="cd3da-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cd3da-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd3da-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd3da-114">Not supported.</span></span>|
|<span data-ttu-id="cd3da-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cd3da-115">Application</span></span>|<span data-ttu-id="cd3da-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="cd3da-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd3da-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cd3da-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/events/onSignupStart/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cd3da-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cd3da-118">Optional query parameters</span></span>

<span data-ttu-id="cd3da-119">Este método dá suporte ao parâmetro de consulta OData para expandir os detalhes `$expand` de um invokeUserFlowListener.</span><span class="sxs-lookup"><span data-stu-id="cd3da-119">This method supports the `$expand` OData query parameter to expand the details of an invokeUserFlowListener.</span></span> <span data-ttu-id="cd3da-120">Confira abaixo um exemplo.</span><span class="sxs-lookup"><span data-stu-id="cd3da-120">See below for an example.</span></span> <span data-ttu-id="cd3da-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="cd3da-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cd3da-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cd3da-122">Request headers</span></span>

|<span data-ttu-id="cd3da-123">Nome</span><span class="sxs-lookup"><span data-stu-id="cd3da-123">Name</span></span>|<span data-ttu-id="cd3da-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd3da-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cd3da-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="cd3da-125">Authorization</span></span>|<span data-ttu-id="cd3da-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd3da-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd3da-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cd3da-128">Request body</span></span>

<span data-ttu-id="cd3da-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cd3da-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd3da-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd3da-130">Response</span></span>

<span data-ttu-id="cd3da-131">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [authenticationListener](../resources/authenticationlistener.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cd3da-131">If successful, this method returns a `200 OK` response code and an [authenticationListener](../resources/authenticationlistener.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cd3da-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cd3da-132">Examples</span></span>

### <a name="example-1-get-an-authenticationlistener-by-id"></a><span data-ttu-id="cd3da-133">Exemplo 1: Obter um authenticationListener por id</span><span class="sxs-lookup"><span data-stu-id="cd3da-133">Example 1: Get an authenticationListener by id</span></span>

#### <a name="request"></a><span data-ttu-id="cd3da-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd3da-134">Request</span></span>

<span data-ttu-id="cd3da-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd3da-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_authenticationlistener"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}
```

#### <a name="response"></a><span data-ttu-id="cd3da-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd3da-136">Response</span></span>

<span data-ttu-id="cd3da-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cd3da-137">The following is an example of the response.</span></span>

<span data-ttu-id="cd3da-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cd3da-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationListener"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "odata.context": "https://graph.microsoft.com/beta/$metadata#identity/events/onSignUpStart/$entity",
  "@odata.type": "#microsoft.graph.invokeUserFlowListener",
  "id": "2adb5c12-5c12-2adb-125c-db2a125cdb2a",
  "priority": 101,
  "sourceFilter": {
      "includeApplications": [
          "3dfff01b-0afb-4a07-967f-d1ccbd81102a"
      ]
   }
}
```

### <a name="example-2-expand-invokeuserflowlistener-for-a-specific-authenticationlistener"></a><span data-ttu-id="cd3da-139">Exemplo 2: Expanda invokeUserFlowListener para uma autenticação específicaListener</span><span class="sxs-lookup"><span data-stu-id="cd3da-139">Example 2: Expand invokeUserFlowListener for a specific authenticationListener</span></span>

<span data-ttu-id="cd3da-140">O exemplo a seguir obtém o ouvinte por id do evento onSignupStart e expande o fluxo de usuário invocado.</span><span class="sxs-lookup"><span data-stu-id="cd3da-140">The following example gets the listener by id for the onSignupStart event and expands the user flow that is invoked.</span></span>

#### <a name="request"></a><span data-ttu-id="cd3da-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd3da-141">Request</span></span>

<span data-ttu-id="cd3da-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd3da-142">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_authenticationlistener_invokeuserflowlistener"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}?$expand=microsoft.graph.invokeUserFlowAction/userFlow
```

#### <a name="response"></a><span data-ttu-id="cd3da-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd3da-143">Response</span></span>

<span data-ttu-id="cd3da-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cd3da-144">The following is an example of the response.</span></span>

<span data-ttu-id="cd3da-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cd3da-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.invokeUserFlowListener"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/events/onSignUpStart(microsoft.graph.invokeUserFlowListener/userFlow())/$entity",
  "@odata.type": "#microsoft.graph.invokeUserFlowListener",
  "id": "2adb5c12-5c12-2adb-125c-db2a125cdb2a",
  "priority": 101,
  "sourceFilter": {
      "includeApplications": [
          "3dfff01b-0afb-4a07-967f-d1ccbd81102a"
      ]
  },
  "userFlow": {
      "id": "B2X_1_Partner",
      "userFlowType": "signUpOrSignIn",
      "userFlowTypeVersion": 1
  }
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Get authenticationListener",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: get_authenticationlistener_invokeuserflowlistener/userFlow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: get_authenticationlistener_invokeuserflowlistener/userFlow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
