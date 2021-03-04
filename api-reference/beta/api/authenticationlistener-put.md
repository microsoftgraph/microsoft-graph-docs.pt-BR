---
title: Colocar authenticationListener
description: Substitua um objeto authenticationListener.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6e41dde2a8c22394fd28fe3730ac44655c7eb310
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438446"
---
# <a name="put-authenticationlistener"></a><span data-ttu-id="0ddb9-103">Colocar authenticationListener</span><span class="sxs-lookup"><span data-stu-id="0ddb9-103">Put authenticationListener</span></span>

<span data-ttu-id="0ddb9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ddb9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ddb9-105">Substitua um [authenticationListener definido](../resources/authenticationlistener.md) para o evento onSignupStart no pipeline de autenticação.</span><span class="sxs-lookup"><span data-stu-id="0ddb9-105">Replace an [authenticationListener](../resources/authenticationlistener.md) defined for the onSignupStart event in the authentication pipeline.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ddb9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0ddb9-106">Permissions</span></span>

<span data-ttu-id="0ddb9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ddb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ddb9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ddb9-109">Permission type</span></span>|<span data-ttu-id="0ddb9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0ddb9-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ddb9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ddb9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0ddb9-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="0ddb9-112">Policy.ReadWrite.ApplicationConfiguration</span></span>|
|<span data-ttu-id="0ddb9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ddb9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ddb9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ddb9-114">Not supported.</span></span>|
|<span data-ttu-id="0ddb9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ddb9-115">Application</span></span>|<span data-ttu-id="0ddb9-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="0ddb9-116">Policy.ReadWrite.ApplicationConfiguration</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ddb9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ddb9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PUT /identity/events/onSignupStart/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0ddb9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ddb9-118">Request headers</span></span>

|<span data-ttu-id="0ddb9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0ddb9-119">Name</span></span>|<span data-ttu-id="0ddb9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ddb9-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0ddb9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ddb9-121">Authorization</span></span>|<span data-ttu-id="0ddb9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ddb9-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0ddb9-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0ddb9-124">Content-Type</span></span>|<span data-ttu-id="0ddb9-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ddb9-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ddb9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ddb9-127">Request body</span></span>

<span data-ttu-id="0ddb9-128">No corpo da solicitação, fornece uma representação JSON do [objeto authenticationListener.](../resources/authenticationlistener.md)</span><span class="sxs-lookup"><span data-stu-id="0ddb9-128">In the request body, supply a JSON representation of the [authenticationListener](../resources/authenticationlistener.md) object.</span></span>

<span data-ttu-id="0ddb9-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [invokeUserFlowListener](../resources/invokeuserflowlistener.md).</span><span class="sxs-lookup"><span data-stu-id="0ddb9-129">The following table shows the properties that are required when you create the [invokeUserFlowListener](../resources/invokeuserflowlistener.md).</span></span>

|<span data-ttu-id="0ddb9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ddb9-130">Property</span></span>|<span data-ttu-id="0ddb9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ddb9-131">Type</span></span>|<span data-ttu-id="0ddb9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ddb9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ddb9-133">Prioridade</span><span class="sxs-lookup"><span data-stu-id="0ddb9-133">priority</span></span>|<span data-ttu-id="0ddb9-134">Int32</span><span class="sxs-lookup"><span data-stu-id="0ddb9-134">Int32</span></span>|<span data-ttu-id="0ddb9-135">A prioridade do ouvinte.</span><span class="sxs-lookup"><span data-stu-id="0ddb9-135">The priority of the listener.</span></span> <span data-ttu-id="0ddb9-136">Determina a ordem de avaliação quando um evento tem vários ouvintes.</span><span class="sxs-lookup"><span data-stu-id="0ddb9-136">Determines the order of evaluation when an event has multiple listeners.</span></span> <span data-ttu-id="0ddb9-137">A prioridade é avaliada de baixo para alto.</span><span class="sxs-lookup"><span data-stu-id="0ddb9-137">The priority is evaluated from low to high.</span></span>|
|<span data-ttu-id="0ddb9-138">sourceFilter</span><span class="sxs-lookup"><span data-stu-id="0ddb9-138">sourceFilter</span></span>|[<span data-ttu-id="0ddb9-139">authenticationSourceFilter</span><span class="sxs-lookup"><span data-stu-id="0ddb9-139">authenticationSourceFilter</span></span>](../resources/authenticationsourcefilter.md)|<span data-ttu-id="0ddb9-140">Filtrar com base na origem da autenticação usada para determinar se o ouvinte é avaliado.</span><span class="sxs-lookup"><span data-stu-id="0ddb9-140">Filter based on the source of the authentication that is used to determine whether the listener is evaluated.</span></span> <span data-ttu-id="0ddb9-141">No momento, isso está limitado a avaliações com base no aplicativo ao que o usuário está autenticando.</span><span class="sxs-lookup"><span data-stu-id="0ddb9-141">This is currently limited to evaluations based on application the user is authenticating to.</span></span>|
|<span data-ttu-id="0ddb9-142">userFlow</span><span class="sxs-lookup"><span data-stu-id="0ddb9-142">userFlow</span></span>|[<span data-ttu-id="0ddb9-143">b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="0ddb9-143">b2xIdentityUserFlow</span></span>](../resources/b2xidentityuserflow.md)|<span data-ttu-id="0ddb9-144">A referência ao objeto de fluxo do usuário que é invocado nesta ação.</span><span class="sxs-lookup"><span data-stu-id="0ddb9-144">The reference to the user flow object that is invoked in this action.</span></span>|

## <a name="response"></a><span data-ttu-id="0ddb9-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ddb9-145">Response</span></span>

<span data-ttu-id="0ddb9-146">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0ddb9-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0ddb9-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0ddb9-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0ddb9-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ddb9-148">Request</span></span>

<span data-ttu-id="0ddb9-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ddb9-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "put_authenticationlistener_from_"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}
Content-Type: application/json

{
    "@odata.type": "#Microsoft.Graph.InvokeUserFlowListener",
    "priority": 101,
    "sourceFilter": {
        "includeApplications": [
            "1fc41a76-3050-4529-8095-9af8897cf63d"
        ]
    },
    "userFlow": {
        "id": "B2X_1_Partner"
    }
}
```

### <a name="response"></a><span data-ttu-id="0ddb9-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ddb9-150">Response</span></span>

<span data-ttu-id="0ddb9-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0ddb9-151">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
