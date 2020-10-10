---
title: Excluir fido2AuthenticationMethod
description: Exclui um objeto fido2AuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: af396880c260a8e74dc67636015e68e49ce291de
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418167"
---
# <a name="delete-fido2authenticationmethod"></a><span data-ttu-id="80a0c-103">Excluir fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="80a0c-103">Delete fido2AuthenticationMethod</span></span>
<span data-ttu-id="80a0c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80a0c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80a0c-105">Exclui o objeto do [método de autenticação de chave de segurança FIDO2](../resources/fido2authenticationmethod.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="80a0c-105">Deletes a user's [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="80a0c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="80a0c-106">Permissions</span></span>
<span data-ttu-id="80a0c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80a0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80a0c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80a0c-109">Permission type</span></span>|<span data-ttu-id="80a0c-110">Permissões que atuam em si (de a mais de privilégios mínimos)</span><span class="sxs-lookup"><span data-stu-id="80a0c-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="80a0c-111">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="80a0c-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="80a0c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80a0c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="80a0c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80a0c-113">Not supported.</span></span>|<span data-ttu-id="80a0c-114">UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="80a0c-114">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="80a0c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80a0c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80a0c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80a0c-116">Not supported.</span></span>|<span data-ttu-id="80a0c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80a0c-117">Not supported.</span></span>
|<span data-ttu-id="80a0c-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80a0c-118">Application</span></span>|<span data-ttu-id="80a0c-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80a0c-119">Not supported.</span></span>|<span data-ttu-id="80a0c-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80a0c-120">Not supported.</span></span>

<span data-ttu-id="80a0c-121">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa de uma das seguintes [funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="80a0c-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="80a0c-122">Administrador global</span><span class="sxs-lookup"><span data-stu-id="80a0c-122">Global admin</span></span>
* <span data-ttu-id="80a0c-123">Leitor global</span><span class="sxs-lookup"><span data-stu-id="80a0c-123">Global reader</span></span>
* <span data-ttu-id="80a0c-124">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="80a0c-124">Privileged authentication admin</span></span>
* <span data-ttu-id="80a0c-125">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="80a0c-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="80a0c-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80a0c-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/fido2Methods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="80a0c-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80a0c-127">Request headers</span></span>
|<span data-ttu-id="80a0c-128">Nome</span><span class="sxs-lookup"><span data-stu-id="80a0c-128">Name</span></span>|<span data-ttu-id="80a0c-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="80a0c-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="80a0c-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="80a0c-130">Authorization</span></span>|<span data-ttu-id="80a0c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80a0c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="80a0c-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80a0c-133">Request body</span></span>
<span data-ttu-id="80a0c-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="80a0c-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80a0c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="80a0c-135">Response</span></span>

<span data-ttu-id="80a0c-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80a0c-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="80a0c-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="80a0c-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="80a0c-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80a0c-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/fido2Methods/_jpuR-TGZtk6aQCLF3BQjA2
```


### <a name="response"></a><span data-ttu-id="80a0c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="80a0c-140">Response</span></span>
<span data-ttu-id="80a0c-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="80a0c-141">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

