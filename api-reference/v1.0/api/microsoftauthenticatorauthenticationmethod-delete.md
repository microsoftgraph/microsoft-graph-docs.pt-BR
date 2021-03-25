---
title: Excluir microsoftAuthenticatorAuthenticationMethod
description: Exclui um objeto microsoftAuthenticatorAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a2d454e428fd1fdfb9f86af573840eacea42aaec
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202825"
---
# <a name="delete-microsoftauthenticatorauthenticationmethod"></a><span data-ttu-id="46403-103">Excluir microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="46403-103">Delete microsoftAuthenticatorAuthenticationMethod</span></span>
<span data-ttu-id="46403-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46403-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="46403-105">Exclui um [objeto microsoftAuthenticatorAuthenticationMethod.](../resources/microsoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="46403-105">Deletes a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="46403-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="46403-106">Permissions</span></span>

<span data-ttu-id="46403-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46403-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="46403-109">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="46403-109">Permissions acting on self</span></span>

|<span data-ttu-id="46403-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46403-110">Permission type</span></span>      | <span data-ttu-id="46403-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46403-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="46403-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46403-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="46403-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="46403-113">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="46403-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46403-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46403-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46403-115">Not supported.</span></span> |
| <span data-ttu-id="46403-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46403-116">Application</span></span>                            | <span data-ttu-id="46403-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46403-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="46403-118">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="46403-118">Permissions acting on other users</span></span>

|<span data-ttu-id="46403-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46403-119">Permission type</span></span>      | <span data-ttu-id="46403-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46403-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="46403-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46403-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="46403-122">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46403-122">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="46403-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46403-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46403-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46403-124">Not supported.</span></span> |
| <span data-ttu-id="46403-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46403-125">Application</span></span>                            | <span data-ttu-id="46403-126">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46403-126">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="46403-127">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="46403-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="46403-128">Administrador global</span><span class="sxs-lookup"><span data-stu-id="46403-128">Global admin</span></span>
* <span data-ttu-id="46403-129">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="46403-129">Privileged authentication admin</span></span>
* <span data-ttu-id="46403-130">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="46403-130">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="46403-131">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46403-131">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
DELETE /users/{id | userPrincipalName}/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
```

## <a name="request-headers"></a><span data-ttu-id="46403-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46403-132">Request headers</span></span>
|<span data-ttu-id="46403-133">Nome</span><span class="sxs-lookup"><span data-stu-id="46403-133">Name</span></span>|<span data-ttu-id="46403-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="46403-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="46403-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="46403-135">Authorization</span></span>|<span data-ttu-id="46403-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46403-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="46403-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46403-138">Request body</span></span>
<span data-ttu-id="46403-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="46403-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46403-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="46403-140">Response</span></span>

<span data-ttu-id="46403-141">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="46403-141">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="46403-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="46403-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="46403-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46403-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="46403-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="46403-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_microsoftauthenticatorauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/users/kim@contoso.com/authentication/microsoftAuthenticatorMethods/_jpuR-TGZtk6aQCLF3BQjA2
```
# <a name="c"></a>[<span data-ttu-id="46403-145">C#</span><span class="sxs-lookup"><span data-stu-id="46403-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-microsoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="46403-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46403-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-microsoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="46403-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46403-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-microsoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="46403-148">Java</span><span class="sxs-lookup"><span data-stu-id="46403-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-microsoftauthenticatorauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="46403-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="46403-149">Response</span></span>
<span data-ttu-id="46403-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="46403-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

