---
title: Obter passwordAuthenticationMethod
description: Recupere as propriedades e os relacionamentos do objeto passwordauthenticationmethod.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cf24e7b30a2cd38830a4291bf4a698b728a7b0cf
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796651"
---
# <a name="get-passwordauthenticationmethod"></a><span data-ttu-id="ac903-103">Obter passwordAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ac903-103">Get passwordAuthenticationMethod</span></span>

<span data-ttu-id="ac903-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac903-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac903-105">Recupere as propriedades e os relacionamentos de um objeto de método [de autenticação de](../resources/passwordauthenticationmethod.md) senha.</span><span class="sxs-lookup"><span data-stu-id="ac903-105">Retrieve the properties and relationships of a [password authentication method](../resources/passwordauthenticationmethod.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="ac903-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="ac903-106">Permissions</span></span>

<span data-ttu-id="ac903-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac903-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="ac903-109">Permissões agindo por si só</span><span class="sxs-lookup"><span data-stu-id="ac903-109">Permissions acting on self</span></span>

|<span data-ttu-id="ac903-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac903-110">Permission type</span></span>      | <span data-ttu-id="ac903-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ac903-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="ac903-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac903-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ac903-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ac903-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="ac903-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac903-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac903-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac903-115">Not supported.</span></span> |
| <span data-ttu-id="ac903-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac903-116">Application</span></span>                            | <span data-ttu-id="ac903-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac903-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="ac903-118">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="ac903-118">Permissions acting on other users</span></span>

|<span data-ttu-id="ac903-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac903-119">Permission type</span></span>      | <span data-ttu-id="ac903-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ac903-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="ac903-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac903-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="ac903-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac903-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="ac903-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac903-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac903-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac903-124">Not supported.</span></span> |
| <span data-ttu-id="ac903-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac903-125">Application</span></span>                            | <span data-ttu-id="ac903-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac903-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="ac903-127">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="ac903-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="ac903-128">Administração global</span><span class="sxs-lookup"><span data-stu-id="ac903-128">Global admin</span></span>
* <span data-ttu-id="ac903-129">Leitor global</span><span class="sxs-lookup"><span data-stu-id="ac903-129">Global reader</span></span>
* <span data-ttu-id="ac903-130">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="ac903-130">Privileged authentication admin</span></span>
* <span data-ttu-id="ac903-131">Administrador de autenticação (vê apenas números de telefone com máscara)</span><span class="sxs-lookup"><span data-stu-id="ac903-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="ac903-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac903-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/passwordMethods/{id}
GET /users/{id | userPrincipalName}/authentication/passwordMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ac903-133">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ac903-133">Optional query parameters</span></span>

<span data-ttu-id="ac903-134">Esse método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ac903-134">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ac903-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac903-135">Request headers</span></span>

| <span data-ttu-id="ac903-136">Nome</span><span class="sxs-lookup"><span data-stu-id="ac903-136">Name</span></span>      |<span data-ttu-id="ac903-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac903-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ac903-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac903-138">Authorization</span></span> | <span data-ttu-id="ac903-139">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="ac903-139">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac903-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac903-140">Request body</span></span>

<span data-ttu-id="ac903-141">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ac903-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac903-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac903-142">Response</span></span>

<span data-ttu-id="ac903-143">Se bem-sucedido, este método retorna um código de resposta e o objeto `200 OK` [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac903-143">If successful, this method returns a `200 OK` response code and the requested [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ac903-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ac903-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ac903-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac903-145">Request</span></span>

<span data-ttu-id="ac903-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac903-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ac903-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac903-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordauthenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/passwordMethods/{id}
```
# <a name="c"></a>[<span data-ttu-id="ac903-148">C#</span><span class="sxs-lookup"><span data-stu-id="ac903-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac903-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac903-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac903-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac903-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ac903-151">Java</span><span class="sxs-lookup"><span data-stu-id="ac903-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-passwordauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ac903-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac903-152">Response</span></span>

<span data-ttu-id="ac903-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ac903-153">The following is an example of the response.</span></span>

> <span data-ttu-id="ac903-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ac903-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordAuthenticationMethod"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "28c10230-6103-485e-b985-444c60001490",
  "password": null,
  "creationDateTime": null
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get passwordAuthenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
