---
title: Obter phoneAuthenticationMethod
description: Recupere um único objeto phoneAuthenticationMethod.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 4aea872d99deedb3fbf952954e2d6ff691994220
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957284"
---
# <a name="get-phoneauthenticationmethod"></a><span data-ttu-id="64da1-103">Obter phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="64da1-103">Get phoneAuthenticationMethod</span></span>

<span data-ttu-id="64da1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64da1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64da1-105">Recupere um único [objeto phoneAuthenticationMethod.](../resources/phoneauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="64da1-105">Retrieve a single [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="64da1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="64da1-106">Permissions</span></span>

<span data-ttu-id="64da1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64da1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="64da1-109">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="64da1-109">Permissions acting on self</span></span>

|<span data-ttu-id="64da1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64da1-110">Permission type</span></span>      | <span data-ttu-id="64da1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64da1-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="64da1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64da1-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="64da1-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64da1-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="64da1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64da1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64da1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64da1-115">Not supported.</span></span> |
| <span data-ttu-id="64da1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64da1-116">Application</span></span>                            | <span data-ttu-id="64da1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64da1-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="64da1-118">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="64da1-118">Permissions acting on other users</span></span>

|<span data-ttu-id="64da1-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64da1-119">Permission type</span></span>      | <span data-ttu-id="64da1-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64da1-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="64da1-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64da1-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="64da1-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64da1-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="64da1-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64da1-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64da1-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64da1-124">Not supported.</span></span> |
| <span data-ttu-id="64da1-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64da1-125">Application</span></span>                            | <span data-ttu-id="64da1-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64da1-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="64da1-127">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="64da1-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="64da1-128">Administrador global</span><span class="sxs-lookup"><span data-stu-id="64da1-128">Global admin</span></span>
* <span data-ttu-id="64da1-129">Leitor global</span><span class="sxs-lookup"><span data-stu-id="64da1-129">Global reader</span></span>
* <span data-ttu-id="64da1-130">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="64da1-130">Privileged authentication admin</span></span>
* <span data-ttu-id="64da1-131">Administrador de autenticação (apenas vê números de telefone mascarados)</span><span class="sxs-lookup"><span data-stu-id="64da1-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="64da1-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64da1-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/phoneMethods/{id}
GET /users/{id | userPrincipalName}/authentication/phoneMethods/{id}
```
<span data-ttu-id="64da1-133">O valor correspondente ao phoneType a ser `id` recuperado é um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="64da1-133">The value of `id` corresponding to the phoneType to retrieve is one of the following:</span></span>
+ <span data-ttu-id="64da1-134">`b6332ec1-7057-4abe-9331-3d72feddfe41` para recuperar `alternateMobile` **o phoneType**.</span><span class="sxs-lookup"><span data-stu-id="64da1-134">`b6332ec1-7057-4abe-9331-3d72feddfe41` to retrieve the `alternateMobile` **phoneType**.</span></span>
+ <span data-ttu-id="64da1-135">`e37fc753-ff3b-4958-9484-eaa9425c82bc` para recuperar `office` **o phoneType**.</span><span class="sxs-lookup"><span data-stu-id="64da1-135">`e37fc753-ff3b-4958-9484-eaa9425c82bc` to retrieve the `office` **phoneType**.</span></span>
+ <span data-ttu-id="64da1-136">`3179e48a-750b-4051-897c-87b9720928f7` para recuperar `mobile` **o phoneType**.</span><span class="sxs-lookup"><span data-stu-id="64da1-136">`3179e48a-750b-4051-897c-87b9720928f7` to retrieve the `mobile` **phoneType**.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="64da1-137">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="64da1-137">Optional query parameters</span></span>

<span data-ttu-id="64da1-138">Este método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="64da1-138">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="64da1-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64da1-139">Request headers</span></span>

| <span data-ttu-id="64da1-140">Nome</span><span class="sxs-lookup"><span data-stu-id="64da1-140">Name</span></span>      |<span data-ttu-id="64da1-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="64da1-141">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="64da1-142">Autorização</span><span class="sxs-lookup"><span data-stu-id="64da1-142">Authorization</span></span> | <span data-ttu-id="64da1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64da1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64da1-145">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64da1-145">Request body</span></span>

<span data-ttu-id="64da1-146">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="64da1-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64da1-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="64da1-147">Response</span></span>

<span data-ttu-id="64da1-148">Se tiver êxito, este método retornará um código de resposta e `200 OK` o objeto [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64da1-148">If successful, this method returns a `200 OK` response code and the requested [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="64da1-149">Exemplos</span><span class="sxs-lookup"><span data-stu-id="64da1-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="64da1-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64da1-150">Request</span></span>

<span data-ttu-id="64da1-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="64da1-151">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="64da1-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="64da1-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_phoneauthenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
```
# <a name="c"></a>[<span data-ttu-id="64da1-153">C#</span><span class="sxs-lookup"><span data-stu-id="64da1-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-phoneauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64da1-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64da1-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-phoneauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64da1-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64da1-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-phoneauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64da1-156">Java</span><span class="sxs-lookup"><span data-stu-id="64da1-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-phoneauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="64da1-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="64da1-157">Response</span></span>

<span data-ttu-id="64da1-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="64da1-158">The following is an example of the response.</span></span>

> <span data-ttu-id="64da1-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64da1-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
