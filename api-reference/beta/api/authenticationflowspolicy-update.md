---
title: Atualizar authenticationFlowsPolicy
description: Atualize a propriedade Boolean selfServiceSignUp de um objeto authenticationFlowsPolicy.
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 626e1dc8a851f2c8da6a9bb815a4e783cf44e7d2
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556370"
---
# <a name="update-authenticationflowspolicy"></a><span data-ttu-id="dbb4e-103">Atualizar authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="dbb4e-103">Update authenticationFlowsPolicy</span></span>

<span data-ttu-id="dbb4e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbb4e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dbb4e-105">Atualize a propriedade Boolean **selfServiceSignUp** de um objeto [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="dbb4e-105">Update the Boolean **selfServiceSignUp** property of an [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object.</span></span> <span data-ttu-id="dbb4e-106">Não é possível modificar a **identificação**, o **tipo**e a **Descrição** das propriedades.</span><span class="sxs-lookup"><span data-stu-id="dbb4e-106">The properties **id**, **type**, and **description** cannot be modified.</span></span>

## <a name="permissions"></a><span data-ttu-id="dbb4e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="dbb4e-107">Permissions</span></span>
<span data-ttu-id="dbb4e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dbb4e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbb4e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dbb4e-110">Permission type</span></span>|<span data-ttu-id="dbb4e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dbb4e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dbb4e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dbb4e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dbb4e-113">Policy. ReadWrite. AuthenticationFlows</span><span class="sxs-lookup"><span data-stu-id="dbb4e-113">Policy.ReadWrite.AuthenticationFlows</span></span>|
|<span data-ttu-id="dbb4e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dbb4e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dbb4e-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="dbb4e-115">Not Supported</span></span>|
|<span data-ttu-id="dbb4e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dbb4e-116">Application</span></span>|<span data-ttu-id="dbb4e-117">Policy. ReadWrite. AuthenticationFlows</span><span class="sxs-lookup"><span data-stu-id="dbb4e-117">Policy.ReadWrite.AuthenticationFlows</span></span>|

## <a name="http-request"></a><span data-ttu-id="dbb4e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dbb4e-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationFlowsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="dbb4e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dbb4e-119">Request headers</span></span>
|<span data-ttu-id="dbb4e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="dbb4e-120">Name</span></span>|<span data-ttu-id="dbb4e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbb4e-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="dbb4e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dbb4e-122">Authorization</span></span>|<span data-ttu-id="dbb4e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbb4e-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="dbb4e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dbb4e-125">Content-Type</span></span>|<span data-ttu-id="dbb4e-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dbb4e-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbb4e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dbb4e-128">Request body</span></span>
<span data-ttu-id="dbb4e-129">No corpo da solicitação, você pode fornecer uma representação JSON do objeto [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) (mas não é obrigatório).</span><span class="sxs-lookup"><span data-stu-id="dbb4e-129">In the request body, you can supply a JSON representation of the [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object (but is not required.)</span></span>

<span data-ttu-id="dbb4e-130">A tabela a seguir mostra as propriedades que são necessárias ao atualizar o [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="dbb4e-130">The following table shows the properties that are required when you update the [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md).</span></span>

|<span data-ttu-id="dbb4e-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dbb4e-131">Property</span></span>|<span data-ttu-id="dbb4e-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbb4e-132">Type</span></span>|<span data-ttu-id="dbb4e-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbb4e-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbb4e-134">selfServiceSignUp</span><span class="sxs-lookup"><span data-stu-id="dbb4e-134">selfServiceSignUp</span></span>|[<span data-ttu-id="dbb4e-135">selfServiceSignUpAuthenticationFlowConfiguration</span><span class="sxs-lookup"><span data-stu-id="dbb4e-135">selfServiceSignUpAuthenticationFlowConfiguration</span></span>](../resources/selfservicesignupauthenticationflowconfiguration.md)|<span data-ttu-id="dbb4e-136">Configuração de inscrição de autoatendimento.</span><span class="sxs-lookup"><span data-stu-id="dbb4e-136">Self-service sign-up configuration.</span></span>|

## <a name="response"></a><span data-ttu-id="dbb4e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbb4e-137">Response</span></span>

<span data-ttu-id="dbb4e-138">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.</span><span class="sxs-lookup"><span data-stu-id="dbb4e-138">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbb4e-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dbb4e-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="dbb4e-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dbb4e-140">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_authenticationflowspolicy"
}
-->
```http
PATCH https://graph.microsoft.com/beta/policies/authenticationFlowsPolicy
Content-Type: application/json

{
  "selfServiceSignUp": {
    "isEnabled": true
  }
}
```

### <a name="response"></a><span data-ttu-id="dbb4e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="dbb4e-141">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
``` http
HTTP/1.1 204 No Content
```
