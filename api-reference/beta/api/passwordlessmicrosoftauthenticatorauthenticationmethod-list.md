---
title: Listar passwordlessMicrosoftAuthenticatorAuthenticationMethods
description: Recupere uma lista dos objetos passwordlessMicrosoftAuthenticatorAuthenticationMethod e suas propriedades.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7ae837eb7938a1734f30402e24db31c96cb0f587
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968606"
---
# <a name="list-passwordlessmicrosoftauthenticatorauthenticationmethods"></a><span data-ttu-id="060aa-103">Listar passwordlessMicrosoftAuthenticatorAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="060aa-103">List passwordlessMicrosoftAuthenticatorAuthenticationMethods</span></span>
<span data-ttu-id="060aa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="060aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="060aa-105">Recupere uma lista de objetos de [método de entrada sem senha do autenticador](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) de um usuário do Microsoft Authenticator e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="060aa-105">Retrieve a list of a user's [Microsoft Authenticator Passwordless Phone Sign-in method](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) objects and their properties.</span></span>

> [!NOTE]
> <span data-ttu-id="060aa-106">Alterações substanciais de esquema são planejadas para APIs que gerenciam o aplicativo Microsoft Authenticator enquanto as APIs estão no Mirosoft Graph beta.</span><span class="sxs-lookup"><span data-stu-id="060aa-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="060aa-107">Como os padrões de chamada serão alterados, recomendamos que você não faça uma dependência de produção nessas APIs.</span><span class="sxs-lookup"><span data-stu-id="060aa-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>

## <a name="permissions"></a><span data-ttu-id="060aa-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="060aa-108">Permissions</span></span>
<span data-ttu-id="060aa-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="060aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="060aa-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="060aa-111">Permission type</span></span>|<span data-ttu-id="060aa-112">Permissões que atuam em si (de a mais de privilégios mínimos)</span><span class="sxs-lookup"><span data-stu-id="060aa-112">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="060aa-113">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="060aa-113">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="060aa-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="060aa-114">Delegated (work or school account)</span></span>|<span data-ttu-id="060aa-115">UserAuthenticationMethod. Read, UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="060aa-115">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span>|<span data-ttu-id="060aa-116">UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="060aa-116">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="060aa-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="060aa-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="060aa-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="060aa-118">Not supported.</span></span>|<span data-ttu-id="060aa-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="060aa-119">Not supported.</span></span>
|<span data-ttu-id="060aa-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="060aa-120">Application</span></span>|<span data-ttu-id="060aa-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="060aa-121">Not supported.</span></span>|<span data-ttu-id="060aa-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="060aa-122">Not supported.</span></span>

<span data-ttu-id="060aa-123">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa de uma das seguintes [funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="060aa-123">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="060aa-124">Administrador global</span><span class="sxs-lookup"><span data-stu-id="060aa-124">Global admin</span></span>
* <span data-ttu-id="060aa-125">Leitor global</span><span class="sxs-lookup"><span data-stu-id="060aa-125">Global reader</span></span>
* <span data-ttu-id="060aa-126">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="060aa-126">Privileged authentication admin</span></span>
* <span data-ttu-id="060aa-127">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="060aa-127">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="060aa-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="060aa-128">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/passwordlessMicrosoftAuthenticatorMethods
GET /users/{id | userPrincipalName}/authentication/passwordlessMicrosoftAuthenticatorMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="060aa-129">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="060aa-129">Optional query parameters</span></span>
<span data-ttu-id="060aa-130">Este método não oferece suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="060aa-130">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="060aa-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="060aa-131">Request headers</span></span>
|<span data-ttu-id="060aa-132">Nome</span><span class="sxs-lookup"><span data-stu-id="060aa-132">Name</span></span>|<span data-ttu-id="060aa-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="060aa-133">Description</span></span>|
|:---|:---|
|<span data-ttu-id="060aa-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="060aa-134">Authorization</span></span>|<span data-ttu-id="060aa-135">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="060aa-135">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="060aa-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="060aa-136">Request body</span></span>
<span data-ttu-id="060aa-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="060aa-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="060aa-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="060aa-138">Response</span></span>

<span data-ttu-id="060aa-139">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="060aa-139">If successful, this method returns a `200 OK` response code and a collection of [passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="060aa-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="060aa-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="060aa-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="060aa-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="060aa-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="060aa-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordlessmicrosoftauthenticatorauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/passwordlessMicrosoftAuthenticatorMethods
```
# <a name="c"></a>[<span data-ttu-id="060aa-143">C#</span><span class="sxs-lookup"><span data-stu-id="060aa-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordlessmicrosoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="060aa-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="060aa-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordlessmicrosoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="060aa-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="060aa-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordlessmicrosoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="060aa-146">Java</span><span class="sxs-lookup"><span data-stu-id="060aa-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-passwordlessmicrosoftauthenticatorauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="060aa-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="060aa-147">Response</span></span>
<span data-ttu-id="060aa-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="060aa-148">The following is an example of the response.</span></span>

<span data-ttu-id="060aa-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="060aa-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": [
    {
      "id": "R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1",
      "displayName": "My mobile phone",
      "creationDateTime": "2020-09-02T04:16:49Z"
    },
    {
      "id": "J18B378Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJGM1",
      "displayName": "My tablet",
      "creationDateTime": "2020-09-02T03:36:19Z"
    }
  ]
}
```

