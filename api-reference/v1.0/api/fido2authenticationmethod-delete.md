---
title: Excluir fido2AuthenticationMethod
description: Exclui um objeto fido2AuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 26dc814b92a987d8868cf89d7802a601ef165dd9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964591"
---
# <a name="delete-fido2authenticationmethod"></a><span data-ttu-id="28ab4-103">Excluir fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="28ab4-103">Delete fido2AuthenticationMethod</span></span>
<span data-ttu-id="28ab4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28ab4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="28ab4-105">Exclui o objeto do método de autenticação de chave de segurança [FIDO2 de um](../resources/fido2authenticationmethod.md) usuário.</span><span class="sxs-lookup"><span data-stu-id="28ab4-105">Deletes a user's [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="28ab4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="28ab4-106">Permissions</span></span>

<span data-ttu-id="28ab4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28ab4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="28ab4-109">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="28ab4-109">Permissions acting on self</span></span>

|<span data-ttu-id="28ab4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28ab4-110">Permission type</span></span>      | <span data-ttu-id="28ab4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28ab4-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="28ab4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28ab4-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="28ab4-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28ab4-113">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="28ab4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28ab4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28ab4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28ab4-115">Not supported.</span></span> |
| <span data-ttu-id="28ab4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28ab4-116">Application</span></span>                            | <span data-ttu-id="28ab4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28ab4-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="28ab4-118">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="28ab4-118">Permissions acting on other users</span></span>

|<span data-ttu-id="28ab4-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28ab4-119">Permission type</span></span>      | <span data-ttu-id="28ab4-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28ab4-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="28ab4-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28ab4-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="28ab4-122">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28ab4-122">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="28ab4-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28ab4-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28ab4-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28ab4-124">Not supported.</span></span> |
| <span data-ttu-id="28ab4-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28ab4-125">Application</span></span>                            | <span data-ttu-id="28ab4-126">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28ab4-126">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="28ab4-127">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="28ab4-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="28ab4-128">Administrador global</span><span class="sxs-lookup"><span data-stu-id="28ab4-128">Global admin</span></span>
* <span data-ttu-id="28ab4-129">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="28ab4-129">Privileged authentication admin</span></span>
* <span data-ttu-id="28ab4-130">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="28ab4-130">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="28ab4-131">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28ab4-131">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/fido2Methods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="28ab4-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28ab4-132">Request headers</span></span>
|<span data-ttu-id="28ab4-133">Nome</span><span class="sxs-lookup"><span data-stu-id="28ab4-133">Name</span></span>|<span data-ttu-id="28ab4-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="28ab4-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="28ab4-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="28ab4-135">Authorization</span></span>|<span data-ttu-id="28ab4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28ab4-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="28ab4-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28ab4-138">Request body</span></span>
<span data-ttu-id="28ab4-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="28ab4-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28ab4-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="28ab4-140">Response</span></span>

<span data-ttu-id="28ab4-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28ab4-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="28ab4-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="28ab4-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="28ab4-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28ab4-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="28ab4-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="28ab4-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/users/kim@contoso.com/authentication/fido2Methods/_jpuR-TGZtk6aQCLF3BQjA2
```

### <a name="response"></a><span data-ttu-id="28ab4-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="28ab4-146">Response</span></span>
<span data-ttu-id="28ab4-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="28ab4-147">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

