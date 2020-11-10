---
title: Obter emailAuthenticationMethod
description: Leia as propriedades e os relacionamentos de um objeto emailAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 35552ec9bd8d4e0910af372ebb761636595d2d9e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955424"
---
# <a name="get-emailauthenticationmethod"></a><span data-ttu-id="dd83c-103">Obter emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="dd83c-103">Get emailAuthenticationMethod</span></span>
<span data-ttu-id="dd83c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd83c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd83c-105">Recupere o objeto de [método de autenticação de email](../resources/emailauthenticationmethod.md) único de um usuário.</span><span class="sxs-lookup"><span data-stu-id="dd83c-105">Retrieve a user's single [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd83c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dd83c-106">Permissions</span></span>
<span data-ttu-id="dd83c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd83c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd83c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd83c-109">Permission type</span></span>|<span data-ttu-id="dd83c-110">Permissões que atuam em si (de a mais de privilégios mínimos)</span><span class="sxs-lookup"><span data-stu-id="dd83c-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="dd83c-111">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dd83c-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="dd83c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd83c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dd83c-113">UserAuthenticationMethod. Read, UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="dd83c-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span>|<span data-ttu-id="dd83c-114">UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="dd83c-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="dd83c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd83c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd83c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd83c-116">Not supported.</span></span>|<span data-ttu-id="dd83c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd83c-117">Not supported.</span></span>
|<span data-ttu-id="dd83c-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd83c-118">Application</span></span>|<span data-ttu-id="dd83c-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd83c-119">Not supported.</span></span>|<span data-ttu-id="dd83c-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd83c-120">Not supported.</span></span>

<span data-ttu-id="dd83c-121">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa de uma das seguintes [funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="dd83c-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="dd83c-122">Administrador global</span><span class="sxs-lookup"><span data-stu-id="dd83c-122">Global admin</span></span>
* <span data-ttu-id="dd83c-123">Leitor global</span><span class="sxs-lookup"><span data-stu-id="dd83c-123">Global reader</span></span>
* <span data-ttu-id="dd83c-124">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="dd83c-124">Privileged authentication admin</span></span>
* <span data-ttu-id="dd83c-125">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="dd83c-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="dd83c-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd83c-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/emailMethods/{id}
GET /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dd83c-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd83c-127">Request headers</span></span>
|<span data-ttu-id="dd83c-128">Nome</span><span class="sxs-lookup"><span data-stu-id="dd83c-128">Name</span></span>|<span data-ttu-id="dd83c-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd83c-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="dd83c-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd83c-130">Authorization</span></span>|<span data-ttu-id="dd83c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd83c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd83c-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd83c-133">Request body</span></span>
<span data-ttu-id="dd83c-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dd83c-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd83c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd83c-135">Response</span></span>

<span data-ttu-id="dd83c-136">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd83c-136">If successful, this method returns a `200 OK` response code and the requested [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dd83c-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dd83c-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dd83c-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd83c-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="dd83c-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd83c-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f
```
# <a name="c"></a>[<span data-ttu-id="dd83c-140">C#</span><span class="sxs-lookup"><span data-stu-id="dd83c-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-emailauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd83c-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd83c-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-emailauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd83c-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd83c-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-emailauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dd83c-143">Java</span><span class="sxs-lookup"><span data-stu-id="dd83c-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-emailauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="dd83c-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd83c-144">Response</span></span>
<span data-ttu-id="dd83c-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dd83c-145">The following is an example of the response.</span></span>

<span data-ttu-id="dd83c-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dd83c-146">**Note:** The response object shown here might be shortened for readability.</span></span>
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

