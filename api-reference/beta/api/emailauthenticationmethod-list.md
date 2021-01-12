---
title: Listar emailAuthenticationMethods
description: Obter uma lista dos objetos emailAuthenticationMethod e suas propriedades.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 53d6e3ff9c1fa98196a838d185551c28754f0516
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796454"
---
# <a name="list-emailauthenticationmethods"></a><span data-ttu-id="c4268-103">Listar emailAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="c4268-103">List emailAuthenticationMethods</span></span>
<span data-ttu-id="c4268-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4268-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4268-105">Recupere uma lista de objetos do Método de Autenticação de [email de](../resources/emailauthenticationmethod.md) um usuário e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="c4268-105">Retrieve a list of a user's [email Authentication Method](../resources/emailauthenticationmethod.md) objects and their properties.</span></span> <span data-ttu-id="c4268-106">Essa chamada retornará apenas um único objeto, pois apenas um método de email pode ser definido para os usuários.</span><span class="sxs-lookup"><span data-stu-id="c4268-106">This call will only return a single object as only one email method can be set on users.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4268-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="c4268-107">Permissions</span></span>
<span data-ttu-id="c4268-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4268-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4268-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4268-110">Permission type</span></span>|<span data-ttu-id="c4268-111">Permissões atuando por si mesmo (do mais para o menos privilegiado)</span><span class="sxs-lookup"><span data-stu-id="c4268-111">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="c4268-112">Permissões atuando em outras pessoas (de menos para mais privilegiados)</span><span class="sxs-lookup"><span data-stu-id="c4268-112">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="c4268-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4268-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c4268-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4268-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="c4268-115">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4268-115">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="c4268-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4268-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4268-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4268-117">Not supported.</span></span> | <span data-ttu-id="c4268-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4268-118">Not supported.</span></span> |
| <span data-ttu-id="c4268-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4268-119">Application</span></span>                            | <span data-ttu-id="c4268-120">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="c4268-120">Not applicable.</span></span> | <span data-ttu-id="c4268-121">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4268-121">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="c4268-122">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa de uma das seguintes [funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="c4268-122">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="c4268-123">Administração global</span><span class="sxs-lookup"><span data-stu-id="c4268-123">Global admin</span></span>
* <span data-ttu-id="c4268-124">Leitor global</span><span class="sxs-lookup"><span data-stu-id="c4268-124">Global reader</span></span>
* <span data-ttu-id="c4268-125">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="c4268-125">Privileged authentication admin</span></span>
* <span data-ttu-id="c4268-126">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="c4268-126">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="c4268-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4268-127">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/emailMethods
GET /users/{id | userPrincipalName}/authentication/emailMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c4268-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c4268-128">Optional query parameters</span></span>
<span data-ttu-id="c4268-129">Esse método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c4268-129">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4268-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4268-130">Request headers</span></span>
|<span data-ttu-id="c4268-131">Nome</span><span class="sxs-lookup"><span data-stu-id="c4268-131">Name</span></span>|<span data-ttu-id="c4268-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4268-132">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c4268-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4268-133">Authorization</span></span>|<span data-ttu-id="c4268-134">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="c4268-134">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4268-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4268-135">Request body</span></span>
<span data-ttu-id="c4268-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c4268-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4268-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4268-137">Response</span></span>

<span data-ttu-id="c4268-138">Se bem-sucedido, este método retorna um código de resposta e uma coleção de `200 OK` [objetos emailAuthenticationMethod](../resources/emailauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4268-138">If successful, this method returns a `200 OK` response code and a collection of [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c4268-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c4268-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c4268-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4268-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c4268-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4268-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/emailMethods
```
# <a name="c"></a>[<span data-ttu-id="c4268-142">C#</span><span class="sxs-lookup"><span data-stu-id="c4268-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-emailauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4268-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4268-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-emailauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4268-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4268-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-emailauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c4268-145">Java</span><span class="sxs-lookup"><span data-stu-id="c4268-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-emailauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c4268-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4268-146">Response</span></span>
<span data-ttu-id="c4268-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c4268-147">The following is an example of the response.</span></span>

<span data-ttu-id="c4268-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c4268-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.emailAuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": [
    {
      "id": "3ddfcfc8-9383-446f-83cc-3ab9be4be18f",
      "emailAddress": "Kim@contoso.com"
    }
  ]
}
```

