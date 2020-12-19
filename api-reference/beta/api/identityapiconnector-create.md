---
title: Criar identityApiConnector
description: Criar um novo objeto identityApiConnector.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6665054307d601e80d02402a188f6412ab923ffc
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720079"
---
# <a name="create-identityapiconnector"></a><span data-ttu-id="e3d8c-103">Criar identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="e3d8c-103">Create identityApiConnector</span></span>

<span data-ttu-id="e3d8c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3d8c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3d8c-105">Criar um novo objeto [identityApiConnector](../resources/identityapiconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="e3d8c-105">Create a new [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3d8c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e3d8c-106">Permissions</span></span>

<span data-ttu-id="e3d8c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3d8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e3d8c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3d8c-109">Permission type</span></span>                        | <span data-ttu-id="e3d8c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e3d8c-110">Permissions (from most to least privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="e3d8c-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3d8c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3d8c-112">APIConnectors. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e3d8c-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="e3d8c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3d8c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3d8c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3d8c-114">Not supported.</span></span>  |
| <span data-ttu-id="e3d8c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3d8c-115">Application</span></span>                            | <span data-ttu-id="e3d8c-116">APIConnectors. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e3d8c-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="e3d8c-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="e3d8c-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="e3d8c-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="e3d8c-118">Global administrator</span></span>
* <span data-ttu-id="e3d8c-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="e3d8c-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="e3d8c-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3d8c-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /identity/apiConnectors
```

## <a name="request-headers"></a><span data-ttu-id="e3d8c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3d8c-121">Request headers</span></span>

| <span data-ttu-id="e3d8c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e3d8c-122">Name</span></span>          | <span data-ttu-id="e3d8c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3d8c-123">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="e3d8c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3d8c-124">Authorization</span></span> | <span data-ttu-id="e3d8c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3d8c-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="e3d8c-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e3d8c-127">Content-Type</span></span>  | <span data-ttu-id="e3d8c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3d8c-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3d8c-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3d8c-130">Request body</span></span>

<span data-ttu-id="e3d8c-131">No corpo da solicitação, forneça uma representação JSON do objeto [identityApiConnector](../resources/identityapiconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="e3d8c-131">In the request body, supply a JSON representation of the [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

<span data-ttu-id="e3d8c-132">A tabela a seguir mostra as propriedades que são necessárias ao criar [identityApiConnector](../resources/identityapiconnector.md).</span><span class="sxs-lookup"><span data-stu-id="e3d8c-132">The following table shows the properties that are required when you create the [identityApiConnector](../resources/identityapiconnector.md).</span></span>

|<span data-ttu-id="e3d8c-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3d8c-133">Property</span></span>|<span data-ttu-id="e3d8c-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3d8c-134">Type</span></span>|<span data-ttu-id="e3d8c-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3d8c-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3d8c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e3d8c-136">displayName</span></span>|<span data-ttu-id="e3d8c-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3d8c-137">String</span></span>| <span data-ttu-id="e3d8c-138">O nome do conector da API.</span><span class="sxs-lookup"><span data-stu-id="e3d8c-138">The name of the API connector.</span></span> |
|<span data-ttu-id="e3d8c-139">targetUrl</span><span class="sxs-lookup"><span data-stu-id="e3d8c-139">targetUrl</span></span>|<span data-ttu-id="e3d8c-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e3d8c-140">String</span></span>| <span data-ttu-id="e3d8c-141">A URL do ponto de extremidade da API a ser chamado.</span><span class="sxs-lookup"><span data-stu-id="e3d8c-141">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="e3d8c-142">authenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="e3d8c-142">authenticationConfiguration</span></span>|[<span data-ttu-id="e3d8c-143">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="e3d8c-143">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="e3d8c-144">O objeto que descreve os detalhes de configuração de autenticação para chamar a API.</span><span class="sxs-lookup"><span data-stu-id="e3d8c-144">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="e3d8c-145">Só há suporte para a [autenticação básica](../resources/basicauthentication.md) .</span><span class="sxs-lookup"><span data-stu-id="e3d8c-145">Only [Basic authentication](../resources/basicauthentication.md) is supported.</span></span>|

## <a name="response"></a><span data-ttu-id="e3d8c-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3d8c-146">Response</span></span>

<span data-ttu-id="e3d8c-147">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [identityApiConnector](../resources/identityapiconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3d8c-147">If successful, this method returns a `201 Created` response code and an [identityApiConnector](../resources/identityapiconnector.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e3d8c-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e3d8c-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e3d8c-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3d8c-149">Request</span></span>

<span data-ttu-id="e3d8c-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3d8c-150">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_identityapiconnector"
}
-->

```http
POST https://graph.microsoft.com/beta/identity/apiConnectors
Content-Type: application/json

{
    "displayName":"Test API",
    "targetUrl":"https://someapi.com/api",
    "authenticationConfiguration": {
      "@odata.type":"#microsoft.graph.basicAuthentication",
      "username":"<USERNAME>",
      "password":"<PASSWORD>"
    }
}
```

### <a name="response"></a><span data-ttu-id="e3d8c-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3d8c-151">Response</span></span>

<span data-ttu-id="e3d8c-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e3d8c-152">The following is an example of the response.</span></span>

<span data-ttu-id="e3d8c-153">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e3d8c-153">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityApiConnector"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/apiConnectors/$entity",
    "id":"guid",
    "displayName": "Test API",
    "targetUrl": "https://someapi.com/api",
    "authenticationConfiguration": {
        "@odata.type": "#microsoft.graph.basicAuthentication",
        "username": "<USERNAME>",
        "password": "******"
    }
}
```
