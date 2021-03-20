---
title: Listar emailAuthenticationMethods
description: Obter uma lista dos objetos emailAuthenticationMethod e suas propriedades.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6ed898bdbea7c8db3fe7fe2d97fd1d4db789241f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950981"
---
# <a name="list-emailauthenticationmethods"></a><span data-ttu-id="24efd-103">Listar emailAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="24efd-103">List emailAuthenticationMethods</span></span>
<span data-ttu-id="24efd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24efd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24efd-105">Recupere uma lista de objetos do Método de Autenticação de [email](../resources/emailauthenticationmethod.md) de um usuário e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="24efd-105">Retrieve a list of a user's [email Authentication Method](../resources/emailauthenticationmethod.md) objects and their properties.</span></span> <span data-ttu-id="24efd-106">Essa chamada retornará apenas um único objeto, pois apenas um método de email pode ser definido nos usuários.</span><span class="sxs-lookup"><span data-stu-id="24efd-106">This call will only return a single object as only one email method can be set on users.</span></span>

## <a name="permissions"></a><span data-ttu-id="24efd-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="24efd-107">Permissions</span></span>
<span data-ttu-id="24efd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24efd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24efd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24efd-110">Permission type</span></span>|<span data-ttu-id="24efd-111">Permissões agindo por si mesmo (do mínimo para o mais privilegiado)</span><span class="sxs-lookup"><span data-stu-id="24efd-111">Permissions acting on self (from least to most privileged)</span></span>|<span data-ttu-id="24efd-112">Permissões atuando em outras pessoas (do mínimo ao mais privilegiado)</span><span class="sxs-lookup"><span data-stu-id="24efd-112">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="24efd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24efd-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="24efd-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24efd-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="24efd-115">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24efd-115">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="24efd-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24efd-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24efd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24efd-117">Not supported.</span></span> | <span data-ttu-id="24efd-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24efd-118">Not supported.</span></span> |
| <span data-ttu-id="24efd-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24efd-119">Application</span></span>                            | <span data-ttu-id="24efd-120">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="24efd-120">Not applicable.</span></span> | <span data-ttu-id="24efd-121">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24efd-121">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="24efd-122">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma das seguintes [funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="24efd-122">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="24efd-123">Administrador global</span><span class="sxs-lookup"><span data-stu-id="24efd-123">Global admin</span></span>
* <span data-ttu-id="24efd-124">Leitor global</span><span class="sxs-lookup"><span data-stu-id="24efd-124">Global reader</span></span>
* <span data-ttu-id="24efd-125">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="24efd-125">Privileged authentication admin</span></span>
* <span data-ttu-id="24efd-126">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="24efd-126">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="24efd-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24efd-127">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/emailMethods
GET /users/{id | userPrincipalName}/authentication/emailMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="24efd-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="24efd-128">Optional query parameters</span></span>
<span data-ttu-id="24efd-129">Este método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="24efd-129">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="24efd-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24efd-130">Request headers</span></span>
|<span data-ttu-id="24efd-131">Nome</span><span class="sxs-lookup"><span data-stu-id="24efd-131">Name</span></span>|<span data-ttu-id="24efd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="24efd-132">Description</span></span>|
|:---|:---|
|<span data-ttu-id="24efd-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="24efd-133">Authorization</span></span>|<span data-ttu-id="24efd-134">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="24efd-134">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="24efd-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24efd-135">Request body</span></span>
<span data-ttu-id="24efd-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="24efd-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24efd-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="24efd-137">Response</span></span>

<span data-ttu-id="24efd-138">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos emailAuthenticationMethod](../resources/emailauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24efd-138">If successful, this method returns a `200 OK` response code and a collection of [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="24efd-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="24efd-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="24efd-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24efd-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="24efd-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="24efd-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethod_2"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/emailMethods
```
# <a name="c"></a>[<span data-ttu-id="24efd-142">C#</span><span class="sxs-lookup"><span data-stu-id="24efd-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-emailauthenticationmethod-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="24efd-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="24efd-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-emailauthenticationmethod-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="24efd-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="24efd-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-emailauthenticationmethod-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="24efd-145">Java</span><span class="sxs-lookup"><span data-stu-id="24efd-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-emailauthenticationmethod-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="24efd-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="24efd-146">Response</span></span>
<span data-ttu-id="24efd-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="24efd-147">The following is an example of the response.</span></span>

<span data-ttu-id="24efd-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="24efd-148">**Note:** The response object shown here might be shortened for readability.</span></span>
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

