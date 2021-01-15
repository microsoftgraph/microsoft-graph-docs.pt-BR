---
title: Excluir emailAuthenticationMethod
description: Exclui um objeto emailAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7fbb2f6af414da2c44ca6d68dc688973e9d34bce
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873497"
---
# <a name="delete-emailauthenticationmethod"></a><span data-ttu-id="7ddeb-103">Excluir emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7ddeb-103">Delete emailAuthenticationMethod</span></span>
<span data-ttu-id="7ddeb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ddeb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ddeb-105">Exclui um objeto do método de autenticação [de email de um](../resources/emailauthenticationmethod.md) usuário.</span><span class="sxs-lookup"><span data-stu-id="7ddeb-105">Deletes a user's [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ddeb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7ddeb-106">Permissions</span></span>
<span data-ttu-id="7ddeb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ddeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ddeb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ddeb-109">Permission type</span></span>|<span data-ttu-id="7ddeb-110">Permissões atuando por si mesmo (do menos para o mais privilegiado)</span><span class="sxs-lookup"><span data-stu-id="7ddeb-110">Permissions acting on self (from least to most privileged)</span></span>|<span data-ttu-id="7ddeb-111">Permissões atuando em outras pessoas (de menos para mais privilegiados)</span><span class="sxs-lookup"><span data-stu-id="7ddeb-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="7ddeb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ddeb-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="7ddeb-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7ddeb-113">UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="7ddeb-114">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ddeb-114">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="7ddeb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ddeb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ddeb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ddeb-116">Not supported.</span></span> | <span data-ttu-id="7ddeb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ddeb-117">Not supported.</span></span> |
| <span data-ttu-id="7ddeb-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ddeb-118">Application</span></span>                            | <span data-ttu-id="7ddeb-119">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="7ddeb-119">Not applicable.</span></span> | <span data-ttu-id="7ddeb-120">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ddeb-120">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="7ddeb-121">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="7ddeb-121">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="7ddeb-122">Administrador global</span><span class="sxs-lookup"><span data-stu-id="7ddeb-122">Global admin</span></span>
* <span data-ttu-id="7ddeb-123">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="7ddeb-123">Privileged authentication admin</span></span>
* <span data-ttu-id="7ddeb-124">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="7ddeb-124">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="7ddeb-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ddeb-125">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7ddeb-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ddeb-126">Request headers</span></span>
|<span data-ttu-id="7ddeb-127">Nome</span><span class="sxs-lookup"><span data-stu-id="7ddeb-127">Name</span></span>|<span data-ttu-id="7ddeb-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ddeb-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7ddeb-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ddeb-129">Authorization</span></span>|<span data-ttu-id="7ddeb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ddeb-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ddeb-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ddeb-132">Request body</span></span>
<span data-ttu-id="7ddeb-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7ddeb-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ddeb-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ddeb-134">Response</span></span>

<span data-ttu-id="7ddeb-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ddeb-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7ddeb-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7ddeb-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7ddeb-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ddeb-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7ddeb-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ddeb-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_emailauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f
```
# <a name="c"></a>[<span data-ttu-id="7ddeb-140">C#</span><span class="sxs-lookup"><span data-stu-id="7ddeb-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-emailauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ddeb-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ddeb-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-emailauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ddeb-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ddeb-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-emailauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7ddeb-143">Java</span><span class="sxs-lookup"><span data-stu-id="7ddeb-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-emailauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="7ddeb-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ddeb-144">Response</span></span>
<span data-ttu-id="7ddeb-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7ddeb-145">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

