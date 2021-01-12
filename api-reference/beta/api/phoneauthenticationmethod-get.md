---
title: Obter phoneAuthenticationMethod
description: Recupere um único objeto phoneAuthenticationMethod.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 76e0718f847b9e8eddc2b87c5a8bb523cc464a78
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796658"
---
# <a name="get-phoneauthenticationmethod"></a><span data-ttu-id="a6b5b-103">Obter phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a6b5b-103">Get phoneAuthenticationMethod</span></span>

<span data-ttu-id="a6b5b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6b5b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6b5b-105">Recupere um único [objeto phoneAuthenticationMethod.](../resources/phoneauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="a6b5b-105">Retrieve a single [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6b5b-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="a6b5b-106">Permissions</span></span>

<span data-ttu-id="a6b5b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6b5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="a6b5b-109">Permissões agindo por si só</span><span class="sxs-lookup"><span data-stu-id="a6b5b-109">Permissions acting on self</span></span>

|<span data-ttu-id="a6b5b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6b5b-110">Permission type</span></span>      | <span data-ttu-id="a6b5b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6b5b-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="a6b5b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6b5b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a6b5b-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a6b5b-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="a6b5b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6b5b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6b5b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6b5b-115">Not supported.</span></span> |
| <span data-ttu-id="a6b5b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6b5b-116">Application</span></span>                            | <span data-ttu-id="a6b5b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6b5b-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="a6b5b-118">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="a6b5b-118">Permissions acting on other users</span></span>

|<span data-ttu-id="a6b5b-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6b5b-119">Permission type</span></span>      | <span data-ttu-id="a6b5b-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6b5b-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="a6b5b-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6b5b-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="a6b5b-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6b5b-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="a6b5b-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6b5b-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6b5b-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6b5b-124">Not supported.</span></span> |
| <span data-ttu-id="a6b5b-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6b5b-125">Application</span></span>                            | <span data-ttu-id="a6b5b-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6b5b-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="a6b5b-127">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="a6b5b-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="a6b5b-128">Administração global</span><span class="sxs-lookup"><span data-stu-id="a6b5b-128">Global admin</span></span>
* <span data-ttu-id="a6b5b-129">Leitor global</span><span class="sxs-lookup"><span data-stu-id="a6b5b-129">Global reader</span></span>
* <span data-ttu-id="a6b5b-130">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="a6b5b-130">Privileged authentication admin</span></span>
* <span data-ttu-id="a6b5b-131">Administrador de autenticação (vê apenas números de telefone com máscara)</span><span class="sxs-lookup"><span data-stu-id="a6b5b-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="a6b5b-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6b5b-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/phoneMethods/{id}
GET /users/{id | userPrincipalName}/authentication/phoneMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a6b5b-133">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a6b5b-133">Optional query parameters</span></span>

<span data-ttu-id="a6b5b-134">Esse método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a6b5b-134">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6b5b-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6b5b-135">Request headers</span></span>

| <span data-ttu-id="a6b5b-136">Nome</span><span class="sxs-lookup"><span data-stu-id="a6b5b-136">Name</span></span>      |<span data-ttu-id="a6b5b-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6b5b-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a6b5b-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6b5b-138">Authorization</span></span> | <span data-ttu-id="a6b5b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6b5b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6b5b-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6b5b-141">Request body</span></span>

<span data-ttu-id="a6b5b-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a6b5b-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6b5b-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6b5b-143">Response</span></span>

<span data-ttu-id="a6b5b-144">Se bem-sucedido, este método retorna um código de resposta e o objeto `200 OK` [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6b5b-144">If successful, this method returns a `200 OK` response code and the requested [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a6b5b-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a6b5b-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a6b5b-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6b5b-146">Request</span></span>

<span data-ttu-id="a6b5b-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6b5b-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a6b5b-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6b5b-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_phoneauthenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
```
# <a name="c"></a>[<span data-ttu-id="a6b5b-149">C#</span><span class="sxs-lookup"><span data-stu-id="a6b5b-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-phoneauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a6b5b-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6b5b-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-phoneauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a6b5b-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6b5b-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-phoneauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a6b5b-152">Java</span><span class="sxs-lookup"><span data-stu-id="a6b5b-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-phoneauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a6b5b-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6b5b-153">Response</span></span>

<span data-ttu-id="a6b5b-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a6b5b-154">The following is an example of the response.</span></span>

> <span data-ttu-id="a6b5b-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6b5b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "phoneNumber": "+1 2065555555",
  "phoneType": "mobile",
  "smsSignInState": "ready",
  "id": "3179e48a-750b-4051-897c-87b9720928f7"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get phoneAuthenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
