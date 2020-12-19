---
title: Atualizar identityApiConnector
description: Atualiza as propriedades de um objeto identityApiConnector.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e06927b3058f78396d9df6d54e7336ff6ba1b521
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720084"
---
# <a name="update-identityapiconnector"></a><span data-ttu-id="9b3e6-103">Atualizar identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="9b3e6-103">Update identityApiConnector</span></span>

<span data-ttu-id="9b3e6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b3e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b3e6-105">Atualiza as propriedades de um objeto [identityApiConnector](../resources/identityapiconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="9b3e6-105">Update the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b3e6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9b3e6-106">Permissions</span></span>

<span data-ttu-id="9b3e6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b3e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9b3e6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b3e6-109">Permission type</span></span>                        | <span data-ttu-id="9b3e6-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9b3e6-110">Permissions (from most to least privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="9b3e6-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b3e6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9b3e6-112">APIConnectors. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9b3e6-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="9b3e6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b3e6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b3e6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b3e6-114">Not supported.</span></span>  |
| <span data-ttu-id="9b3e6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9b3e6-115">Application</span></span>                            | <span data-ttu-id="9b3e6-116">APIConnectors. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9b3e6-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="9b3e6-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="9b3e6-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="9b3e6-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="9b3e6-118">Global administrator</span></span>
* <span data-ttu-id="9b3e6-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="9b3e6-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="9b3e6-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b3e6-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/apiConnectors/{identityApiConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="9b3e6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b3e6-121">Request headers</span></span>
|<span data-ttu-id="9b3e6-122">Nome</span><span class="sxs-lookup"><span data-stu-id="9b3e6-122">Name</span></span>|<span data-ttu-id="9b3e6-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b3e6-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9b3e6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b3e6-124">Authorization</span></span>|<span data-ttu-id="9b3e6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b3e6-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9b3e6-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9b3e6-127">Content-Type</span></span>|<span data-ttu-id="9b3e6-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b3e6-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b3e6-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b3e6-130">Request body</span></span>
<span data-ttu-id="9b3e6-131">No corpo da solicitação, forneça uma representação JSON do objeto [identityApiConnector](../resources/identityapiconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="9b3e6-131">In the request body, supply a JSON representation of the [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

<span data-ttu-id="9b3e6-132">A tabela a seguir mostra as propriedades do [identityApiConnector](../resources/identityapiconnector.md) que podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="9b3e6-132">The following table shows the properties of the [identityApiConnector](../resources/identityapiconnector.md) that can be updated.</span></span>


|<span data-ttu-id="9b3e6-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b3e6-133">Property</span></span>|<span data-ttu-id="9b3e6-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b3e6-134">Type</span></span>|<span data-ttu-id="9b3e6-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b3e6-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b3e6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9b3e6-136">displayName</span></span>|<span data-ttu-id="9b3e6-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b3e6-137">String</span></span>| <span data-ttu-id="9b3e6-138">O nome do conector da API.</span><span class="sxs-lookup"><span data-stu-id="9b3e6-138">The name of the API connector.</span></span> |
|<span data-ttu-id="9b3e6-139">targetUrl</span><span class="sxs-lookup"><span data-stu-id="9b3e6-139">targetUrl</span></span>|<span data-ttu-id="9b3e6-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b3e6-140">String</span></span>| <span data-ttu-id="9b3e6-141">A URL do ponto de extremidade da API a ser chamado.</span><span class="sxs-lookup"><span data-stu-id="9b3e6-141">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="9b3e6-142">authenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="9b3e6-142">authenticationConfiguration</span></span>|[<span data-ttu-id="9b3e6-143">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="9b3e6-143">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="9b3e6-144">O objeto que descreve os detalhes de configuração de autenticação para chamar a API.</span><span class="sxs-lookup"><span data-stu-id="9b3e6-144">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="9b3e6-145">Só há suporte para a [autenticação básica](../resources/basicauthentication.md) no momento.</span><span class="sxs-lookup"><span data-stu-id="9b3e6-145">Only [Basic authentication](../resources/basicauthentication.md) is supported at this time.</span></span> <span data-ttu-id="9b3e6-146">Todas as propriedades do apiAuthenticationConfigurationBase devem ser definidas ao mesmo tempo, como nome de usuário e senha.</span><span class="sxs-lookup"><span data-stu-id="9b3e6-146">All properties of the apiAuthenticationConfigurationBase must be set at the same time, like both username and password.</span></span>|

## <a name="response"></a><span data-ttu-id="9b3e6-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b3e6-147">Response</span></span>

<span data-ttu-id="9b3e6-148">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9b3e6-148">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="9b3e6-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9b3e6-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9b3e6-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b3e6-150">Request</span></span>

<span data-ttu-id="9b3e6-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b3e6-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_identityapiconnector"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/apiConnectors/{identityApiConnectorId}
Content-Type: application/json

{
  "displayName": "New Test API",
  "targetUrl": "https://otherapi.com/api/endpoint",
  "authenticationConfiguration": {
    "@odata.type": "microsoft.graph.basicAuthentication",
    "username":"<NEW_USERNAME>", 
    "password":"<NEW_PASSWORD>"
  }
}
```

### <a name="response"></a><span data-ttu-id="9b3e6-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b3e6-152">Response</span></span>

<span data-ttu-id="9b3e6-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9b3e6-153">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```
