---
title: Excluir windowsHelloForBusinessAuthenticationMethod
description: Exclui um objeto windowsHelloForBusinessAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: de3e491a5eef3f09b89134fdc45dbb9805b82627
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51467943"
---
# <a name="delete-windowshelloforbusinessauthenticationmethod"></a><span data-ttu-id="3702f-103">Excluir windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3702f-103">Delete windowsHelloForBusinessAuthenticationMethod</span></span>
<span data-ttu-id="3702f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3702f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3702f-105">Exclui um [objeto windowsHelloForBusinessAuthenticationMethod.](../resources/windowshelloforbusinessauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="3702f-105">Deletes a [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3702f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3702f-106">Permissions</span></span>

<span data-ttu-id="3702f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3702f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="3702f-109">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="3702f-109">Permissions acting on self</span></span>

|<span data-ttu-id="3702f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3702f-110">Permission type</span></span>      | <span data-ttu-id="3702f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3702f-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="3702f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3702f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3702f-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3702f-113">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="3702f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3702f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3702f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3702f-115">Not supported.</span></span> |
| <span data-ttu-id="3702f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3702f-116">Application</span></span>                            | <span data-ttu-id="3702f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3702f-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="3702f-118">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="3702f-118">Permissions acting on other users</span></span>

|<span data-ttu-id="3702f-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3702f-119">Permission type</span></span>      | <span data-ttu-id="3702f-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3702f-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="3702f-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3702f-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="3702f-122">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3702f-122">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="3702f-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3702f-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3702f-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3702f-124">Not supported.</span></span> |
| <span data-ttu-id="3702f-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3702f-125">Application</span></span>                            | <span data-ttu-id="3702f-126">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3702f-126">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="3702f-127">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="3702f-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="3702f-128">Administrador global</span><span class="sxs-lookup"><span data-stu-id="3702f-128">Global admin</span></span>
* <span data-ttu-id="3702f-129">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="3702f-129">Privileged authentication admin</span></span>
* <span data-ttu-id="3702f-130">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="3702f-130">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="3702f-131">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3702f-131">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/authentication/windowsHelloForBusinessMethods/{windowsHelloForBusinessAuthenticationMethodId}
DELETE /users/{id | userPrincipalName}/authentication/windowsHelloForBusinessMethods/{windowsHelloForBusinessAuthenticationMethodId}
```

## <a name="request-headers"></a><span data-ttu-id="3702f-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3702f-132">Request headers</span></span>
|<span data-ttu-id="3702f-133">Nome</span><span class="sxs-lookup"><span data-stu-id="3702f-133">Name</span></span>|<span data-ttu-id="3702f-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="3702f-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3702f-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="3702f-135">Authorization</span></span>|<span data-ttu-id="3702f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3702f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3702f-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3702f-138">Request body</span></span>
<span data-ttu-id="3702f-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3702f-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3702f-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3702f-140">Response</span></span>

<span data-ttu-id="3702f-141">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3702f-141">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="3702f-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3702f-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3702f-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3702f-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3702f-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="3702f-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_windowshelloforbusinessauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/users/kim@contoso.com/authentication/windowsHelloForBusinessMethods/_jpuR-TGZtk6aQCLF3BQjA2
```
# <a name="c"></a>[<span data-ttu-id="3702f-145">C#</span><span class="sxs-lookup"><span data-stu-id="3702f-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-windowshelloforbusinessauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3702f-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3702f-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-windowshelloforbusinessauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3702f-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3702f-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-windowshelloforbusinessauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3702f-148">Java</span><span class="sxs-lookup"><span data-stu-id="3702f-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-windowshelloforbusinessauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="3702f-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="3702f-149">Response</span></span>
<span data-ttu-id="3702f-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3702f-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

