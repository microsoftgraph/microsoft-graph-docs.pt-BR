---
title: Métodos de List
description: Recupere uma lista de objetos do método de autenticação.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 48156b4f2c478b5d58978fba837a0f44ed17d502
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515503"
---
# <a name="list-methods"></a><span data-ttu-id="13068-103">Métodos de List</span><span class="sxs-lookup"><span data-stu-id="13068-103">List methods</span></span>

<span data-ttu-id="13068-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13068-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13068-105">Recupere uma lista de objetos [do método de autenticação.](../resources/authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="13068-105">Retrieve a list of [authentication method](../resources/authenticationmethod.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="13068-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="13068-106">Permissions</span></span>

<span data-ttu-id="13068-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13068-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="13068-109">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="13068-109">Permissions acting on self</span></span>

|<span data-ttu-id="13068-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13068-110">Permission type</span></span>      | <span data-ttu-id="13068-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="13068-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="13068-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13068-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="13068-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13068-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="13068-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13068-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13068-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13068-115">Not supported.</span></span> |
| <span data-ttu-id="13068-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13068-116">Application</span></span>                            | <span data-ttu-id="13068-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13068-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="13068-118">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="13068-118">Permissions acting on other users</span></span>

|<span data-ttu-id="13068-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13068-119">Permission type</span></span>      | <span data-ttu-id="13068-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="13068-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="13068-121">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13068-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="13068-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13068-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="13068-123">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13068-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13068-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13068-124">Not supported.</span></span> |
| <span data-ttu-id="13068-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13068-125">Application</span></span>                            | <span data-ttu-id="13068-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13068-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="13068-127">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="13068-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="13068-128">Administrador global</span><span class="sxs-lookup"><span data-stu-id="13068-128">Global admin</span></span>
* <span data-ttu-id="13068-129">Leitor global</span><span class="sxs-lookup"><span data-stu-id="13068-129">Global reader</span></span>
* <span data-ttu-id="13068-130">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="13068-130">Privileged authentication admin</span></span>
* <span data-ttu-id="13068-131">Administrador de autenticação (apenas vê números de telefone mascarados)</span><span class="sxs-lookup"><span data-stu-id="13068-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="13068-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13068-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/methods
GET /users/{id | userPrincipalName}/authentication/methods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="13068-133">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="13068-133">Optional query parameters</span></span>

<span data-ttu-id="13068-134">Este método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="13068-134">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="13068-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13068-135">Request headers</span></span>

| <span data-ttu-id="13068-136">Nome</span><span class="sxs-lookup"><span data-stu-id="13068-136">Name</span></span>      |<span data-ttu-id="13068-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="13068-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="13068-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="13068-138">Authorization</span></span> | <span data-ttu-id="13068-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13068-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13068-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13068-141">Request body</span></span>

<span data-ttu-id="13068-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="13068-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13068-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="13068-143">Response</span></span>

<span data-ttu-id="13068-144">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [authenticationMethod](../resources/authenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13068-144">If successful, this method returns a `200 OK` response code and a collection of [authenticationMethod](../resources/authenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="13068-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="13068-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="13068-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13068-146">Request</span></span>

<span data-ttu-id="13068-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="13068-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="13068-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="13068-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_methods"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/methods
```
# <a name="c"></a>[<span data-ttu-id="13068-149">C#</span><span class="sxs-lookup"><span data-stu-id="13068-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-methods-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="13068-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13068-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-methods-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="13068-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="13068-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-methods-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="13068-152">Java</span><span class="sxs-lookup"><span data-stu-id="13068-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-methods-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="13068-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="13068-153">Response</span></span>

<span data-ttu-id="13068-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="13068-154">The following is an example of the response.</span></span>

> <span data-ttu-id="13068-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13068-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationMethod",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "odata.type": "#microsoft.graph.passwordAuthenticationMethod",
      "id": "28c10230-6103-485e-b985-444c60001490",
      "password": null,
      "creationDateTime": null
    },
    {
      "odata.type": "#microsoft.graph.phoneAuthenticationMethod",
      "id": "3179e48a-750b-4051-897c-87b9720928f7",
      "phoneNumber": "+1 2065555555",
      "authenticationPhoneType": "mobile",
      "smsSignInState": "ready"
    },
    {
      "odata.type": "#microsoft.graph.phoneAuthenticationMethod",
      "id": "b6332ec1-7057-4abe-9331-3d72feddfe41",
      "phoneNumber": "+1 2065555556",
      "authenticationPhoneType": "alternateMobile",
      "smsSignInState": "notSupported"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List methods",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
