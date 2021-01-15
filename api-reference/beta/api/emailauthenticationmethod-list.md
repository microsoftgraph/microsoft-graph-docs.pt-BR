---
title: Listar emailAuthenticationMethods
description: Obter uma lista dos objetos emailAuthenticationMethod e suas propriedades.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bc1ef69b988c0e0aab2921b63fe0a08b545649f4
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49871985"
---
# <a name="list-emailauthenticationmethods"></a><span data-ttu-id="16988-103">Listar emailAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="16988-103">List emailAuthenticationMethods</span></span>
<span data-ttu-id="16988-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16988-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16988-105">Recupere uma lista de objetos do Método de Autenticação de [email de](../resources/emailauthenticationmethod.md) um usuário e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="16988-105">Retrieve a list of a user's [email Authentication Method](../resources/emailauthenticationmethod.md) objects and their properties.</span></span> <span data-ttu-id="16988-106">Essa chamada retornará apenas um único objeto, pois apenas um método de email pode ser definido para os usuários.</span><span class="sxs-lookup"><span data-stu-id="16988-106">This call will only return a single object as only one email method can be set on users.</span></span>

## <a name="permissions"></a><span data-ttu-id="16988-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="16988-107">Permissions</span></span>
<span data-ttu-id="16988-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16988-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16988-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16988-110">Permission type</span></span>|<span data-ttu-id="16988-111">Permissões atuando por si mesmo (do menos para o mais privilegiado)</span><span class="sxs-lookup"><span data-stu-id="16988-111">Permissions acting on self (from least to most privileged)</span></span>|<span data-ttu-id="16988-112">Permissões atuando em outras pessoas (de menos para mais privilegiados)</span><span class="sxs-lookup"><span data-stu-id="16988-112">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="16988-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16988-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="16988-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16988-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="16988-115">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16988-115">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="16988-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16988-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16988-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16988-117">Not supported.</span></span> | <span data-ttu-id="16988-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16988-118">Not supported.</span></span> |
| <span data-ttu-id="16988-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16988-119">Application</span></span>                            | <span data-ttu-id="16988-120">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="16988-120">Not applicable.</span></span> | <span data-ttu-id="16988-121">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16988-121">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="16988-122">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa de uma das seguintes [funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="16988-122">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="16988-123">Administrador global</span><span class="sxs-lookup"><span data-stu-id="16988-123">Global admin</span></span>
* <span data-ttu-id="16988-124">Leitor global</span><span class="sxs-lookup"><span data-stu-id="16988-124">Global reader</span></span>
* <span data-ttu-id="16988-125">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="16988-125">Privileged authentication admin</span></span>
* <span data-ttu-id="16988-126">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="16988-126">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="16988-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16988-127">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/emailMethods
GET /users/{id | userPrincipalName}/authentication/emailMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="16988-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="16988-128">Optional query parameters</span></span>
<span data-ttu-id="16988-129">Esse método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="16988-129">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16988-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16988-130">Request headers</span></span>
|<span data-ttu-id="16988-131">Nome</span><span class="sxs-lookup"><span data-stu-id="16988-131">Name</span></span>|<span data-ttu-id="16988-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="16988-132">Description</span></span>|
|:---|:---|
|<span data-ttu-id="16988-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="16988-133">Authorization</span></span>|<span data-ttu-id="16988-134">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="16988-134">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="16988-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16988-135">Request body</span></span>
<span data-ttu-id="16988-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="16988-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16988-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="16988-137">Response</span></span>

<span data-ttu-id="16988-138">Se bem-sucedido, este método retorna um código de resposta e uma coleção de `200 OK` [objetos emailAuthenticationMethod](../resources/emailauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16988-138">If successful, this method returns a `200 OK` response code and a collection of [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="16988-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="16988-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="16988-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16988-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="16988-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="16988-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/emailMethods
```
# <a name="c"></a>[<span data-ttu-id="16988-142">C#</span><span class="sxs-lookup"><span data-stu-id="16988-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-emailauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16988-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16988-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-emailauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16988-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16988-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-emailauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="16988-145">Java</span><span class="sxs-lookup"><span data-stu-id="16988-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-emailauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="16988-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="16988-146">Response</span></span>
<span data-ttu-id="16988-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="16988-147">The following is an example of the response.</span></span>

<span data-ttu-id="16988-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="16988-148">**Note:** The response object shown here might be shortened for readability.</span></span>
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

