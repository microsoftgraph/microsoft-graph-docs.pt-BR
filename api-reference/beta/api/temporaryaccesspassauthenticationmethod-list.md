---
title: Listar temporaryAccessPassAuthenticationMethods
description: Obter uma lista dos objetos temporaryAccessPassAuthenticationMethod e suas propriedades.
author: inbarckMS
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a7a0b7af4cd5a7040f7cef3360ef153a5af7da60
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475804"
---
# <a name="list-temporaryaccesspassauthenticationmethods"></a><span data-ttu-id="b012c-103">Listar temporaryAccessPassAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="b012c-103">List temporaryAccessPassAuthenticationMethods</span></span>
<span data-ttu-id="b012c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b012c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b012c-105">Recupere uma lista dos objetos [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)  de um usuário e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="b012c-105">Retrieve a list of a user's [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)  objects and their properties.</span></span> <span data-ttu-id="b012c-106">Essa chamada retornará apenas um único objeto, pois apenas um método de Passagem de Acesso Temporário pode ser definido nos usuários.</span><span class="sxs-lookup"><span data-stu-id="b012c-106">This call will only return a single object as only one Temporary Access Pass method can be set on users.</span></span>

## <a name="permissions"></a><span data-ttu-id="b012c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b012c-107">Permissions</span></span>
<span data-ttu-id="b012c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b012c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="b012c-110">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="b012c-110">Permissions acting on self</span></span>

|<span data-ttu-id="b012c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b012c-111">Permission type</span></span>      | <span data-ttu-id="b012c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b012c-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="b012c-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b012c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b012c-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b012c-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="b012c-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b012c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b012c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b012c-116">Not supported.</span></span> |
| <span data-ttu-id="b012c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b012c-117">Application</span></span>                            | <span data-ttu-id="b012c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b012c-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="b012c-119">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="b012c-119">Permissions acting on other users</span></span>

|<span data-ttu-id="b012c-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b012c-120">Permission type</span></span>      | <span data-ttu-id="b012c-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b012c-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="b012c-122">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b012c-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="b012c-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b012c-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="b012c-124">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b012c-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b012c-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b012c-125">Not supported.</span></span> |
| <span data-ttu-id="b012c-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b012c-126">Application</span></span>                            | <span data-ttu-id="b012c-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b012c-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |


<span data-ttu-id="b012c-128">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma das seguintes [funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="b012c-128">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="b012c-129">Administrador global</span><span class="sxs-lookup"><span data-stu-id="b012c-129">Global admin</span></span>
* <span data-ttu-id="b012c-130">Leitor global</span><span class="sxs-lookup"><span data-stu-id="b012c-130">Global reader</span></span>
* <span data-ttu-id="b012c-131">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="b012c-131">Privileged authentication admin</span></span>
* <span data-ttu-id="b012c-132">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="b012c-132">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="b012c-133">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b012c-133">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/temporaryAccessPassMethods
GET /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b012c-134">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b012c-134">Optional query parameters</span></span>
<span data-ttu-id="b012c-135">Este método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b012c-135">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b012c-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b012c-136">Request headers</span></span>
|<span data-ttu-id="b012c-137">Nome</span><span class="sxs-lookup"><span data-stu-id="b012c-137">Name</span></span>|<span data-ttu-id="b012c-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="b012c-138">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b012c-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="b012c-139">Authorization</span></span>|<span data-ttu-id="b012c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b012c-p103">Bearer {token}. Required.</span></span>|

## <a name="request"></a><span data-ttu-id="b012c-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b012c-142">Request</span></span> 
<span data-ttu-id="b012c-143">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b012c-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b012c-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="b012c-144">Response</span></span>

<span data-ttu-id="b012c-145">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b012c-145">If successful, this method returns a `200 OK` response code and a collection of [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) objects in the response body.</span></span>  <span data-ttu-id="b012c-146">Essa chamada retornará apenas um único objeto porque apenas um **temporaryAccessPassAuthenticationMethod** pode ser definido nos usuários.</span><span class="sxs-lookup"><span data-stu-id="b012c-146">This call will only return a single object because only one **temporaryAccessPassAuthenticationMethod** can be set on users.</span></span>

## <a name="examples"></a><span data-ttu-id="b012c-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b012c-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b012c-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b012c-148">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b012c-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="b012c-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_temporaryaccesspassauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/temporaryAccessPassMethods
```
# <a name="c"></a>[<span data-ttu-id="b012c-150">C#</span><span class="sxs-lookup"><span data-stu-id="b012c-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-temporaryaccesspassauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b012c-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b012c-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-temporaryaccesspassauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b012c-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b012c-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-temporaryaccesspassauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b012c-153">Java</span><span class="sxs-lookup"><span data-stu-id="b012c-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-temporaryaccesspassauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b012c-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="b012c-154">Response</span></span>
<span data-ttu-id="b012c-155">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b012c-155">**Note:** The response object shown here might be shortened for readability.</span></span>
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
