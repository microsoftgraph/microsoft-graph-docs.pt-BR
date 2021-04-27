---
title: Obter phoneAuthenticationMethod
description: Recupere um único objeto phoneAuthenticationMethod.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d3f4f9a94025710508d07fdc0b4b2dd85ae74e11
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050035"
---
# <a name="get-phoneauthenticationmethod"></a><span data-ttu-id="f1dbc-103">Obter phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f1dbc-103">Get phoneAuthenticationMethod</span></span>

<span data-ttu-id="f1dbc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1dbc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1dbc-105">Recupere um único [objeto phoneAuthenticationMethod.](../resources/phoneauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="f1dbc-105">Retrieve a single [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object.</span></span> <span data-ttu-id="f1dbc-106">Esse método está disponível apenas para usuários padrão do Azure AD e B2B, mas não para usuários B2C.</span><span class="sxs-lookup"><span data-stu-id="f1dbc-106">This method is available only for standard Azure AD and B2B users, but not B2C users.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1dbc-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1dbc-107">Permissions</span></span>

<span data-ttu-id="f1dbc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1dbc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="f1dbc-110">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="f1dbc-110">Permissions acting on self</span></span>

|<span data-ttu-id="f1dbc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1dbc-111">Permission type</span></span>      | <span data-ttu-id="f1dbc-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1dbc-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="f1dbc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1dbc-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f1dbc-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1dbc-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="f1dbc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1dbc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1dbc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1dbc-116">Not supported.</span></span> |
| <span data-ttu-id="f1dbc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1dbc-117">Application</span></span>                            | <span data-ttu-id="f1dbc-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1dbc-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="f1dbc-119">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="f1dbc-119">Permissions acting on other users</span></span>

|<span data-ttu-id="f1dbc-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1dbc-120">Permission type</span></span>      | <span data-ttu-id="f1dbc-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1dbc-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="f1dbc-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1dbc-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="f1dbc-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1dbc-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="f1dbc-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1dbc-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1dbc-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1dbc-125">Not supported.</span></span> |
| <span data-ttu-id="f1dbc-126">Application</span><span class="sxs-lookup"><span data-stu-id="f1dbc-126">Application</span></span>                            | <span data-ttu-id="f1dbc-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1dbc-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="f1dbc-128">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="f1dbc-128">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="f1dbc-129">Administração global</span><span class="sxs-lookup"><span data-stu-id="f1dbc-129">Global admin</span></span>
* <span data-ttu-id="f1dbc-130">Leitor global</span><span class="sxs-lookup"><span data-stu-id="f1dbc-130">Global reader</span></span>
* <span data-ttu-id="f1dbc-131">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="f1dbc-131">Privileged authentication admin</span></span>
* <span data-ttu-id="f1dbc-132">Administrador de autenticação (apenas vê números de telefone mascarados)</span><span class="sxs-lookup"><span data-stu-id="f1dbc-132">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="f1dbc-133">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1dbc-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/phoneMethods/{id}
GET /users/{id | userPrincipalName}/authentication/phoneMethods/{id}
```
<span data-ttu-id="f1dbc-134">O valor correspondente ao phoneType a ser `id` recuperado é um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="f1dbc-134">The value of `id` corresponding to the phoneType to retrieve is one of the following:</span></span>
+ <span data-ttu-id="f1dbc-135">`b6332ec1-7057-4abe-9331-3d72feddfe41` para recuperar `alternateMobile` **o phoneType**.</span><span class="sxs-lookup"><span data-stu-id="f1dbc-135">`b6332ec1-7057-4abe-9331-3d72feddfe41` to retrieve the `alternateMobile` **phoneType**.</span></span>
+ <span data-ttu-id="f1dbc-136">`e37fc753-ff3b-4958-9484-eaa9425c82bc` para recuperar `office` **o phoneType**.</span><span class="sxs-lookup"><span data-stu-id="f1dbc-136">`e37fc753-ff3b-4958-9484-eaa9425c82bc` to retrieve the `office` **phoneType**.</span></span>
+ <span data-ttu-id="f1dbc-137">`3179e48a-750b-4051-897c-87b9720928f7` para recuperar `mobile` **o phoneType**.</span><span class="sxs-lookup"><span data-stu-id="f1dbc-137">`3179e48a-750b-4051-897c-87b9720928f7` to retrieve the `mobile` **phoneType**.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="f1dbc-138">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f1dbc-138">Optional query parameters</span></span>

<span data-ttu-id="f1dbc-139">Este método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f1dbc-139">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f1dbc-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1dbc-140">Request headers</span></span>

| <span data-ttu-id="f1dbc-141">Nome</span><span class="sxs-lookup"><span data-stu-id="f1dbc-141">Name</span></span>      |<span data-ttu-id="f1dbc-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1dbc-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f1dbc-143">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1dbc-143">Authorization</span></span> | <span data-ttu-id="f1dbc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1dbc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f1dbc-146">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1dbc-146">Request body</span></span>

<span data-ttu-id="f1dbc-147">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f1dbc-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1dbc-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1dbc-148">Response</span></span>

<span data-ttu-id="f1dbc-149">Se tiver êxito, este método retornará um código de resposta e `200 OK` o objeto [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1dbc-149">If successful, this method returns a `200 OK` response code and the requested [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f1dbc-150">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f1dbc-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f1dbc-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1dbc-151">Request</span></span>

<span data-ttu-id="f1dbc-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1dbc-152">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f1dbc-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1dbc-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_phoneauthenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
```
# <a name="c"></a>[<span data-ttu-id="f1dbc-154">C#</span><span class="sxs-lookup"><span data-stu-id="f1dbc-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-phoneauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1dbc-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1dbc-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-phoneauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f1dbc-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f1dbc-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-phoneauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f1dbc-157">Java</span><span class="sxs-lookup"><span data-stu-id="f1dbc-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-phoneauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f1dbc-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1dbc-158">Response</span></span>

<span data-ttu-id="f1dbc-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f1dbc-159">The following is an example of the response.</span></span>

> <span data-ttu-id="f1dbc-160">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f1dbc-160">**Note:** The response object shown here might be shortened for readability.</span></span>

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
