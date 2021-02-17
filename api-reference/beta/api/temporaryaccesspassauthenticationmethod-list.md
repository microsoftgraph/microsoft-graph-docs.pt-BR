---
title: Listar temporaryAccessPassAuthenticationMethods
description: Obter uma lista dos objetos temporaryAccessPassAuthenticationMethod e suas propriedades.
author: inbarckMS
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6b44daae82d401da223d7012c662c9b3c9a97bec
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272615"
---
# <a name="list-temporaryaccesspassauthenticationmethods"></a><span data-ttu-id="200c4-103">Listar temporaryAccessPassAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="200c4-103">List temporaryAccessPassAuthenticationMethods</span></span>
<span data-ttu-id="200c4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="200c4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="200c4-105">Recupere uma lista de objetos [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)  de um usuário e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="200c4-105">Retrieve a list of a user's [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)  objects and their properties.</span></span> <span data-ttu-id="200c4-106">Essa chamada retornará apenas um único objeto, pois apenas um método de Passagem de Acesso Temporário pode ser definido para os usuários.</span><span class="sxs-lookup"><span data-stu-id="200c4-106">This call will only return a single object as only one Temporary Access Pass method can be set on users.</span></span>

## <a name="permissions"></a><span data-ttu-id="200c4-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="200c4-107">Permissions</span></span>
<span data-ttu-id="200c4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="200c4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="200c4-110">Permissões agindo por si só</span><span class="sxs-lookup"><span data-stu-id="200c4-110">Permissions acting on self</span></span>

|<span data-ttu-id="200c4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="200c4-111">Permission type</span></span>      | <span data-ttu-id="200c4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="200c4-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="200c4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="200c4-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="200c4-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="200c4-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="200c4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="200c4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="200c4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="200c4-116">Not supported.</span></span> |
| <span data-ttu-id="200c4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="200c4-117">Application</span></span>                            | <span data-ttu-id="200c4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="200c4-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="200c4-119">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="200c4-119">Permissions acting on other users</span></span>

|<span data-ttu-id="200c4-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="200c4-120">Permission type</span></span>      | <span data-ttu-id="200c4-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="200c4-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="200c4-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="200c4-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="200c4-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="200c4-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="200c4-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="200c4-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="200c4-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="200c4-125">Not supported.</span></span> |
| <span data-ttu-id="200c4-126">Application</span><span class="sxs-lookup"><span data-stu-id="200c4-126">Application</span></span>                            | <span data-ttu-id="200c4-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="200c4-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |


<span data-ttu-id="200c4-128">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa de uma das seguintes [funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="200c4-128">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="200c4-129">Administrador global</span><span class="sxs-lookup"><span data-stu-id="200c4-129">Global admin</span></span>
* <span data-ttu-id="200c4-130">Leitor global</span><span class="sxs-lookup"><span data-stu-id="200c4-130">Global reader</span></span>
* <span data-ttu-id="200c4-131">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="200c4-131">Privileged authentication admin</span></span>
* <span data-ttu-id="200c4-132">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="200c4-132">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="200c4-133">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="200c4-133">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/temporaryAccessPassMethods
GET /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="200c4-134">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="200c4-134">Optional query parameters</span></span>
<span data-ttu-id="200c4-135">Esse método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="200c4-135">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="200c4-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="200c4-136">Request headers</span></span>
|<span data-ttu-id="200c4-137">Nome</span><span class="sxs-lookup"><span data-stu-id="200c4-137">Name</span></span>|<span data-ttu-id="200c4-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="200c4-138">Description</span></span>|
|:---|:---|
|<span data-ttu-id="200c4-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="200c4-139">Authorization</span></span>|<span data-ttu-id="200c4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="200c4-p103">Bearer {token}. Required.</span></span>|

## <a name="request"></a><span data-ttu-id="200c4-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="200c4-142">Request</span></span> 
<span data-ttu-id="200c4-143">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="200c4-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="200c4-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="200c4-144">Response</span></span>

<span data-ttu-id="200c4-145">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="200c4-145">If successful, this method returns a `200 OK` response code and a collection of [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) objects in the response body.</span></span>  <span data-ttu-id="200c4-146">Essa chamada retornará apenas um único objeto porque apenas um **temporaryAccessPassAuthenticationMethod** pode ser definido nos usuários.</span><span class="sxs-lookup"><span data-stu-id="200c4-146">This call will only return a single object because only one **temporaryAccessPassAuthenticationMethod** can be set on users.</span></span>

## <a name="examples"></a><span data-ttu-id="200c4-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="200c4-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="200c4-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="200c4-148">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_temporaryaccesspassauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/temporaryAccessPassMethods
```


### <a name="response"></a><span data-ttu-id="200c4-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="200c4-149">Response</span></span>
<span data-ttu-id="200c4-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="200c4-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.temporaryAccessPassAuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
      "id": "String",
      "temporaryAccessPass": "String",
      "createdDateTime": "String (timestamp)",
      "startDateTime": "String (timestamp)",
      "lifetimeInMinutes": "Integer",
      "isUsableOnce": "Boolean",
      "isUsable": "Boolean",
      "methodUsabilityReason": "String"
    }
  ]
}
```
