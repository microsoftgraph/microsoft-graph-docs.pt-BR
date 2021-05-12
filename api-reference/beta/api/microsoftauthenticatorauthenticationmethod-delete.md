---
title: Excluir microsoftAuthenticatorAuthenticationMethod
description: Exclui um objeto microsoftAuthenticatorAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6d81e3a2ebf0cdbcea426d51cfcd1f3c9686cb1d
ms.sourcegitcommit: 2d8b04725ea4eaf304f3da1056a6451457a4630f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/12/2021
ms.locfileid: "52335678"
---
# <a name="delete-microsoftauthenticatorauthenticationmethod"></a><span data-ttu-id="31b81-103">Excluir microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="31b81-103">Delete microsoftAuthenticatorAuthenticationMethod</span></span>
<span data-ttu-id="31b81-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31b81-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31b81-105">Exclui um [objeto microsoftAuthenticatorAuthenticationMethod.](../resources/microsoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="31b81-105">Deletes a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="31b81-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="31b81-106">Permissions</span></span>

<span data-ttu-id="31b81-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31b81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="31b81-109">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="31b81-109">Permissions acting on self</span></span>

|<span data-ttu-id="31b81-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31b81-110">Permission type</span></span>      | <span data-ttu-id="31b81-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="31b81-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="31b81-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31b81-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="31b81-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="31b81-113">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="31b81-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31b81-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31b81-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31b81-115">Not supported.</span></span> |
| <span data-ttu-id="31b81-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31b81-116">Application</span></span>                            | <span data-ttu-id="31b81-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31b81-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="31b81-118">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="31b81-118">Permissions acting on other users</span></span>

|<span data-ttu-id="31b81-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31b81-119">Permission type</span></span>      | <span data-ttu-id="31b81-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="31b81-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="31b81-121">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31b81-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="31b81-122">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31b81-122">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="31b81-123">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31b81-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31b81-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31b81-124">Not supported.</span></span> |
| <span data-ttu-id="31b81-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31b81-125">Application</span></span>                            | <span data-ttu-id="31b81-126">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31b81-126">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="31b81-127">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="31b81-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="31b81-128">Administrador global</span><span class="sxs-lookup"><span data-stu-id="31b81-128">Global admin</span></span>
* <span data-ttu-id="31b81-129">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="31b81-129">Privileged authentication admin</span></span>
* <span data-ttu-id="31b81-130">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="31b81-130">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="31b81-131">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31b81-131">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
DELETE /users/{id | userPrincipalName}/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
```

## <a name="request-headers"></a><span data-ttu-id="31b81-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31b81-132">Request headers</span></span>
|<span data-ttu-id="31b81-133">Nome</span><span class="sxs-lookup"><span data-stu-id="31b81-133">Name</span></span>|<span data-ttu-id="31b81-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="31b81-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="31b81-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="31b81-135">Authorization</span></span>|<span data-ttu-id="31b81-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31b81-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="31b81-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31b81-138">Request body</span></span>
<span data-ttu-id="31b81-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="31b81-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31b81-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="31b81-140">Response</span></span>

<span data-ttu-id="31b81-141">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="31b81-141">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="31b81-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="31b81-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="31b81-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31b81-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="31b81-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="31b81-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_microsoftauthenticatorauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/microsoftAuthenticatorMethods/_jpuR-TGZtk6aQCLF3BQjA2
```
# <a name="c"></a>[<span data-ttu-id="31b81-145">C#</span><span class="sxs-lookup"><span data-stu-id="31b81-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-microsoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31b81-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31b81-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-microsoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31b81-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31b81-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-microsoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="31b81-148">Java</span><span class="sxs-lookup"><span data-stu-id="31b81-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-microsoftauthenticatorauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="31b81-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="31b81-149">Response</span></span>
<span data-ttu-id="31b81-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="31b81-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

