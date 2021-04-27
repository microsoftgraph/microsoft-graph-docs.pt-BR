---
title: Obter temporaryAccessPassAuthenticationMethod
description: Leia as propriedades e as relações de um objeto temporaryAccessPassAuthenticationMethod.
author: inbarckMS
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ccaa0d574c2fb2261c8cb0e0e0091473ec389f1f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049671"
---
# <a name="get-temporaryaccesspassauthenticationmethod"></a><span data-ttu-id="9798f-103">Obter temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9798f-103">Get temporaryAccessPassAuthenticationMethod</span></span>
<span data-ttu-id="9798f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9798f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9798f-105">Recupere o único objeto  [temporaryAccessPassAuthenticationMethod de um](../resources/temporaryaccesspassauthenticationmethod.md) usuário.</span><span class="sxs-lookup"><span data-stu-id="9798f-105">Retrieve a user's single  [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9798f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9798f-106">Permissions</span></span>
<span data-ttu-id="9798f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9798f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="9798f-109">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="9798f-109">Permissions acting on self</span></span>

|<span data-ttu-id="9798f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9798f-110">Permission type</span></span>      | <span data-ttu-id="9798f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9798f-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="9798f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9798f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9798f-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9798f-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="9798f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9798f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9798f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9798f-115">Not supported.</span></span> |
| <span data-ttu-id="9798f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9798f-116">Application</span></span>                            | <span data-ttu-id="9798f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9798f-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="9798f-118">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="9798f-118">Permissions acting on other users</span></span>

|<span data-ttu-id="9798f-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9798f-119">Permission type</span></span>      | <span data-ttu-id="9798f-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9798f-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="9798f-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9798f-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="9798f-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9798f-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="9798f-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9798f-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9798f-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9798f-124">Not supported.</span></span> |
| <span data-ttu-id="9798f-125">Application</span><span class="sxs-lookup"><span data-stu-id="9798f-125">Application</span></span>                            | <span data-ttu-id="9798f-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9798f-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="9798f-127">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="9798f-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="9798f-128">Administração global</span><span class="sxs-lookup"><span data-stu-id="9798f-128">Global admin</span></span>
* <span data-ttu-id="9798f-129">Leitor global</span><span class="sxs-lookup"><span data-stu-id="9798f-129">Global reader</span></span>
* <span data-ttu-id="9798f-130">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="9798f-130">Privileged authentication admin</span></span>
* <span data-ttu-id="9798f-131">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="9798f-131">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="9798f-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9798f-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/temporaryAccessPassMethods/{temporaryAccessPassAuthenticationMethodId}
GET /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods/{temporaryAccessPassAuthenticationMethodId}
```


## <a name="request-headers"></a><span data-ttu-id="9798f-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9798f-133">Request headers</span></span>
|<span data-ttu-id="9798f-134">Nome</span><span class="sxs-lookup"><span data-stu-id="9798f-134">Name</span></span>|<span data-ttu-id="9798f-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="9798f-135">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9798f-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="9798f-136">Authorization</span></span>|<span data-ttu-id="9798f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9798f-p102">Bearer {token}. Required.</span></span>|


## <a name="request-body"></a><span data-ttu-id="9798f-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9798f-139">Request body</span></span>
<span data-ttu-id="9798f-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9798f-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9798f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="9798f-141">Response</span></span>

<span data-ttu-id="9798f-142">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9798f-142">If successful, this method returns a `200 OK` response code and a [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9798f-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9798f-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9798f-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9798f-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9798f-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="9798f-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_temporaryaccesspassauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/temporaryAccessPassMethods/30fd0dfc-0dfc-30fd-fc0d-fd30fc0dfd30
```
# <a name="c"></a>[<span data-ttu-id="9798f-146">C#</span><span class="sxs-lookup"><span data-stu-id="9798f-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-temporaryaccesspassauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9798f-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9798f-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-temporaryaccesspassauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9798f-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9798f-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-temporaryaccesspassauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9798f-149">Java</span><span class="sxs-lookup"><span data-stu-id="9798f-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-temporaryaccesspassauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="9798f-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="9798f-150">Response</span></span>
<span data-ttu-id="9798f-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9798f-151">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.temporaryAccessPassAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
    "id": "30fd0dfc-0dfc-30fd-fc0d-fd30fc0dfd30",
    "temporaryAccessPass": null,
    "createdDateTime": "String (timestamp)",
    "startDateTime": "String (timestamp)",
    "lifetimeInMinutes": "Integer",
    "isUsableOnce": "Boolean",
    "isUsable": "Boolean",
    "methodUsabilityReason": "String"
  }
}
```
