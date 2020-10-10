---
title: Obter passwordlessMicrosoftAuthenticatorAuthenticationMethod
description: Leia as propriedades e os relacionamentos de um objeto passwordlessMicrosoftAuthenticatorAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8402360e4d4ca87afe2f09aa5b03a52e452aa0a8
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418219"
---
# <a name="get-passwordlessmicrosoftauthenticatorauthenticationmethod"></a><span data-ttu-id="f7fc9-103">Obter passwordlessMicrosoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f7fc9-103">Get passwordlessMicrosoftAuthenticatorAuthenticationMethod</span></span>
<span data-ttu-id="f7fc9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7fc9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7fc9-105">Recuperar um único objeto do [método de entrada de conexão sem senha do Microsoft Authenticator](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f7fc9-105">Retrieve a user's single [Microsoft Authenticator Passwordless Phone Sign-in method](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="f7fc9-106">Alterações substanciais de esquema são planejadas para APIs que gerenciam o aplicativo Microsoft Authenticator enquanto as APIs estão no Mirosoft Graph beta.</span><span class="sxs-lookup"><span data-stu-id="f7fc9-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="f7fc9-107">Como os padrões de chamada serão alterados, recomendamos que você não faça uma dependência de produção nessas APIs.</span><span class="sxs-lookup"><span data-stu-id="f7fc9-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7fc9-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7fc9-108">Permissions</span></span>
<span data-ttu-id="f7fc9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7fc9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7fc9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7fc9-111">Permission type</span></span>|<span data-ttu-id="f7fc9-112">Permissões que atuam em si (de a mais de privilégios mínimos)</span><span class="sxs-lookup"><span data-stu-id="f7fc9-112">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="f7fc9-113">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7fc9-113">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="f7fc9-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7fc9-114">Delegated (work or school account)</span></span>|<span data-ttu-id="f7fc9-115">UserAuthenticationMethod. Read, UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f7fc9-115">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span>|<span data-ttu-id="f7fc9-116">UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f7fc9-116">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="f7fc9-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7fc9-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7fc9-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7fc9-118">Not supported.</span></span>|<span data-ttu-id="f7fc9-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7fc9-119">Not supported.</span></span>
|<span data-ttu-id="f7fc9-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7fc9-120">Application</span></span>|<span data-ttu-id="f7fc9-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7fc9-121">Not supported.</span></span>|<span data-ttu-id="f7fc9-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7fc9-122">Not supported.</span></span>

<span data-ttu-id="f7fc9-123">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa de uma das seguintes [funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="f7fc9-123">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="f7fc9-124">Administrador global</span><span class="sxs-lookup"><span data-stu-id="f7fc9-124">Global admin</span></span>
* <span data-ttu-id="f7fc9-125">Leitor global</span><span class="sxs-lookup"><span data-stu-id="f7fc9-125">Global reader</span></span>
* <span data-ttu-id="f7fc9-126">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="f7fc9-126">Privileged authentication admin</span></span>
* <span data-ttu-id="f7fc9-127">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="f7fc9-127">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="f7fc9-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7fc9-128">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
GET /users/{id | userPrincipalName}/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f7fc9-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7fc9-129">Request headers</span></span>
|<span data-ttu-id="f7fc9-130">Nome</span><span class="sxs-lookup"><span data-stu-id="f7fc9-130">Name</span></span>|<span data-ttu-id="f7fc9-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7fc9-131">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f7fc9-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7fc9-132">Authorization</span></span>|<span data-ttu-id="f7fc9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7fc9-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7fc9-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7fc9-135">Request body</span></span>
<span data-ttu-id="f7fc9-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f7fc9-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7fc9-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7fc9-137">Response</span></span>

<span data-ttu-id="f7fc9-138">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7fc9-138">If successful, this method returns a `200 OK` response code and the requested [passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f7fc9-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f7fc9-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f7fc9-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7fc9-140">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_passwordlessmicrosoftauthenticatorauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/passwordlessMicrosoftAuthenticatorMethods/R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1
```


### <a name="response"></a><span data-ttu-id="f7fc9-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7fc9-141">Response</span></span>
<span data-ttu-id="f7fc9-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f7fc9-142">The following is an example of the response.</span></span>

<span data-ttu-id="f7fc9-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f7fc9-143">**Note:** The response object shown here might be shortened for readability.</span></span>
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

