---
title: Listar ouvintes onSignUpStart
description: Obter a coleção de recursos authenticationListener suportados pelo evento onSignupStart.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 346db0f1085190252b2bb8e48dcfcb8adfc23f61
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872363"
---
# <a name="list-onsignupstart-listeners"></a><span data-ttu-id="96e13-103">Listar ouvintes onSignUpStart</span><span class="sxs-lookup"><span data-stu-id="96e13-103">List onSignUpStart listeners</span></span>

<span data-ttu-id="96e13-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96e13-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96e13-105">Obter a coleção de recursos authenticationListener suportados pelo evento onSignupStart.</span><span class="sxs-lookup"><span data-stu-id="96e13-105">Get the collection of authenticationListener resources supported by the onSignupStart event.</span></span> <span data-ttu-id="96e13-106">O evento onSignUpStart dá suporte ao [tipo invokeUserFlowListener.](../resources/invokeuserflowlistener.md)</span><span class="sxs-lookup"><span data-stu-id="96e13-106">The onSignUpStart event supports the [invokeUserFlowListener](../resources/invokeuserflowlistener.md) type.</span></span>

<span data-ttu-id="96e13-107">Quando um [invokeUserFlowListener](../resources/invokeuserflowlistener.md) é atribuído [a](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) um evento onSignUpStart, um aplicativo é associado a um fluxo de usuário, habilitando um processo de inscrição de autoatendente nele.</span><span class="sxs-lookup"><span data-stu-id="96e13-107">When an [invokeUserFlowListener](../resources/invokeuserflowlistener.md) is assigned to an onSignUpStart event, an application is associated with a user flow, therefore enabling a [self-service sign up](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) process on it.</span></span> <span data-ttu-id="96e13-108">Depois que o evento de autenticação para invocar um fluxo de usuário é criado, os usuários que vão para esse aplicativo poderão iniciar um fluxo de inscrição que provisiona uma conta de convidado.</span><span class="sxs-lookup"><span data-stu-id="96e13-108">Once the authentication event for invoking a user flow is created, users who go to that application will be able to initiate a sign-up flow that provisions a guest account.</span></span>

## <a name="permissions"></a><span data-ttu-id="96e13-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="96e13-109">Permissions</span></span>

<span data-ttu-id="96e13-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96e13-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96e13-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96e13-112">Permission type</span></span>|<span data-ttu-id="96e13-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="96e13-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96e13-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96e13-114">Delegated (work or school account)</span></span>|<span data-ttu-id="96e13-115">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="96e13-115">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span>|
|<span data-ttu-id="96e13-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96e13-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96e13-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96e13-117">Not supported.</span></span>|
|<span data-ttu-id="96e13-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96e13-118">Application</span></span>|<span data-ttu-id="96e13-119">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="96e13-119">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span>|

## <a name="http-request"></a><span data-ttu-id="96e13-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96e13-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/events/onSignupStart
```

## <a name="optional-query-parameters"></a><span data-ttu-id="96e13-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="96e13-121">Optional query parameters</span></span>

<span data-ttu-id="96e13-122">Esse método dá suporte `$expand` ao parâmetro de consulta OData para expandir os detalhes de um invokeUserFlowListener.</span><span class="sxs-lookup"><span data-stu-id="96e13-122">This method supports the `$expand` OData query parameter to expand the details of an invokeUserFlowListener.</span></span> <span data-ttu-id="96e13-123">Veja abaixo um exemplo.</span><span class="sxs-lookup"><span data-stu-id="96e13-123">See below for an example.</span></span> <span data-ttu-id="96e13-124">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="96e13-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="96e13-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96e13-125">Request headers</span></span>

|<span data-ttu-id="96e13-126">Nome</span><span class="sxs-lookup"><span data-stu-id="96e13-126">Name</span></span>|<span data-ttu-id="96e13-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="96e13-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="96e13-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="96e13-128">Authorization</span></span>|<span data-ttu-id="96e13-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96e13-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="96e13-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96e13-131">Request body</span></span>

<span data-ttu-id="96e13-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="96e13-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96e13-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="96e13-133">Response</span></span>

<span data-ttu-id="96e13-134">Se bem-sucedido, este método retorna um código de resposta e uma `200 OK` coleção de [objetos authenticationListener](../resources/authenticationlistener.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96e13-134">If successful, this method returns a `200 OK` response code and a collection of [authenticationListener](../resources/authenticationlistener.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="96e13-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="96e13-135">Examples</span></span>

### <a name="example-1-list-authenticationlisteners-for-the-onsignupstart-event"></a><span data-ttu-id="96e13-136">Exemplo 1: Listar authenticationListeners para o evento onSignUpStart</span><span class="sxs-lookup"><span data-stu-id="96e13-136">Example 1: List authenticationListeners for the onSignUpStart event</span></span>

#### <a name="request"></a><span data-ttu-id="96e13-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96e13-137">Request</span></span>

<span data-ttu-id="96e13-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="96e13-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_authenticationlistener"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/events/onSignupStart
```

#### <a name="response"></a><span data-ttu-id="96e13-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="96e13-139">Response</span></span>

<span data-ttu-id="96e13-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="96e13-140">The following is an example of the response.</span></span>

<span data-ttu-id="96e13-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="96e13-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.authenticationListener)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/events/onSignUpStart",
  "value": [
    {
      "@odata.type": "#microsoft.graph.invokeUserFlowListener",
      "id": "2adb5c12-5c12-2adb-125c-db2a125cdb2a",
      "priority": 101,
      "sourceFilter": {
        "includeApplications": [
            "3dfff01b-0afb-4a07-967f-d1ccbd81102a"
        ]
      }
    },
    {
      "@odata.type": "#Microsoft.Graph.InvokeUserFlowListener",
      "id": "0a09997f-fa0c-4f3c-9d02-76762ac069c8",
      "priority": 100,
      "sourceFilter": {
          "includeApplications": [
              "b0e1638f-4c39-4cd1-82b3-91d1caef65f8"
        ]
      }
    }
  ]
}
```

### <a name="example-2-expand-invokeuserflowlisteners-in-authenticationlisteners-for-the-onsignupstart-event"></a><span data-ttu-id="96e13-142">Exemplo 2: Expandir invokeUserFlowListeners em authenticationListeners para o evento onSignUpStart</span><span class="sxs-lookup"><span data-stu-id="96e13-142">Example 2: Expand invokeUserFlowListeners in authenticationListeners for the onSignUpStart event</span></span>

<span data-ttu-id="96e13-143">O exemplo a seguir lista os ouvintes definidos para o evento onSignupStart e, para cada ouvinte, expande o fluxo do usuário invocado.</span><span class="sxs-lookup"><span data-stu-id="96e13-143">The following example lists the listeners defined for the onSignupStart event, and for each listener, expands the user flow that is invoked.</span></span>

#### <a name="request"></a><span data-ttu-id="96e13-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96e13-144">Request</span></span>

<span data-ttu-id="96e13-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="96e13-145">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_authenticationlistener_invokeuserflowlistener"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/events/onSignupStart?$expand=microsoft.graph.invokeUserFlowListener/userFlow
```

#### <a name="response"></a><span data-ttu-id="96e13-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="96e13-146">Response</span></span>

<span data-ttu-id="96e13-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="96e13-147">The following is an example of the response.</span></span>

<span data-ttu-id="96e13-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="96e13-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.invokeUserFlowListener)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/events/onSignUpStart(microsoft.graph.invokeUserFlowListener/userFlow())/$entity",
  "value": [
    {
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
    },
    {
      "@odata.type": "#microsoft.graph.InvokeUserFlowListener",
      "id": "0a09997f-fa0c-4f3c-9d02-76762ac069c8",
      "priority": 100,
      "sourceFilter": {
        "includeApplications": [
            "b0e1638f-4c39-4cd1-82b3-91d1caef65f8"
        ]
      },
      "userFlow": {
            "id": "B2X_1_Partner",
            "userFlowType": "signUpOrSignIn",
            "userFlowTypeVersion": 1
      }
    }
  ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "List onSignUpStart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: list_authenticationlistener_invokeuserflowlistener/container/userFlow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: list_authenticationlistener_invokeuserflowlistener/container/userFlow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
