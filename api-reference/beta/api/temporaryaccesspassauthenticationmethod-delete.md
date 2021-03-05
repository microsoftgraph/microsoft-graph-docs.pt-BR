---
title: Excluir temporaryAccessPassAuthenticationMethod
description: Exclui um objeto temporaryAccessPassAuthenticationMethod.
author: inbarckMS
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 31879dfc0d572f1914b15582ec515b0f8a44c85a
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475071"
---
# <a name="delete-temporaryaccesspassauthenticationmethod"></a><span data-ttu-id="5a38c-103">Excluir temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5a38c-103">Delete temporaryAccessPassAuthenticationMethod</span></span>
<span data-ttu-id="5a38c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a38c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a38c-105">[Exclua um objeto temporaryAccessPassAuthenticationMethod.](../resources/temporaryaccesspassauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="5a38c-105">Delete a [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object.</span></span>

<span data-ttu-id="5a38c-106">Embora o Passe de Acesso Temporário atual no usuário seja válido, ele precisa ser excluído antes que um novo Passe de Acesso Temporário possa ser criado no usuário.</span><span class="sxs-lookup"><span data-stu-id="5a38c-106">While the current Temporary Access Pass on the user is valid, it needs to be deleted before a new Temporary Access Pass can be created on the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a38c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5a38c-107">Permissions</span></span>
<span data-ttu-id="5a38c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a38c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="5a38c-110">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="5a38c-110">Permissions acting on self</span></span>

|<span data-ttu-id="5a38c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a38c-111">Permission type</span></span>      | <span data-ttu-id="5a38c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5a38c-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="5a38c-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a38c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="5a38c-114">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a38c-114">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="5a38c-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a38c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a38c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a38c-116">Not supported.</span></span> |
| <span data-ttu-id="5a38c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a38c-117">Application</span></span>                            | <span data-ttu-id="5a38c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a38c-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="5a38c-119">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="5a38c-119">Permissions acting on other users</span></span>

|<span data-ttu-id="5a38c-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a38c-120">Permission type</span></span>      | <span data-ttu-id="5a38c-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5a38c-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="5a38c-122">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a38c-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="5a38c-123">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a38c-123">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="5a38c-124">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a38c-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a38c-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a38c-125">Not supported.</span></span> |
| <span data-ttu-id="5a38c-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a38c-126">Application</span></span>                            | <span data-ttu-id="5a38c-127">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a38c-127">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="5a38c-128">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="5a38c-128">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="5a38c-129">Administrador global</span><span class="sxs-lookup"><span data-stu-id="5a38c-129">Global admin</span></span>
* <span data-ttu-id="5a38c-130">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="5a38c-130">Privileged authentication admin</span></span>
* <span data-ttu-id="5a38c-131">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="5a38c-131">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="5a38c-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a38c-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods/{id}
DELETE /me/authentication/temporaryAccessPassMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5a38c-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a38c-133">Request headers</span></span>
|<span data-ttu-id="5a38c-134">Nome</span><span class="sxs-lookup"><span data-stu-id="5a38c-134">Name</span></span>|<span data-ttu-id="5a38c-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a38c-135">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5a38c-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a38c-136">Authorization</span></span>|<span data-ttu-id="5a38c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a38c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a38c-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a38c-139">Request body</span></span>
<span data-ttu-id="5a38c-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5a38c-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a38c-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a38c-141">Response</span></span>

<span data-ttu-id="5a38c-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a38c-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5a38c-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5a38c-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5a38c-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a38c-145">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5a38c-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a38c-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_temporaryaccesspassauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/temporaryAccessPassMethods/{id}
```
# <a name="c"></a>[<span data-ttu-id="5a38c-147">C#</span><span class="sxs-lookup"><span data-stu-id="5a38c-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-temporaryaccesspassauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5a38c-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a38c-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-temporaryaccesspassauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a38c-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a38c-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-temporaryaccesspassauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5a38c-150">Java</span><span class="sxs-lookup"><span data-stu-id="5a38c-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-temporaryaccesspassauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="5a38c-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a38c-151">Response</span></span>
<span data-ttu-id="5a38c-152">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5a38c-152">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
