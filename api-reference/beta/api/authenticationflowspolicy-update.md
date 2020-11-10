---
title: Atualizar authenticationFlowsPolicy
description: Atualize a propriedade booleana selfServiceSignUp de um objeto authenticationFlowsPolicy.
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 57c9428d8a0d946282be96ad5d2631f51b808659
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961369"
---
# <a name="update-authenticationflowspolicy"></a><span data-ttu-id="bca29-103">Atualizar authenticationFlowsPolicy</span><span class="sxs-lookup"><span data-stu-id="bca29-103">Update authenticationFlowsPolicy</span></span>

<span data-ttu-id="bca29-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bca29-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bca29-105">Atualize a propriedade booleana **selfServiceSignUp** de um objeto [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bca29-105">Update the Boolean **selfServiceSignUp** property of an [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object.</span></span> <span data-ttu-id="bca29-106">As propriedades **id** , **tipo** e **descrição** não podem ser modificadas.</span><span class="sxs-lookup"><span data-stu-id="bca29-106">The properties **id** , **type** , and **description** cannot be modified.</span></span>

## <a name="permissions"></a><span data-ttu-id="bca29-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="bca29-107">Permissions</span></span>
<span data-ttu-id="bca29-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bca29-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bca29-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bca29-110">Permission type</span></span>|<span data-ttu-id="bca29-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bca29-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bca29-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bca29-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bca29-113">Policy.ReadWrite.AuthenticationFlows</span><span class="sxs-lookup"><span data-stu-id="bca29-113">Policy.ReadWrite.AuthenticationFlows</span></span>|
|<span data-ttu-id="bca29-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bca29-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bca29-115">Não suportado</span><span class="sxs-lookup"><span data-stu-id="bca29-115">Not Supported</span></span>|
|<span data-ttu-id="bca29-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bca29-116">Application</span></span>|<span data-ttu-id="bca29-117">Policy.ReadWrite.AuthenticationFlows</span><span class="sxs-lookup"><span data-stu-id="bca29-117">Policy.ReadWrite.AuthenticationFlows</span></span>|

## <a name="http-request"></a><span data-ttu-id="bca29-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bca29-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationFlowsPolicy
```

## <a name="request-headers"></a><span data-ttu-id="bca29-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bca29-119">Request headers</span></span>
|<span data-ttu-id="bca29-120">Nome</span><span class="sxs-lookup"><span data-stu-id="bca29-120">Name</span></span>|<span data-ttu-id="bca29-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="bca29-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bca29-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bca29-122">Authorization</span></span>|<span data-ttu-id="bca29-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bca29-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="bca29-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bca29-125">Content-Type</span></span>|<span data-ttu-id="bca29-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bca29-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bca29-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bca29-128">Request body</span></span>
<span data-ttu-id="bca29-129">No corpo da solicitação, você pode fornecer uma representação JSON do objeto [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) (mas não é obrigatório).</span><span class="sxs-lookup"><span data-stu-id="bca29-129">In the request body, you can supply a JSON representation of the [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object (but is not required.)</span></span>

<span data-ttu-id="bca29-130">A tabela a seguir mostra as propriedades obrigatórias ao atualizar [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md).</span><span class="sxs-lookup"><span data-stu-id="bca29-130">The following table shows the properties that are required when you update the [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md).</span></span>

|<span data-ttu-id="bca29-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bca29-131">Property</span></span>|<span data-ttu-id="bca29-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="bca29-132">Type</span></span>|<span data-ttu-id="bca29-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="bca29-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bca29-134">selfServiceSignUp</span><span class="sxs-lookup"><span data-stu-id="bca29-134">selfServiceSignUp</span></span>|[<span data-ttu-id="bca29-135">selfServiceSignUpAuthenticationFlowConfiguration</span><span class="sxs-lookup"><span data-stu-id="bca29-135">selfServiceSignUpAuthenticationFlowConfiguration</span></span>](../resources/selfservicesignupauthenticationflowconfiguration.md)|<span data-ttu-id="bca29-136">Configuração de inscrição de autoatendimento.</span><span class="sxs-lookup"><span data-stu-id="bca29-136">Self-service sign-up configuration.</span></span>|

## <a name="response"></a><span data-ttu-id="bca29-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="bca29-137">Response</span></span>

<span data-ttu-id="bca29-138">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.</span><span class="sxs-lookup"><span data-stu-id="bca29-138">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="bca29-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bca29-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="bca29-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bca29-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="bca29-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="bca29-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="bca29-142">C#</span><span class="sxs-lookup"><span data-stu-id="bca29-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authenticationflowspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bca29-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bca29-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authenticationflowspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bca29-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bca29-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authenticationflowspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bca29-145">Java</span><span class="sxs-lookup"><span data-stu-id="bca29-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authenticationflowspolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bca29-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="bca29-146">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
``` http
HTTP/1.1 204 No Content
```


