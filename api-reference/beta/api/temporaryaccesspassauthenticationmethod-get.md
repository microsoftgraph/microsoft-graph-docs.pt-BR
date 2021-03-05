---
title: Obter temporaryAccessPassAuthenticationMethod
description: Leia as propriedades e as relações de um objeto temporaryAccessPassAuthenticationMethod.
author: inbarckMS
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 515218cc365c9d46bf0aaa7f419b542702ed27fa
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475092"
---
# <a name="get-temporaryaccesspassauthenticationmethod"></a><span data-ttu-id="af5a8-103">Obter temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="af5a8-103">Get temporaryAccessPassAuthenticationMethod</span></span>
<span data-ttu-id="af5a8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af5a8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af5a8-105">Recupere o único objeto  [temporaryAccessPassAuthenticationMethod de um](../resources/temporaryaccesspassauthenticationmethod.md) usuário.</span><span class="sxs-lookup"><span data-stu-id="af5a8-105">Retrieve a user's single  [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="af5a8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="af5a8-106">Permissions</span></span>
<span data-ttu-id="af5a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af5a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="af5a8-109">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="af5a8-109">Permissions acting on self</span></span>

|<span data-ttu-id="af5a8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af5a8-110">Permission type</span></span>      | <span data-ttu-id="af5a8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="af5a8-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="af5a8-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af5a8-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="af5a8-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="af5a8-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="af5a8-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af5a8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af5a8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af5a8-115">Not supported.</span></span> |
| <span data-ttu-id="af5a8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af5a8-116">Application</span></span>                            | <span data-ttu-id="af5a8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af5a8-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="af5a8-118">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="af5a8-118">Permissions acting on other users</span></span>

|<span data-ttu-id="af5a8-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af5a8-119">Permission type</span></span>      | <span data-ttu-id="af5a8-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="af5a8-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="af5a8-121">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af5a8-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="af5a8-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af5a8-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="af5a8-123">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af5a8-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af5a8-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af5a8-124">Not supported.</span></span> |
| <span data-ttu-id="af5a8-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af5a8-125">Application</span></span>                            | <span data-ttu-id="af5a8-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af5a8-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="af5a8-127">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="af5a8-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="af5a8-128">Administrador global</span><span class="sxs-lookup"><span data-stu-id="af5a8-128">Global admin</span></span>
* <span data-ttu-id="af5a8-129">Leitor global</span><span class="sxs-lookup"><span data-stu-id="af5a8-129">Global reader</span></span>
* <span data-ttu-id="af5a8-130">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="af5a8-130">Privileged authentication admin</span></span>
* <span data-ttu-id="af5a8-131">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="af5a8-131">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="af5a8-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af5a8-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/temporaryAccessPassMethods/{temporaryAccessPassAuthenticationMethodId}
GET /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods/{temporaryAccessPassAuthenticationMethodId}
```


## <a name="request-headers"></a><span data-ttu-id="af5a8-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af5a8-133">Request headers</span></span>
|<span data-ttu-id="af5a8-134">Nome</span><span class="sxs-lookup"><span data-stu-id="af5a8-134">Name</span></span>|<span data-ttu-id="af5a8-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="af5a8-135">Description</span></span>|
|:---|:---|
|<span data-ttu-id="af5a8-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="af5a8-136">Authorization</span></span>|<span data-ttu-id="af5a8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af5a8-p102">Bearer {token}. Required.</span></span>|


## <a name="request-body"></a><span data-ttu-id="af5a8-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af5a8-139">Request body</span></span>
<span data-ttu-id="af5a8-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="af5a8-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af5a8-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="af5a8-141">Response</span></span>

<span data-ttu-id="af5a8-142">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af5a8-142">If successful, this method returns a `200 OK` response code and a [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="af5a8-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="af5a8-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="af5a8-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af5a8-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="af5a8-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="af5a8-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_temporaryaccesspassauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/temporaryAccessPassMethods/30fd0dfc-0dfc-30fd-fc0d-fd30fc0dfd30
```
# <a name="c"></a>[<span data-ttu-id="af5a8-146">C#</span><span class="sxs-lookup"><span data-stu-id="af5a8-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-temporaryaccesspassauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="af5a8-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="af5a8-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-temporaryaccesspassauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="af5a8-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="af5a8-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-temporaryaccesspassauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="af5a8-149">Java</span><span class="sxs-lookup"><span data-stu-id="af5a8-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-temporaryaccesspassauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="af5a8-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="af5a8-150">Response</span></span>
<span data-ttu-id="af5a8-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="af5a8-151">**Note:** The response object shown here might be shortened for readability.</span></span>
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
