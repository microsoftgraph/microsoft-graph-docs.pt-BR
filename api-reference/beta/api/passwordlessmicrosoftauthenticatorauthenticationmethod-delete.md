---
title: Excluir passwordlessMicrosoftAuthenticatorAuthenticationMethod
description: Exclui um objetoMicrosoftAuthenticatorAuthenticationMethod sem senha.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6e894cd8332969e708c8a7d8d1a53ca7c17be2dc
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796560"
---
# <a name="delete-passwordlessmicrosoftauthenticatorauthenticationmethod-deprecated"></a><span data-ttu-id="ae329-103">Excluir passwordlessMicrosoftAuthenticatorAuthenticationMethod (preterido)</span><span class="sxs-lookup"><span data-stu-id="ae329-103">Delete passwordlessMicrosoftAuthenticatorAuthenticationMethod (deprecated)</span></span>
<span data-ttu-id="ae329-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae329-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae329-105">Exclui o objeto do método de login de telefone sem senha do [Microsoft Authenticator de um](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) usuário.</span><span class="sxs-lookup"><span data-stu-id="ae329-105">Deletes a user's [Microsoft Authenticator Passwordless Phone Sign-in method](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) object.</span></span>

> [!CAUTION]
> <span data-ttu-id="ae329-106">A API do método de login de telefone sem senha do Microsoft Authenticator foi preterida e interromperá o retorno dos resultados em 31 de dezembro de 2020.</span><span class="sxs-lookup"><span data-stu-id="ae329-106">The Microsoft Authenticator Passwordless Phone Sign-in method API is deprecated and will stop returning results on December 31, 2020.</span></span> <span data-ttu-id="ae329-107">Use o novo Método [de Autenticação do Microsoft Authenticator.](../resources/microsoftAuthenticatorAuthenticationMethod.md)</span><span class="sxs-lookup"><span data-stu-id="ae329-107">Please use the new [Microsoft Authenticator Authentication Method](../resources/microsoftAuthenticatorAuthenticationMethod.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ae329-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="ae329-108">Permissions</span></span>

<span data-ttu-id="ae329-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae329-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="ae329-111">Permissões agindo por si só</span><span class="sxs-lookup"><span data-stu-id="ae329-111">Permissions acting on self</span></span>

|<span data-ttu-id="ae329-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae329-112">Permission type</span></span>      | <span data-ttu-id="ae329-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ae329-113">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="ae329-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae329-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="ae329-115">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ae329-115">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="ae329-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae329-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae329-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae329-117">Not supported.</span></span> |
| <span data-ttu-id="ae329-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae329-118">Application</span></span>                            | <span data-ttu-id="ae329-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae329-119">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="ae329-120">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="ae329-120">Permissions acting on other users</span></span>

|<span data-ttu-id="ae329-121">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae329-121">Permission type</span></span>      | <span data-ttu-id="ae329-122">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ae329-122">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="ae329-123">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae329-123">Delegated (work or school account)</span></span>     | <span data-ttu-id="ae329-124">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae329-124">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="ae329-125">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae329-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae329-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae329-126">Not supported.</span></span> |
| <span data-ttu-id="ae329-127">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae329-127">Application</span></span>                            | <span data-ttu-id="ae329-128">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae329-128">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="ae329-129">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="ae329-129">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="ae329-130">Administração global</span><span class="sxs-lookup"><span data-stu-id="ae329-130">Global admin</span></span>
* <span data-ttu-id="ae329-131">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="ae329-131">Privileged authentication admin</span></span>
* <span data-ttu-id="ae329-132">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="ae329-132">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="ae329-133">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae329-133">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ae329-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae329-134">Request headers</span></span>
|<span data-ttu-id="ae329-135">Nome</span><span class="sxs-lookup"><span data-stu-id="ae329-135">Name</span></span>|<span data-ttu-id="ae329-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae329-136">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ae329-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae329-137">Authorization</span></span>|<span data-ttu-id="ae329-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae329-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae329-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae329-140">Request body</span></span>
<span data-ttu-id="ae329-141">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ae329-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae329-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae329-142">Response</span></span>

<span data-ttu-id="ae329-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae329-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ae329-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ae329-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ae329-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae329-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ae329-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae329-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_passwordlessmicrosoftauthenticatorauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/passwordlessMicrosoftAuthenticatorMethods/R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1
```
# <a name="c"></a>[<span data-ttu-id="ae329-148">C#</span><span class="sxs-lookup"><span data-stu-id="ae329-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ae329-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae329-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ae329-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae329-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ae329-151">Java</span><span class="sxs-lookup"><span data-stu-id="ae329-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ae329-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae329-152">Response</span></span>
<span data-ttu-id="ae329-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ae329-153">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

