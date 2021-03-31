---
title: Excluir fido2AuthenticationMethod
description: Exclui um objeto fido2AuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 2ef78f3957f262b59bef7c627ea5450c2c759ab7
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469021"
---
# <a name="delete-fido2authenticationmethod"></a><span data-ttu-id="d2d5f-103">Excluir fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d2d5f-103">Delete fido2AuthenticationMethod</span></span>
<span data-ttu-id="d2d5f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2d5f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d2d5f-105">Exclui o objeto do método de autenticação de chave de segurança [FIDO2 de um](../resources/fido2authenticationmethod.md) usuário.</span><span class="sxs-lookup"><span data-stu-id="d2d5f-105">Deletes a user's [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2d5f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d2d5f-106">Permissions</span></span>

<span data-ttu-id="d2d5f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2d5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="d2d5f-109">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="d2d5f-109">Permissions acting on self</span></span>

|<span data-ttu-id="d2d5f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2d5f-110">Permission type</span></span>      | <span data-ttu-id="d2d5f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d2d5f-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="d2d5f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2d5f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d2d5f-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2d5f-113">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="d2d5f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2d5f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2d5f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2d5f-115">Not supported.</span></span> |
| <span data-ttu-id="d2d5f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2d5f-116">Application</span></span>                            | <span data-ttu-id="d2d5f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2d5f-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="d2d5f-118">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="d2d5f-118">Permissions acting on other users</span></span>

|<span data-ttu-id="d2d5f-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2d5f-119">Permission type</span></span>      | <span data-ttu-id="d2d5f-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d2d5f-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="d2d5f-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2d5f-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="d2d5f-122">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2d5f-122">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="d2d5f-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2d5f-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2d5f-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2d5f-124">Not supported.</span></span> |
| <span data-ttu-id="d2d5f-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2d5f-125">Application</span></span>                            | <span data-ttu-id="d2d5f-126">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2d5f-126">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="d2d5f-127">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="d2d5f-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="d2d5f-128">Administrador global</span><span class="sxs-lookup"><span data-stu-id="d2d5f-128">Global admin</span></span>
* <span data-ttu-id="d2d5f-129">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="d2d5f-129">Privileged authentication admin</span></span>
* <span data-ttu-id="d2d5f-130">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="d2d5f-130">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="d2d5f-131">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2d5f-131">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/fido2Methods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d2d5f-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2d5f-132">Request headers</span></span>
|<span data-ttu-id="d2d5f-133">Nome</span><span class="sxs-lookup"><span data-stu-id="d2d5f-133">Name</span></span>|<span data-ttu-id="d2d5f-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2d5f-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d2d5f-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2d5f-135">Authorization</span></span>|<span data-ttu-id="d2d5f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2d5f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2d5f-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2d5f-138">Request body</span></span>
<span data-ttu-id="d2d5f-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d2d5f-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2d5f-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2d5f-140">Response</span></span>

<span data-ttu-id="d2d5f-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2d5f-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d2d5f-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d2d5f-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d2d5f-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2d5f-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d2d5f-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2d5f-145">HTTP</span></span>](#tab/http)

# <a name="http"></a>[<span data-ttu-id="d2d5f-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2d5f-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/users/kim@contoso.com/authentication/fido2Methods/_jpuR-TGZtk6aQCLF3BQjA2
```
# <a name="c"></a>[<span data-ttu-id="d2d5f-147">C#</span><span class="sxs-lookup"><span data-stu-id="d2d5f-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-fido2authenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2d5f-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2d5f-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-fido2authenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2d5f-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2d5f-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-fido2authenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d2d5f-150">Java</span><span class="sxs-lookup"><span data-stu-id="d2d5f-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-fido2authenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d2d5f-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2d5f-151">Response</span></span>
<span data-ttu-id="d2d5f-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d2d5f-152">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

