---
title: Listar passwordlessMicrosoftAuthenticatorAuthenticationMethods
description: Recupere uma lista dos objetosMicrosoftAuthenticatorAuthenticationMethod e suas propriedades.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 18a0e9e6961e97f2b6d9c709eff61676242417ab
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447770"
---
# <a name="list-passwordlessmicrosoftauthenticatorauthenticationmethods-deprecated"></a><span data-ttu-id="1c811-103">Listar passwordlessMicrosoftAuthenticatorAuthenticationMethods (preterido)</span><span class="sxs-lookup"><span data-stu-id="1c811-103">List passwordlessMicrosoftAuthenticatorAuthenticationMethods (deprecated)</span></span>
<span data-ttu-id="1c811-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c811-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c811-105">Recupere uma lista dos objetos do método de Login de Telefone sem Senha do [Microsoft Authenticator e](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="1c811-105">Retrieve a list of a user's [Microsoft Authenticator Passwordless Phone Sign-in method](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) objects and their properties.</span></span>

> [!CAUTION]
> <span data-ttu-id="1c811-106">A API do método de login sem senha do Microsoft Authenticator Phone está preterida e interromperá o retorno dos resultados em 31 de dezembro de 2020.</span><span class="sxs-lookup"><span data-stu-id="1c811-106">The Microsoft Authenticator Passwordless Phone Sign-in method API is deprecated and will stop returning results on December 31, 2020.</span></span> <span data-ttu-id="1c811-107">Use o novo [Método de Autenticação do Autenticador microsoft](../resources/microsoftAuthenticatorAuthenticationMethod.md).</span><span class="sxs-lookup"><span data-stu-id="1c811-107">Please use the new [Microsoft Authenticator Authentication Method](../resources/microsoftAuthenticatorAuthenticationMethod.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1c811-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="1c811-108">Permissions</span></span>

<span data-ttu-id="1c811-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c811-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="1c811-111">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="1c811-111">Permissions acting on self</span></span>

|<span data-ttu-id="1c811-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c811-112">Permission type</span></span>      | <span data-ttu-id="1c811-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1c811-113">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="1c811-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c811-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="1c811-115">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c811-115">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="1c811-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c811-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c811-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c811-117">Not supported.</span></span> |
| <span data-ttu-id="1c811-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c811-118">Application</span></span>                            | <span data-ttu-id="1c811-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c811-119">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="1c811-120">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="1c811-120">Permissions acting on other users</span></span>

|<span data-ttu-id="1c811-121">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c811-121">Permission type</span></span>      | <span data-ttu-id="1c811-122">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1c811-122">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="1c811-123">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c811-123">Delegated (work or school account)</span></span>     | <span data-ttu-id="1c811-124">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c811-124">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="1c811-125">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c811-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c811-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c811-126">Not supported.</span></span> |
| <span data-ttu-id="1c811-127">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c811-127">Application</span></span>                            | <span data-ttu-id="1c811-128">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c811-128">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="1c811-129">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="1c811-129">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="1c811-130">Administrador global</span><span class="sxs-lookup"><span data-stu-id="1c811-130">Global admin</span></span>
* <span data-ttu-id="1c811-131">Leitor global</span><span class="sxs-lookup"><span data-stu-id="1c811-131">Global reader</span></span>
* <span data-ttu-id="1c811-132">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="1c811-132">Privileged authentication admin</span></span>
* <span data-ttu-id="1c811-133">Administrador de autenticação (apenas vê números de telefone mascarados)</span><span class="sxs-lookup"><span data-stu-id="1c811-133">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="1c811-134">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c811-134">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/passwordlessMicrosoftAuthenticatorMethods
GET /users/{id | userPrincipalName}/authentication/passwordlessMicrosoftAuthenticatorMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1c811-135">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1c811-135">Optional query parameters</span></span>
<span data-ttu-id="1c811-136">Este método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1c811-136">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c811-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c811-137">Request headers</span></span>
|<span data-ttu-id="1c811-138">Nome</span><span class="sxs-lookup"><span data-stu-id="1c811-138">Name</span></span>|<span data-ttu-id="1c811-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c811-139">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1c811-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c811-140">Authorization</span></span>|<span data-ttu-id="1c811-141">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="1c811-141">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c811-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c811-142">Request body</span></span>
<span data-ttu-id="1c811-143">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1c811-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c811-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c811-144">Response</span></span>

<span data-ttu-id="1c811-145">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetosMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c811-145">If successful, this method returns a `200 OK` response code and a collection of [passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1c811-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1c811-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1c811-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c811-147">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1c811-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c811-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordlessmicrosoftauthenticatorauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/passwordlessMicrosoftAuthenticatorMethods
```
# <a name="c"></a>[<span data-ttu-id="1c811-149">C#</span><span class="sxs-lookup"><span data-stu-id="1c811-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordlessmicrosoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c811-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c811-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordlessmicrosoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c811-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c811-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordlessmicrosoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c811-152">Java</span><span class="sxs-lookup"><span data-stu-id="1c811-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-passwordlessmicrosoftauthenticatorauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="1c811-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c811-153">Response</span></span>
<span data-ttu-id="1c811-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1c811-154">The following is an example of the response.</span></span>

<span data-ttu-id="1c811-155">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1c811-155">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": [
    {
      "id": "R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1",
      "displayName": "My mobile phone",
      "creationDateTime": "2020-09-02T04:16:49Z"
    },
    {
      "id": "J18B378Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJGM1",
      "displayName": "My tablet",
      "creationDateTime": "2020-09-02T03:36:19Z"
    }
  ]
}
```

