---
title: 'phoneAuthenticationMethod: disableSmsSignIn'
description: Desabilitar a login do SMS para um telefone celular
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: eb8933a141dcd343ab26a5d5809844ee79c39697
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516490"
---
# <a name="phoneauthenticationmethod-disablesmssignin"></a><span data-ttu-id="06c01-103">phoneAuthenticationMethod: disableSmsSignIn</span><span class="sxs-lookup"><span data-stu-id="06c01-103">phoneAuthenticationMethod: disableSmsSignIn</span></span>

<span data-ttu-id="06c01-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06c01-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06c01-105">Desabilite a login do SMS para um número `mobile` de telefone existente.</span><span class="sxs-lookup"><span data-stu-id="06c01-105">Disable SMS sign-in for an existing `mobile` phone number.</span></span> 

><span data-ttu-id="06c01-106">**Observação:** O número não estará mais disponível para a assinatura sms, o que pode impedir que o usuário entre.</span><span class="sxs-lookup"><span data-stu-id="06c01-106">**Note:** The number will no longer be available for SMS sign-in, which can prevent your user from signing in.</span></span>

## <a name="permissions"></a><span data-ttu-id="06c01-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="06c01-107">Permissions</span></span>

<span data-ttu-id="06c01-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06c01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="06c01-110">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="06c01-110">Permissions acting on self</span></span>

|<span data-ttu-id="06c01-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06c01-111">Permission type</span></span>      | <span data-ttu-id="06c01-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="06c01-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="06c01-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06c01-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="06c01-114">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06c01-114">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="06c01-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06c01-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06c01-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06c01-116">Not supported.</span></span> |
| <span data-ttu-id="06c01-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06c01-117">Application</span></span>                            | <span data-ttu-id="06c01-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06c01-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="06c01-119">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="06c01-119">Permissions acting on other users</span></span>

|<span data-ttu-id="06c01-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06c01-120">Permission type</span></span>      | <span data-ttu-id="06c01-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="06c01-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="06c01-122">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06c01-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="06c01-123">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06c01-123">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="06c01-124">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06c01-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06c01-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06c01-125">Not supported.</span></span> |
| <span data-ttu-id="06c01-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06c01-126">Application</span></span>                            | <span data-ttu-id="06c01-127">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06c01-127">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="06c01-128">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="06c01-128">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="06c01-129">Administrador global</span><span class="sxs-lookup"><span data-stu-id="06c01-129">Global admin</span></span>
* <span data-ttu-id="06c01-130">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="06c01-130">Privileged authentication admin</span></span>
* <span data-ttu-id="06c01-131">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="06c01-131">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="06c01-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06c01-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods/{id}/disableSmsSignIn
POST /users/{id | userPrincipalName}/authentication/phoneMethods/{id}/disableSmsSignIn
```

## <a name="request-headers"></a><span data-ttu-id="06c01-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06c01-133">Request headers</span></span>

| <span data-ttu-id="06c01-134">Nome</span><span class="sxs-lookup"><span data-stu-id="06c01-134">Name</span></span>          | <span data-ttu-id="06c01-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="06c01-135">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="06c01-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="06c01-136">Authorization</span></span> | <span data-ttu-id="06c01-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06c01-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06c01-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06c01-139">Request body</span></span>

<span data-ttu-id="06c01-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="06c01-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06c01-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="06c01-141">Response</span></span>

<span data-ttu-id="06c01-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06c01-p103">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="06c01-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="06c01-144">Examples</span></span>

<span data-ttu-id="06c01-145">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="06c01-145">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="06c01-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06c01-146">Request</span></span>

<span data-ttu-id="06c01-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="06c01-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="06c01-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="06c01-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "phoneauthenticationmethod_disablesmssignin"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7/disableSmsSignIn
```
# <a name="c"></a>[<span data-ttu-id="06c01-149">C#</span><span class="sxs-lookup"><span data-stu-id="06c01-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/phoneauthenticationmethod-disablesmssignin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="06c01-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06c01-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/phoneauthenticationmethod-disablesmssignin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="06c01-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06c01-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/phoneauthenticationmethod-disablesmssignin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="06c01-152">Java</span><span class="sxs-lookup"><span data-stu-id="06c01-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/phoneauthenticationmethod-disablesmssignin-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="06c01-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="06c01-153">Response</span></span>

<span data-ttu-id="06c01-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="06c01-154">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phoneAuthenticationMethod: disableSmsSignIn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
