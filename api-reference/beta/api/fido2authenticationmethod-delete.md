---
title: Excluir fido2AuthenticationMethod
description: Exclui um objeto fido2AuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 3d92da843b6e18a07cf98e42dee685a1d692d6ef
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436075"
---
# <a name="delete-fido2authenticationmethod"></a><span data-ttu-id="d7037-103">Excluir fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d7037-103">Delete fido2AuthenticationMethod</span></span>
<span data-ttu-id="d7037-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7037-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7037-105">Exclui o objeto do método de autenticação de chave de segurança [FIDO2 de um](../resources/fido2authenticationmethod.md) usuário.</span><span class="sxs-lookup"><span data-stu-id="d7037-105">Deletes a user's [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7037-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d7037-106">Permissions</span></span>
<span data-ttu-id="d7037-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7037-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7037-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7037-109">Permission type</span></span>|<span data-ttu-id="d7037-110">Permissões agindo por si mesmo (do mínimo para o mais privilegiado)</span><span class="sxs-lookup"><span data-stu-id="d7037-110">Permissions acting on self (from least to most privileged)</span></span>|<span data-ttu-id="d7037-111">Permissões atuando em outras pessoas (do mínimo ao mais privilegiado)</span><span class="sxs-lookup"><span data-stu-id="d7037-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="d7037-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7037-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d7037-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7037-113">UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="d7037-114">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7037-114">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="d7037-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7037-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7037-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7037-116">Not supported.</span></span> | <span data-ttu-id="d7037-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7037-117">Not supported.</span></span> |
| <span data-ttu-id="d7037-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7037-118">Application</span></span>                            | <span data-ttu-id="d7037-119">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="d7037-119">Not applicable.</span></span> | <span data-ttu-id="d7037-120">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7037-120">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="d7037-121">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma das seguintes [funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="d7037-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="d7037-122">Administrador global</span><span class="sxs-lookup"><span data-stu-id="d7037-122">Global admin</span></span>
* <span data-ttu-id="d7037-123">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="d7037-123">Privileged authentication admin</span></span>
* <span data-ttu-id="d7037-124">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="d7037-124">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="d7037-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7037-125">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/fido2Methods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d7037-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7037-126">Request headers</span></span>
|<span data-ttu-id="d7037-127">Nome</span><span class="sxs-lookup"><span data-stu-id="d7037-127">Name</span></span>|<span data-ttu-id="d7037-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7037-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d7037-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="d7037-129">Authorization</span></span>|<span data-ttu-id="d7037-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d7037-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7037-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7037-132">Request body</span></span>
<span data-ttu-id="d7037-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d7037-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7037-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7037-134">Response</span></span>

<span data-ttu-id="d7037-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7037-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d7037-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d7037-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d7037-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7037-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d7037-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7037-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/fido2Methods/_jpuR-TGZtk6aQCLF3BQjA2
```
# <a name="c"></a>[<span data-ttu-id="d7037-140">C#</span><span class="sxs-lookup"><span data-stu-id="d7037-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-fido2authenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d7037-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7037-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-fido2authenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d7037-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7037-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-fido2authenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d7037-143">Java</span><span class="sxs-lookup"><span data-stu-id="d7037-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-fido2authenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d7037-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7037-144">Response</span></span>
<span data-ttu-id="d7037-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d7037-145">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

