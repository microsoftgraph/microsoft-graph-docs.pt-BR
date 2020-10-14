---
title: Obter passwordlessMicrosoftAuthenticatorAuthenticationMethod
description: Leia as propriedades e os relacionamentos de um objeto passwordlessMicrosoftAuthenticatorAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1a92e7669df96efe69d8e793fc327a8c578ffcde
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48457496"
---
# <a name="get-passwordlessmicrosoftauthenticatorauthenticationmethod"></a><span data-ttu-id="cb142-103">Obter passwordlessMicrosoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="cb142-103">Get passwordlessMicrosoftAuthenticatorAuthenticationMethod</span></span>
<span data-ttu-id="cb142-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb142-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb142-105">Recuperar um único objeto do [método de entrada de conexão sem senha do Microsoft Authenticator](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="cb142-105">Retrieve a user's single [Microsoft Authenticator Passwordless Phone Sign-in method](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="cb142-106">Alterações substanciais de esquema são planejadas para APIs que gerenciam o aplicativo Microsoft Authenticator enquanto as APIs estão no Mirosoft Graph beta.</span><span class="sxs-lookup"><span data-stu-id="cb142-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="cb142-107">Como os padrões de chamada serão alterados, recomendamos que você não faça uma dependência de produção nessas APIs.</span><span class="sxs-lookup"><span data-stu-id="cb142-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb142-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="cb142-108">Permissions</span></span>
<span data-ttu-id="cb142-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb142-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb142-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb142-111">Permission type</span></span>|<span data-ttu-id="cb142-112">Permissões que atuam em si (de a mais de privilégios mínimos)</span><span class="sxs-lookup"><span data-stu-id="cb142-112">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="cb142-113">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cb142-113">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="cb142-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb142-114">Delegated (work or school account)</span></span>|<span data-ttu-id="cb142-115">UserAuthenticationMethod. Read, UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="cb142-115">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span>|<span data-ttu-id="cb142-116">UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="cb142-116">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="cb142-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb142-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb142-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb142-118">Not supported.</span></span>|<span data-ttu-id="cb142-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb142-119">Not supported.</span></span>
|<span data-ttu-id="cb142-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cb142-120">Application</span></span>|<span data-ttu-id="cb142-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb142-121">Not supported.</span></span>|<span data-ttu-id="cb142-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb142-122">Not supported.</span></span>

<span data-ttu-id="cb142-123">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa de uma das seguintes [funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="cb142-123">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="cb142-124">Administrador global</span><span class="sxs-lookup"><span data-stu-id="cb142-124">Global admin</span></span>
* <span data-ttu-id="cb142-125">Leitor global</span><span class="sxs-lookup"><span data-stu-id="cb142-125">Global reader</span></span>
* <span data-ttu-id="cb142-126">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="cb142-126">Privileged authentication admin</span></span>
* <span data-ttu-id="cb142-127">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="cb142-127">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="cb142-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb142-128">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
GET /users/{id | userPrincipalName}/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cb142-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb142-129">Request headers</span></span>
|<span data-ttu-id="cb142-130">Nome</span><span class="sxs-lookup"><span data-stu-id="cb142-130">Name</span></span>|<span data-ttu-id="cb142-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb142-131">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cb142-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb142-132">Authorization</span></span>|<span data-ttu-id="cb142-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb142-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb142-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb142-135">Request body</span></span>
<span data-ttu-id="cb142-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cb142-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb142-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb142-137">Response</span></span>

<span data-ttu-id="cb142-138">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb142-138">If successful, this method returns a `200 OK` response code and the requested [passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cb142-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cb142-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cb142-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb142-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="cb142-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="cb142-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordlessmicrosoftauthenticatorauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/passwordlessMicrosoftAuthenticatorMethods/R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1
```
# <a name="c"></a>[<span data-ttu-id="cb142-142">C#</span><span class="sxs-lookup"><span data-stu-id="cb142-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordlessmicrosoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cb142-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cb142-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordlessmicrosoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cb142-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cb142-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordlessmicrosoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="cb142-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb142-145">Response</span></span>
<span data-ttu-id="cb142-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cb142-146">The following is an example of the response.</span></span>

<span data-ttu-id="cb142-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cb142-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": {
      "id": "R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1",
      "displayName": "My mobile phone",
      "creationDateTime": "2020-09-02T04:16:49Z"
  }
}
```

