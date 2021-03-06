---
title: Listar windowsHelloForBusinessAuthenticationMethods
description: Obter uma lista dos objetos windowsHelloForBusinessAuthenticationMethod e suas propriedades.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8891e6a6afb6f2656740122081fe86aadd7bbd0f
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516366"
---
# <a name="list-windowshelloforbusinessauthenticationmethods"></a><span data-ttu-id="0f4d0-103">Listar windowsHelloForBusinessAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="0f4d0-103">List windowsHelloForBusinessAuthenticationMethods</span></span>
<span data-ttu-id="0f4d0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f4d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f4d0-105">Obter uma lista dos [objetos windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="0f4d0-105">Get a list of the [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f4d0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0f4d0-106">Permissions</span></span>

<span data-ttu-id="0f4d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f4d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="0f4d0-109">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="0f4d0-109">Permissions acting on self</span></span>

|<span data-ttu-id="0f4d0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f4d0-110">Permission type</span></span>      | <span data-ttu-id="0f4d0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0f4d0-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="0f4d0-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f4d0-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0f4d0-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0f4d0-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="0f4d0-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f4d0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f4d0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f4d0-115">Not supported.</span></span> |
| <span data-ttu-id="0f4d0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f4d0-116">Application</span></span>                            | <span data-ttu-id="0f4d0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f4d0-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="0f4d0-118">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="0f4d0-118">Permissions acting on other users</span></span>

|<span data-ttu-id="0f4d0-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f4d0-119">Permission type</span></span>      | <span data-ttu-id="0f4d0-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0f4d0-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="0f4d0-121">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f4d0-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="0f4d0-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f4d0-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="0f4d0-123">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f4d0-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f4d0-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f4d0-124">Not supported.</span></span> |
| <span data-ttu-id="0f4d0-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f4d0-125">Application</span></span>                            | <span data-ttu-id="0f4d0-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f4d0-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="0f4d0-127">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="0f4d0-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="0f4d0-128">Administrador global</span><span class="sxs-lookup"><span data-stu-id="0f4d0-128">Global admin</span></span>
* <span data-ttu-id="0f4d0-129">Leitor global</span><span class="sxs-lookup"><span data-stu-id="0f4d0-129">Global reader</span></span>
* <span data-ttu-id="0f4d0-130">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="0f4d0-130">Privileged authentication admin</span></span>
* <span data-ttu-id="0f4d0-131">Administrador de autenticação (apenas vê números de telefone mascarados)</span><span class="sxs-lookup"><span data-stu-id="0f4d0-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="0f4d0-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f4d0-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/windowsHelloForBusinessMethods
GET /users/{id | userPrincipalName}/authentication/windowsHelloForBusinessMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0f4d0-133">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0f4d0-133">Optional query parameters</span></span>

<span data-ttu-id="0f4d0-134">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f4d0-134">Not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0f4d0-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f4d0-135">Request headers</span></span>
|<span data-ttu-id="0f4d0-136">Nome</span><span class="sxs-lookup"><span data-stu-id="0f4d0-136">Name</span></span>|<span data-ttu-id="0f4d0-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f4d0-137">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0f4d0-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f4d0-138">Authorization</span></span>|<span data-ttu-id="0f4d0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f4d0-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f4d0-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f4d0-141">Request body</span></span>
<span data-ttu-id="0f4d0-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0f4d0-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f4d0-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f4d0-143">Response</span></span>

<span data-ttu-id="0f4d0-144">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f4d0-144">If successful, this method returns a `200 OK` response code and a collection of [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0f4d0-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0f4d0-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0f4d0-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f4d0-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0f4d0-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f4d0-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_windowshelloforbusinessauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/annie@contoso.com/authentication/windowsHelloForBusinessMethods
```
# <a name="c"></a>[<span data-ttu-id="0f4d0-148">C#</span><span class="sxs-lookup"><span data-stu-id="0f4d0-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-windowshelloforbusinessauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0f4d0-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0f4d0-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-windowshelloforbusinessauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0f4d0-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0f4d0-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-windowshelloforbusinessauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0f4d0-151">Java</span><span class="sxs-lookup"><span data-stu-id="0f4d0-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-windowshelloforbusinessauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="0f4d0-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f4d0-152">Response</span></span>
<span data-ttu-id="0f4d0-153">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0f4d0-153">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsHelloForBusinessAuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
      "id": "b5e01f81-1f81-b5e0-811f-e0b5811fe0b5",
      "displayName": "Jordan's Surface Book",
      "createdDateTime": "2020-11-27T23:12:49Z",
      "keyStrength": "normal"
    },
    {
      "@odata.type": "#microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
      "id": "e6dab818-e68d-433e-89d5-547357870cb2",
      "displayName": "New Surface Duo",
      "createdDateTime": "2020-12-25T02:20:13Z",
      "keyStrength": "normal"
    }
  ]
}
```

