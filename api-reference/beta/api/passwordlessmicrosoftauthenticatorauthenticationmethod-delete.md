---
title: Excluir passwordlessMicrosoftAuthenticatorAuthenticationMethod
description: Exclui um objetoMicrosoftAuthenticatorAuthenticationMethod sem senha.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5bd76dcb0652fdea395592ff916cd37eac789384
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515958"
---
# <a name="delete-passwordlessmicrosoftauthenticatorauthenticationmethod-deprecated"></a><span data-ttu-id="20665-103">Excluir passwordlessMicrosoftAuthenticatorAuthenticationMethod (preterido)</span><span class="sxs-lookup"><span data-stu-id="20665-103">Delete passwordlessMicrosoftAuthenticatorAuthenticationMethod (deprecated)</span></span>
<span data-ttu-id="20665-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20665-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20665-105">Exclui o objeto do método de Login de Telefone Sem Senha do [Microsoft Authenticator de um](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) usuário.</span><span class="sxs-lookup"><span data-stu-id="20665-105">Deletes a user's [Microsoft Authenticator Passwordless Phone Sign-in method](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) object.</span></span>

> [!CAUTION]
> <span data-ttu-id="20665-106">A API do método de login sem senha do Microsoft Authenticator Phone está preterida e interromperá o retorno dos resultados em 31 de dezembro de 2020.</span><span class="sxs-lookup"><span data-stu-id="20665-106">The Microsoft Authenticator Passwordless Phone Sign-in method API is deprecated and will stop returning results on December 31, 2020.</span></span> <span data-ttu-id="20665-107">Use o novo [Método de Autenticação do Autenticador microsoft](../resources/microsoftAuthenticatorAuthenticationMethod.md).</span><span class="sxs-lookup"><span data-stu-id="20665-107">Please use the new [Microsoft Authenticator Authentication Method](../resources/microsoftAuthenticatorAuthenticationMethod.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="20665-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="20665-108">Permissions</span></span>

<span data-ttu-id="20665-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20665-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="20665-111">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="20665-111">Permissions acting on self</span></span>

|<span data-ttu-id="20665-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20665-112">Permission type</span></span>      | <span data-ttu-id="20665-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20665-113">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="20665-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20665-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="20665-115">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20665-115">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="20665-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20665-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20665-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20665-117">Not supported.</span></span> |
| <span data-ttu-id="20665-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20665-118">Application</span></span>                            | <span data-ttu-id="20665-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20665-119">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="20665-120">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="20665-120">Permissions acting on other users</span></span>

|<span data-ttu-id="20665-121">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20665-121">Permission type</span></span>      | <span data-ttu-id="20665-122">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20665-122">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="20665-123">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20665-123">Delegated (work or school account)</span></span>     | <span data-ttu-id="20665-124">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20665-124">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="20665-125">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20665-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20665-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20665-126">Not supported.</span></span> |
| <span data-ttu-id="20665-127">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20665-127">Application</span></span>                            | <span data-ttu-id="20665-128">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20665-128">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="20665-129">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="20665-129">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="20665-130">Administrador global</span><span class="sxs-lookup"><span data-stu-id="20665-130">Global admin</span></span>
* <span data-ttu-id="20665-131">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="20665-131">Privileged authentication admin</span></span>
* <span data-ttu-id="20665-132">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="20665-132">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="20665-133">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20665-133">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="20665-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20665-134">Request headers</span></span>
|<span data-ttu-id="20665-135">Nome</span><span class="sxs-lookup"><span data-stu-id="20665-135">Name</span></span>|<span data-ttu-id="20665-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="20665-136">Description</span></span>|
|:---|:---|
|<span data-ttu-id="20665-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="20665-137">Authorization</span></span>|<span data-ttu-id="20665-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20665-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="20665-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20665-140">Request body</span></span>
<span data-ttu-id="20665-141">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="20665-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20665-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="20665-142">Response</span></span>

<span data-ttu-id="20665-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20665-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="20665-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="20665-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="20665-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20665-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="20665-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="20665-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_passwordlessmicrosoftauthenticatorauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/passwordlessMicrosoftAuthenticatorMethods/R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1
```
# <a name="c"></a>[<span data-ttu-id="20665-148">C#</span><span class="sxs-lookup"><span data-stu-id="20665-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20665-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20665-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20665-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20665-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="20665-151">Java</span><span class="sxs-lookup"><span data-stu-id="20665-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="20665-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="20665-152">Response</span></span>
<span data-ttu-id="20665-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="20665-153">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

