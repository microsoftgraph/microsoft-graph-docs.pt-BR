---
title: Obter passwordlessMicrosoftAuthenticatorAuthenticationMethod
description: Leia as propriedades e as relações de um objetoMicrosoftAuthenticatorAuthenticationMethod sem senha.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5089bc5920cd01fff5f159c919142223640a0b32
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516714"
---
# <a name="get-passwordlessmicrosoftauthenticatorauthenticationmethod-deprecated"></a><span data-ttu-id="4e7f3-103">Obter passwordlessMicrosoftAuthenticatorAuthenticationMethod (preterido)</span><span class="sxs-lookup"><span data-stu-id="4e7f3-103">Get passwordlessMicrosoftAuthenticatorAuthenticationMethod (deprecated)</span></span>
<span data-ttu-id="4e7f3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e7f3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e7f3-105">Recupere o único objeto de método de Login de Telefone Sem Senha do [Microsoft Authenticator de um](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) usuário.</span><span class="sxs-lookup"><span data-stu-id="4e7f3-105">Retrieve a user's single [Microsoft Authenticator Passwordless Phone Sign-in method](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) object.</span></span>

> [!CAUTION]
> <span data-ttu-id="4e7f3-106">A API do método de login sem senha do Microsoft Authenticator Phone está preterida e interromperá o retorno dos resultados em 31 de dezembro de 2020.</span><span class="sxs-lookup"><span data-stu-id="4e7f3-106">The Microsoft Authenticator Passwordless Phone Sign-in method API is deprecated and will stop returning results on December 31, 2020.</span></span> <span data-ttu-id="4e7f3-107">Use o novo [Método de Autenticação do Autenticador microsoft](../resources/microsoftAuthenticatorAuthenticationMethod.md).</span><span class="sxs-lookup"><span data-stu-id="4e7f3-107">Please use the new [Microsoft Authenticator Authentication Method](../resources/microsoftAuthenticatorAuthenticationMethod.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4e7f3-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="4e7f3-108">Permissions</span></span>

<span data-ttu-id="4e7f3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e7f3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="4e7f3-111">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="4e7f3-111">Permissions acting on self</span></span>

|<span data-ttu-id="4e7f3-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e7f3-112">Permission type</span></span>      | <span data-ttu-id="4e7f3-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4e7f3-113">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="4e7f3-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e7f3-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="4e7f3-115">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e7f3-115">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="4e7f3-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e7f3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e7f3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e7f3-117">Not supported.</span></span> |
| <span data-ttu-id="4e7f3-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4e7f3-118">Application</span></span>                            | <span data-ttu-id="4e7f3-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e7f3-119">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="4e7f3-120">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="4e7f3-120">Permissions acting on other users</span></span>

|<span data-ttu-id="4e7f3-121">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e7f3-121">Permission type</span></span>      | <span data-ttu-id="4e7f3-122">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4e7f3-122">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="4e7f3-123">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e7f3-123">Delegated (work or school account)</span></span>     | <span data-ttu-id="4e7f3-124">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e7f3-124">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="4e7f3-125">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e7f3-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e7f3-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e7f3-126">Not supported.</span></span> |
| <span data-ttu-id="4e7f3-127">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4e7f3-127">Application</span></span>                            | <span data-ttu-id="4e7f3-128">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e7f3-128">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="4e7f3-129">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="4e7f3-129">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="4e7f3-130">Administrador global</span><span class="sxs-lookup"><span data-stu-id="4e7f3-130">Global admin</span></span>
* <span data-ttu-id="4e7f3-131">Leitor global</span><span class="sxs-lookup"><span data-stu-id="4e7f3-131">Global reader</span></span>
* <span data-ttu-id="4e7f3-132">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="4e7f3-132">Privileged authentication admin</span></span>
* <span data-ttu-id="4e7f3-133">Administrador de autenticação (apenas vê números de telefone mascarados)</span><span class="sxs-lookup"><span data-stu-id="4e7f3-133">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="4e7f3-134">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e7f3-134">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
GET /users/{id | userPrincipalName}/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4e7f3-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4e7f3-135">Request headers</span></span>
|<span data-ttu-id="4e7f3-136">Nome</span><span class="sxs-lookup"><span data-stu-id="4e7f3-136">Name</span></span>|<span data-ttu-id="4e7f3-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e7f3-137">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4e7f3-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="4e7f3-138">Authorization</span></span>|<span data-ttu-id="4e7f3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4e7f3-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e7f3-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e7f3-141">Request body</span></span>
<span data-ttu-id="4e7f3-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4e7f3-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e7f3-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e7f3-143">Response</span></span>

<span data-ttu-id="4e7f3-144">Se tiver êxito, este método retornará um código de resposta e o objeto `200 OK` [PasswordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4e7f3-144">If successful, this method returns a `200 OK` response code and the requested [passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4e7f3-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4e7f3-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4e7f3-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e7f3-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4e7f3-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e7f3-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordlessmicrosoftauthenticatorauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/passwordlessMicrosoftAuthenticatorMethods/R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1
```
# <a name="c"></a>[<span data-ttu-id="4e7f3-148">C#</span><span class="sxs-lookup"><span data-stu-id="4e7f3-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordlessmicrosoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e7f3-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e7f3-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordlessmicrosoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e7f3-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e7f3-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordlessmicrosoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4e7f3-151">Java</span><span class="sxs-lookup"><span data-stu-id="4e7f3-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-passwordlessmicrosoftauthenticatorauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="4e7f3-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e7f3-152">Response</span></span>
<span data-ttu-id="4e7f3-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4e7f3-153">The following is an example of the response.</span></span>

<span data-ttu-id="4e7f3-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4e7f3-154">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": {
      "id": "R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1",
      "displayName": "My mobile phone",
      "creationDateTime": "2020-09-02T04:16:49Z"
  }
}
```

