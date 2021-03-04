---
title: Listar microsoftAuthenticatorAuthenticationMethods
description: Obter uma lista dos objetos microsoftAuthenticatorAuthenticationMethod e suas propriedades.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c1fb487b482d2fe5fbf8b80f85c9b296bce52cc9
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447944"
---
# <a name="list-microsoftauthenticatorauthenticationmethods"></a><span data-ttu-id="e5eb2-103">Listar microsoftAuthenticatorAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="e5eb2-103">List microsoftAuthenticatorAuthenticationMethods</span></span>
<span data-ttu-id="e5eb2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5eb2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e5eb2-105">Obter uma lista dos [objetos microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="e5eb2-105">Get a list of the [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5eb2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e5eb2-106">Permissions</span></span>

<span data-ttu-id="e5eb2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5eb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="e5eb2-109">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="e5eb2-109">Permissions acting on self</span></span>

|<span data-ttu-id="e5eb2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5eb2-110">Permission type</span></span>      | <span data-ttu-id="e5eb2-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5eb2-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="e5eb2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5eb2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e5eb2-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5eb2-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="e5eb2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5eb2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5eb2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5eb2-115">Not supported.</span></span> |
| <span data-ttu-id="e5eb2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5eb2-116">Application</span></span>                            | <span data-ttu-id="e5eb2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5eb2-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="e5eb2-118">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="e5eb2-118">Permissions acting on other users</span></span>

|<span data-ttu-id="e5eb2-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5eb2-119">Permission type</span></span>      | <span data-ttu-id="e5eb2-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5eb2-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="e5eb2-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5eb2-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="e5eb2-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5eb2-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="e5eb2-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5eb2-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5eb2-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5eb2-124">Not supported.</span></span> |
| <span data-ttu-id="e5eb2-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5eb2-125">Application</span></span>                            | <span data-ttu-id="e5eb2-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5eb2-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="e5eb2-127">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="e5eb2-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="e5eb2-128">Administrador global</span><span class="sxs-lookup"><span data-stu-id="e5eb2-128">Global admin</span></span>
* <span data-ttu-id="e5eb2-129">Leitor global</span><span class="sxs-lookup"><span data-stu-id="e5eb2-129">Global reader</span></span>
* <span data-ttu-id="e5eb2-130">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="e5eb2-130">Privileged authentication admin</span></span>
* <span data-ttu-id="e5eb2-131">Administrador de autenticação (apenas vê números de telefone mascarados)</span><span class="sxs-lookup"><span data-stu-id="e5eb2-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="e5eb2-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5eb2-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/microsoftAuthenticatorMethods
GET /users/{id | userPrincipalName}/authentication/microsoftAuthenticatorMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e5eb2-133">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e5eb2-133">Optional query parameters</span></span>

<span data-ttu-id="e5eb2-134">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5eb2-134">Not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e5eb2-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5eb2-135">Request headers</span></span>

|<span data-ttu-id="e5eb2-136">Nome</span><span class="sxs-lookup"><span data-stu-id="e5eb2-136">Name</span></span>|<span data-ttu-id="e5eb2-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5eb2-137">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e5eb2-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5eb2-138">Authorization</span></span>|<span data-ttu-id="e5eb2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5eb2-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5eb2-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5eb2-141">Request body</span></span>

<span data-ttu-id="e5eb2-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e5eb2-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5eb2-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5eb2-143">Response</span></span>

<span data-ttu-id="e5eb2-144">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5eb2-144">If successful, this method returns a `200 OK` response code and a collection of [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e5eb2-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e5eb2-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e5eb2-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5eb2-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e5eb2-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5eb2-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_microsoftauthenticatorauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/anirban@contoso.com/authentication/microsoftAuthenticatorMethods
```
# <a name="c"></a>[<span data-ttu-id="e5eb2-148">C#</span><span class="sxs-lookup"><span data-stu-id="e5eb2-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-microsoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5eb2-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5eb2-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-microsoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5eb2-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5eb2-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-microsoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5eb2-151">Java</span><span class="sxs-lookup"><span data-stu-id="e5eb2-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-microsoftauthenticatorauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e5eb2-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5eb2-152">Response</span></span>
<span data-ttu-id="e5eb2-153">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e5eb2-153">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.microsoftAuthenticatorAuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethod",
      "id": "6803c096-c096-6803-96c0-036896c00368",
      "displayName": "Sandeep's iPhone",
      "deviceTag": "",
      "phoneAppVersion": "6.5.4",
      "createdDateTime": "2020-12-03T23:16:12Z"
    }
  ]
}
```

