---
title: Excluir fido2AuthenticationMethod
description: Exclui um objeto fido2AuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 204b29ec29b44c785bce8388dff74866e6620996
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458490"
---
# <a name="delete-fido2authenticationmethod"></a><span data-ttu-id="c67e4-103">Excluir fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c67e4-103">Delete fido2AuthenticationMethod</span></span>
<span data-ttu-id="c67e4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c67e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c67e4-105">Exclui o objeto do [método de autenticação de chave de segurança FIDO2](../resources/fido2authenticationmethod.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="c67e4-105">Deletes a user's [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c67e4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c67e4-106">Permissions</span></span>
<span data-ttu-id="c67e4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c67e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c67e4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c67e4-109">Permission type</span></span>|<span data-ttu-id="c67e4-110">Permissões que atuam em si (de a mais de privilégios mínimos)</span><span class="sxs-lookup"><span data-stu-id="c67e4-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="c67e4-111">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c67e4-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="c67e4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c67e4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c67e4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c67e4-113">Not supported.</span></span>|<span data-ttu-id="c67e4-114">UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c67e4-114">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="c67e4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c67e4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c67e4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c67e4-116">Not supported.</span></span>|<span data-ttu-id="c67e4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c67e4-117">Not supported.</span></span>
|<span data-ttu-id="c67e4-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c67e4-118">Application</span></span>|<span data-ttu-id="c67e4-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c67e4-119">Not supported.</span></span>|<span data-ttu-id="c67e4-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c67e4-120">Not supported.</span></span>

<span data-ttu-id="c67e4-121">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa de uma das seguintes [funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="c67e4-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="c67e4-122">Administrador global</span><span class="sxs-lookup"><span data-stu-id="c67e4-122">Global admin</span></span>
* <span data-ttu-id="c67e4-123">Leitor global</span><span class="sxs-lookup"><span data-stu-id="c67e4-123">Global reader</span></span>
* <span data-ttu-id="c67e4-124">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="c67e4-124">Privileged authentication admin</span></span>
* <span data-ttu-id="c67e4-125">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="c67e4-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="c67e4-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c67e4-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/fido2Methods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c67e4-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c67e4-127">Request headers</span></span>
|<span data-ttu-id="c67e4-128">Nome</span><span class="sxs-lookup"><span data-stu-id="c67e4-128">Name</span></span>|<span data-ttu-id="c67e4-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="c67e4-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c67e4-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="c67e4-130">Authorization</span></span>|<span data-ttu-id="c67e4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c67e4-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c67e4-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c67e4-133">Request body</span></span>
<span data-ttu-id="c67e4-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c67e4-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c67e4-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c67e4-135">Response</span></span>

<span data-ttu-id="c67e4-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c67e4-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c67e4-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c67e4-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c67e4-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c67e4-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c67e4-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="c67e4-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/fido2Methods/_jpuR-TGZtk6aQCLF3BQjA2
```
# <a name="c"></a>[<span data-ttu-id="c67e4-141">C#</span><span class="sxs-lookup"><span data-stu-id="c67e4-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-fido2authenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c67e4-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c67e4-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-fido2authenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c67e4-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c67e4-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-fido2authenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c67e4-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="c67e4-144">Response</span></span>
<span data-ttu-id="c67e4-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c67e4-145">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

