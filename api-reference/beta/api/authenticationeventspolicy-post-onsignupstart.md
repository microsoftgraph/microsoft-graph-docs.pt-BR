---
title: Criar authenticationListener
description: Crie um novo objeto authenticationListener para o evento onSignUpStart.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c24ceff80c873181799ea38fbe23c6054f876bc7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438530"
---
# <a name="create-authenticationlistener"></a><span data-ttu-id="8ae54-103">Criar authenticationListener</span><span class="sxs-lookup"><span data-stu-id="8ae54-103">Create authenticationListener</span></span>

<span data-ttu-id="8ae54-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ae54-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ae54-105">Crie um novo objeto authenticationListener para o evento onSignUpStart.</span><span class="sxs-lookup"><span data-stu-id="8ae54-105">Create a new authenticationListener object for the onSignUpStart event.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ae54-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8ae54-106">Permissions</span></span>

<span data-ttu-id="8ae54-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ae54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ae54-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ae54-109">Permission type</span></span>|<span data-ttu-id="8ae54-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ae54-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ae54-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ae54-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8ae54-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ae54-112">Policy.ReadWrite.ApplicationConfiguration</span></span>|
|<span data-ttu-id="8ae54-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ae54-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ae54-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ae54-114">Not supported.</span></span>|
|<span data-ttu-id="8ae54-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ae54-115">Application</span></span>|<span data-ttu-id="8ae54-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ae54-116">Policy.ReadWrite.ApplicationConfiguration</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ae54-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ae54-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identity/events/onSignupStart
```

## <a name="request-headers"></a><span data-ttu-id="8ae54-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ae54-118">Request headers</span></span>

|<span data-ttu-id="8ae54-119">Nome</span><span class="sxs-lookup"><span data-stu-id="8ae54-119">Name</span></span>|<span data-ttu-id="8ae54-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ae54-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8ae54-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ae54-121">Authorization</span></span>|<span data-ttu-id="8ae54-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ae54-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8ae54-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8ae54-124">Content-Type</span></span>|<span data-ttu-id="8ae54-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ae54-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ae54-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ae54-127">Request body</span></span>

<span data-ttu-id="8ae54-128">No corpo da solicitação, fornece uma representação JSON do [objeto authenticationListener.](../resources/authenticationlistener.md)</span><span class="sxs-lookup"><span data-stu-id="8ae54-128">In the request body, supply a JSON representation of the [authenticationListener](../resources/authenticationlistener.md) object.</span></span>

<span data-ttu-id="8ae54-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [a autenticação invokeUserFlowListenerListener.](../resources/invokeuserflowlistener.md)</span><span class="sxs-lookup"><span data-stu-id="8ae54-129">The following table shows the properties that are required when you create the [invokeUserFlowListener](../resources/invokeuserflowlistener.md) authenticationListener.</span></span>

|<span data-ttu-id="8ae54-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ae54-130">Property</span></span>|<span data-ttu-id="8ae54-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ae54-131">Type</span></span>|<span data-ttu-id="8ae54-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ae54-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ae54-133">Prioridade</span><span class="sxs-lookup"><span data-stu-id="8ae54-133">priority</span></span>|<span data-ttu-id="8ae54-134">Int32</span><span class="sxs-lookup"><span data-stu-id="8ae54-134">Int32</span></span>|<span data-ttu-id="8ae54-135">A prioridade do ouvinte.</span><span class="sxs-lookup"><span data-stu-id="8ae54-135">The priority of the listener.</span></span> <span data-ttu-id="8ae54-136">Determina a ordem de avaliação quando um evento tem vários ouvintes.</span><span class="sxs-lookup"><span data-stu-id="8ae54-136">Determines the order of evaluation when an event has multiple listeners.</span></span> <span data-ttu-id="8ae54-137">A prioridade é avaliada de baixo para alto.</span><span class="sxs-lookup"><span data-stu-id="8ae54-137">The priority is evaluated from low to high.</span></span>|
|<span data-ttu-id="8ae54-138">sourceFilter</span><span class="sxs-lookup"><span data-stu-id="8ae54-138">sourceFilter</span></span>|[<span data-ttu-id="8ae54-139">authenticationSourceFilter</span><span class="sxs-lookup"><span data-stu-id="8ae54-139">authenticationSourceFilter</span></span>](../resources/authenticationsourcefilter.md)|<span data-ttu-id="8ae54-140">Filtrar com base na origem da autenticação usada para determinar se o ouvinte é avaliado.</span><span class="sxs-lookup"><span data-stu-id="8ae54-140">Filter based on the source of the authentication that is used to determine whether the listener is evaluated.</span></span> <span data-ttu-id="8ae54-141">No momento, isso está limitado a avaliações com base no aplicativo ao que o usuário está autenticando.</span><span class="sxs-lookup"><span data-stu-id="8ae54-141">This is currently limited to evaluations based on application the user is authenticating to.</span></span>|
|<span data-ttu-id="8ae54-142">userFlow</span><span class="sxs-lookup"><span data-stu-id="8ae54-142">userFlow</span></span>|[<span data-ttu-id="8ae54-143">b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="8ae54-143">b2xIdentityUserFlow</span></span>](../resources/b2xidentityuserflow.md)|<span data-ttu-id="8ae54-144">O [objeto b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) que será invocado quando essa ação for avaliada.</span><span class="sxs-lookup"><span data-stu-id="8ae54-144">The [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object that will be invoked when this action is evaluated.</span></span>|

## <a name="response"></a><span data-ttu-id="8ae54-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ae54-145">Response</span></span>

<span data-ttu-id="8ae54-146">Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [authenticationListener](../resources/authenticationlistener.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ae54-146">If successful, this method returns a `201 Created` response code and an [authenticationListener](../resources/authenticationlistener.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8ae54-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8ae54-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8ae54-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ae54-148">Request</span></span>

<span data-ttu-id="8ae54-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ae54-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_authenticationlistener_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/events/onSignupStart
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.invokeUserFlowListener",
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

### <a name="response"></a><span data-ttu-id="8ae54-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ae54-150">Response</span></span>

<span data-ttu-id="8ae54-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8ae54-151">The following is an example of the response.</span></span>

<span data-ttu-id="8ae54-152">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8ae54-152">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationListener"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/events/onSignupStart/Microsoft.Graph.InvokeUserFlowListener/$entity",
    "@odata.type": "#microsoft.graph.invokeUserFlowListener",
    "id": "2be3336b-e3b4-44f3-9128-b6fd9ad39bb8",
    "priority": 101,
    "sourceFilter": {
        "includeApplications": [
            "1fc41a76-3050-4529-8095-9af8897cf63d"
        ]
    }
}
```
