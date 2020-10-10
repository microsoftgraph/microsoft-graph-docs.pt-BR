---
title: Excluir emailAuthenticationMethod
description: Exclui um objeto emailAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 281d20e1903e05c4d131f3b2a087d5c1d2043793
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418186"
---
# <a name="delete-emailauthenticationmethod"></a><span data-ttu-id="b9f41-103">Excluir emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b9f41-103">Delete emailAuthenticationMethod</span></span>
<span data-ttu-id="b9f41-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9f41-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9f41-105">Exclui o objeto de [método de autenticação de email](../resources/emailauthenticationmethod.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="b9f41-105">Deletes a user's [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9f41-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b9f41-106">Permissions</span></span>
<span data-ttu-id="b9f41-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9f41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9f41-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9f41-109">Permission type</span></span>|<span data-ttu-id="b9f41-110">Permissões que atuam em si (de a mais de privilégios mínimos)</span><span class="sxs-lookup"><span data-stu-id="b9f41-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="b9f41-111">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b9f41-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="b9f41-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9f41-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b9f41-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9f41-113">Not supported.</span></span>|<span data-ttu-id="b9f41-114">UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b9f41-114">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="b9f41-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9f41-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9f41-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9f41-116">Not supported.</span></span>|<span data-ttu-id="b9f41-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9f41-117">Not supported.</span></span>
|<span data-ttu-id="b9f41-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9f41-118">Application</span></span>|<span data-ttu-id="b9f41-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9f41-119">Not supported.</span></span>|<span data-ttu-id="b9f41-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9f41-120">Not supported.</span></span>

<span data-ttu-id="b9f41-121">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="b9f41-121">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="b9f41-122">Administrador global</span><span class="sxs-lookup"><span data-stu-id="b9f41-122">Global admin</span></span>
* <span data-ttu-id="b9f41-123">Leitor global</span><span class="sxs-lookup"><span data-stu-id="b9f41-123">Global reader</span></span>
* <span data-ttu-id="b9f41-124">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="b9f41-124">Privileged authentication admin</span></span>
* <span data-ttu-id="b9f41-125">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="b9f41-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="b9f41-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9f41-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b9f41-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9f41-127">Request headers</span></span>
|<span data-ttu-id="b9f41-128">Nome</span><span class="sxs-lookup"><span data-stu-id="b9f41-128">Name</span></span>|<span data-ttu-id="b9f41-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9f41-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b9f41-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9f41-130">Authorization</span></span>|<span data-ttu-id="b9f41-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9f41-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9f41-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9f41-133">Request body</span></span>
<span data-ttu-id="b9f41-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b9f41-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9f41-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9f41-135">Response</span></span>

<span data-ttu-id="b9f41-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9f41-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b9f41-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b9f41-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b9f41-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9f41-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_emailauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f
```


### <a name="response"></a><span data-ttu-id="b9f41-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9f41-140">Response</span></span>
<span data-ttu-id="b9f41-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b9f41-141">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

