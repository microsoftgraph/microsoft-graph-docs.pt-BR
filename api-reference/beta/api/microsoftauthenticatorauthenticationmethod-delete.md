---
title: Excluir microsoftAuthenticatorAuthenticationMethod
description: Exclui um objeto microsoftAuthenticatorAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: adf34da25baa01812e1d5cf82112c03716c5cf32
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796722"
---
# <a name="delete-microsoftauthenticatorauthenticationmethod"></a><span data-ttu-id="74c86-103">Excluir microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="74c86-103">Delete microsoftAuthenticatorAuthenticationMethod</span></span>
<span data-ttu-id="74c86-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74c86-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="74c86-105">Exclui um [objeto microsoftAuthenticatorAuthenticationMethod.](../resources/microsoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="74c86-105">Deletes a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="74c86-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="74c86-106">Permissions</span></span>

<span data-ttu-id="74c86-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74c86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="74c86-109">Permissões agindo por si só</span><span class="sxs-lookup"><span data-stu-id="74c86-109">Permissions acting on self</span></span>

|<span data-ttu-id="74c86-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74c86-110">Permission type</span></span>      | <span data-ttu-id="74c86-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="74c86-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="74c86-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74c86-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="74c86-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74c86-113">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="74c86-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74c86-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74c86-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74c86-115">Not supported.</span></span> |
| <span data-ttu-id="74c86-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74c86-116">Application</span></span>                            | <span data-ttu-id="74c86-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74c86-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="74c86-118">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="74c86-118">Permissions acting on other users</span></span>

|<span data-ttu-id="74c86-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74c86-119">Permission type</span></span>      | <span data-ttu-id="74c86-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="74c86-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="74c86-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74c86-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="74c86-122">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74c86-122">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="74c86-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74c86-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74c86-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74c86-124">Not supported.</span></span> |
| <span data-ttu-id="74c86-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74c86-125">Application</span></span>                            | <span data-ttu-id="74c86-126">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74c86-126">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="74c86-127">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="74c86-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="74c86-128">Administração global</span><span class="sxs-lookup"><span data-stu-id="74c86-128">Global admin</span></span>
* <span data-ttu-id="74c86-129">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="74c86-129">Privileged authentication admin</span></span>
* <span data-ttu-id="74c86-130">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="74c86-130">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="74c86-131">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74c86-131">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /me/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
DELETE /user/{id | userPrincipalName}/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
```

## <a name="request-headers"></a><span data-ttu-id="74c86-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74c86-132">Request headers</span></span>
|<span data-ttu-id="74c86-133">Nome</span><span class="sxs-lookup"><span data-stu-id="74c86-133">Name</span></span>|<span data-ttu-id="74c86-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="74c86-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="74c86-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="74c86-135">Authorization</span></span>|<span data-ttu-id="74c86-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74c86-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="74c86-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74c86-138">Request body</span></span>
<span data-ttu-id="74c86-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="74c86-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74c86-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="74c86-140">Response</span></span>

<span data-ttu-id="74c86-141">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="74c86-141">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="74c86-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="74c86-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="74c86-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74c86-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_microsoftauthenticatorauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/user/kim@contoso.com/authentication/microsoftAuthenticatorMethods/_jpuR-TGZtk6aQCLF3BQjA2
```


### <a name="response"></a><span data-ttu-id="74c86-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="74c86-144">Response</span></span>
<span data-ttu-id="74c86-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="74c86-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

