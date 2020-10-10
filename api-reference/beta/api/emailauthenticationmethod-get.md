---
title: Obter emailAuthenticationMethod
description: Leia as propriedades e os relacionamentos de um objeto emailAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6041eb67d4bec818ccc25946559bd26a1a7b7bce
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418187"
---
# <a name="get-emailauthenticationmethod"></a><span data-ttu-id="e08f3-103">Obter emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e08f3-103">Get emailAuthenticationMethod</span></span>
<span data-ttu-id="e08f3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e08f3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e08f3-105">Recupere o objeto de [método de autenticação de email](../resources/emailauthenticationmethod.md) único de um usuário.</span><span class="sxs-lookup"><span data-stu-id="e08f3-105">Retrieve a user's single [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e08f3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e08f3-106">Permissions</span></span>
<span data-ttu-id="e08f3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e08f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e08f3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e08f3-109">Permission type</span></span>|<span data-ttu-id="e08f3-110">Permissões que atuam em si (de a mais de privilégios mínimos)</span><span class="sxs-lookup"><span data-stu-id="e08f3-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="e08f3-111">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e08f3-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="e08f3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e08f3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e08f3-113">UserAuthenticationMethod. Read, UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e08f3-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span>|<span data-ttu-id="e08f3-114">UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e08f3-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="e08f3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e08f3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e08f3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e08f3-116">Not supported.</span></span>|<span data-ttu-id="e08f3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e08f3-117">Not supported.</span></span>
|<span data-ttu-id="e08f3-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e08f3-118">Application</span></span>|<span data-ttu-id="e08f3-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e08f3-119">Not supported.</span></span>|<span data-ttu-id="e08f3-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e08f3-120">Not supported.</span></span>

<span data-ttu-id="e08f3-121">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa de uma das seguintes [funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="e08f3-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="e08f3-122">Administrador global</span><span class="sxs-lookup"><span data-stu-id="e08f3-122">Global admin</span></span>
* <span data-ttu-id="e08f3-123">Leitor global</span><span class="sxs-lookup"><span data-stu-id="e08f3-123">Global reader</span></span>
* <span data-ttu-id="e08f3-124">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="e08f3-124">Privileged authentication admin</span></span>
* <span data-ttu-id="e08f3-125">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="e08f3-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="e08f3-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e08f3-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/emailMethods/{id}
GET /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e08f3-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e08f3-127">Request headers</span></span>
|<span data-ttu-id="e08f3-128">Nome</span><span class="sxs-lookup"><span data-stu-id="e08f3-128">Name</span></span>|<span data-ttu-id="e08f3-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="e08f3-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e08f3-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="e08f3-130">Authorization</span></span>|<span data-ttu-id="e08f3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e08f3-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e08f3-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e08f3-133">Request body</span></span>
<span data-ttu-id="e08f3-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e08f3-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e08f3-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e08f3-135">Response</span></span>

<span data-ttu-id="e08f3-136">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e08f3-136">If successful, this method returns a `200 OK` response code and the requested [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e08f3-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e08f3-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e08f3-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e08f3-138">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f
```


### <a name="response"></a><span data-ttu-id="e08f3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e08f3-139">Response</span></span>
<span data-ttu-id="e08f3-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e08f3-140">The following is an example of the response.</span></span>

<span data-ttu-id="e08f3-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e08f3-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": {
      "id": "3ddfcfc8-9383-446f-83cc-3ab9be4be18f",
      "emailAddress": "Kim@contoso.com"
  }
}
```

