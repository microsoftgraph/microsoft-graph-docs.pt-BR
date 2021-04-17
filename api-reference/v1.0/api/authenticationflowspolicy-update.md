---
title: Atualizar authenticationFlowsPolicy
description: Atualize a propriedade booleana selfServiceSignUp de um objeto authenticationFlowsPolicy.
author: linkhp
localization_priority: Priority
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d81986c75cb636c45488d2fb35e69b05fdb06e2a
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882858"
---
# <a name="update-authenticationflowspolicy"></a><span data-ttu-id="a52ab-103">Atualizar authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="a52ab-103">Update authenticationFlowsPolicy</span></span>

<span data-ttu-id="a52ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a52ab-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a52ab-105">Atualize a propriedade **selfServiceSignUp** de um objeto [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a52ab-105">Update the **selfServiceSignUp** property of an [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object.</span></span> <span data-ttu-id="a52ab-106">As propriedades **id**, **tipo** e **descrição** não podem ser modificadas.</span><span class="sxs-lookup"><span data-stu-id="a52ab-106">The properties **id**, **type**, and **description** cannot be modified.</span></span>

## <a name="permissions"></a><span data-ttu-id="a52ab-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a52ab-107">Permissions</span></span>

<span data-ttu-id="a52ab-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a52ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a52ab-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a52ab-110">Permission type</span></span>|<span data-ttu-id="a52ab-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a52ab-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a52ab-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a52ab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a52ab-113">Policy.ReadWrite.AuthenticationFlows</span><span class="sxs-lookup"><span data-stu-id="a52ab-113">Policy.ReadWrite.AuthenticationFlows</span></span>|
|<span data-ttu-id="a52ab-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a52ab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a52ab-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="a52ab-115">Not Supported</span></span>|
|<span data-ttu-id="a52ab-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a52ab-116">Application</span></span>|<span data-ttu-id="a52ab-117">Policy.ReadWrite.AuthenticationFlows</span><span class="sxs-lookup"><span data-stu-id="a52ab-117">Policy.ReadWrite.AuthenticationFlows</span></span>|

## <a name="http-request"></a><span data-ttu-id="a52ab-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a52ab-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /policies/authenticationFlowsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="a52ab-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a52ab-119">Request headers</span></span>

|<span data-ttu-id="a52ab-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a52ab-120">Name</span></span>|<span data-ttu-id="a52ab-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a52ab-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a52ab-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a52ab-122">Authorization</span></span>|<span data-ttu-id="a52ab-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a52ab-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a52ab-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a52ab-125">Content-Type</span></span>|<span data-ttu-id="a52ab-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a52ab-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a52ab-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a52ab-128">Request body</span></span>

<span data-ttu-id="a52ab-129">No corpo da solicitação, você pode fornecer uma representação JSON do objeto [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a52ab-129">In the request body, you can supply a JSON representation of the [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object.</span></span>

<span data-ttu-id="a52ab-130">A tabela a seguir mostra as propriedades obrigatórias ao atualizar [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a52ab-130">The following table shows the properties that are required when you update the [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md).</span></span>

|<span data-ttu-id="a52ab-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a52ab-131">Property</span></span>|<span data-ttu-id="a52ab-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="a52ab-132">Type</span></span>|<span data-ttu-id="a52ab-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="a52ab-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a52ab-134">selfServiceSignUp</span><span class="sxs-lookup"><span data-stu-id="a52ab-134">selfServiceSignUp</span></span>|[<span data-ttu-id="a52ab-135">selfServiceSignUpAuthenticationFlowConfiguration</span><span class="sxs-lookup"><span data-stu-id="a52ab-135">selfServiceSignUpAuthenticationFlowConfiguration</span></span>](../resources/selfservicesignupauthenticationflowconfiguration.md)|<span data-ttu-id="a52ab-136">Configuração de inscrição de autoatendimento.</span><span class="sxs-lookup"><span data-stu-id="a52ab-136">Self-service sign-up configuration.</span></span>|

## <a name="response"></a><span data-ttu-id="a52ab-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a52ab-137">Response</span></span>

<span data-ttu-id="a52ab-138">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.</span><span class="sxs-lookup"><span data-stu-id="a52ab-138">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="a52ab-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a52ab-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="a52ab-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a52ab-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_authenticationflowspolicy"
}
-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authenticationFlowsPolicy
Content-Type: application/json

{
  "selfServiceSignUp": {
    "isEnabled": true
  }
}
```

### <a name="response"></a><span data-ttu-id="a52ab-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="a52ab-141">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

``` http
HTTP/1.1 204 No Content
```
