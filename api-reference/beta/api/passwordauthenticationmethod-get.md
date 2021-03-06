---
title: Obter passwordAuthenticationMethod
description: Recupere as propriedades e as relações do objeto passwordauthenticationmethod.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2112788ce5127326e0e82ef91c1068b5b56ec14a
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515588"
---
# <a name="get-passwordauthenticationmethod"></a><span data-ttu-id="c091e-103">Obter passwordAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c091e-103">Get passwordAuthenticationMethod</span></span>

<span data-ttu-id="c091e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c091e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c091e-105">Recupere as propriedades e as relações de um objeto de método [de autenticação de](../resources/passwordauthenticationmethod.md) senha.</span><span class="sxs-lookup"><span data-stu-id="c091e-105">Retrieve the properties and relationships of a [password authentication method](../resources/passwordauthenticationmethod.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="c091e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c091e-106">Permissions</span></span>

<span data-ttu-id="c091e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c091e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="c091e-109">Permissões agindo em si mesmo</span><span class="sxs-lookup"><span data-stu-id="c091e-109">Permissions acting on self</span></span>

|<span data-ttu-id="c091e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c091e-110">Permission type</span></span>      | <span data-ttu-id="c091e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c091e-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="c091e-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c091e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c091e-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c091e-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="c091e-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c091e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c091e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c091e-115">Not supported.</span></span> |
| <span data-ttu-id="c091e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c091e-116">Application</span></span>                            | <span data-ttu-id="c091e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c091e-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="c091e-118">Permissões atuando em outros usuários</span><span class="sxs-lookup"><span data-stu-id="c091e-118">Permissions acting on other users</span></span>

|<span data-ttu-id="c091e-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c091e-119">Permission type</span></span>      | <span data-ttu-id="c091e-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c091e-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="c091e-121">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c091e-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="c091e-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c091e-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="c091e-123">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c091e-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c091e-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c091e-124">Not supported.</span></span> |
| <span data-ttu-id="c091e-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c091e-125">Application</span></span>                            | <span data-ttu-id="c091e-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c091e-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="c091e-127">Para cenários delegados em que um administrador está atuando em outro usuário, o administrador precisa de uma [das seguintes funções:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="c091e-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="c091e-128">Administrador global</span><span class="sxs-lookup"><span data-stu-id="c091e-128">Global admin</span></span>
* <span data-ttu-id="c091e-129">Leitor global</span><span class="sxs-lookup"><span data-stu-id="c091e-129">Global reader</span></span>
* <span data-ttu-id="c091e-130">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="c091e-130">Privileged authentication admin</span></span>
* <span data-ttu-id="c091e-131">Administrador de autenticação (apenas vê números de telefone mascarados)</span><span class="sxs-lookup"><span data-stu-id="c091e-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="c091e-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c091e-132">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/passwordMethods/{id}
GET /users/{id | userPrincipalName}/authentication/passwordMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c091e-133">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c091e-133">Optional query parameters</span></span>

<span data-ttu-id="c091e-134">Este método não dá suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c091e-134">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c091e-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c091e-135">Request headers</span></span>

| <span data-ttu-id="c091e-136">Nome</span><span class="sxs-lookup"><span data-stu-id="c091e-136">Name</span></span>      |<span data-ttu-id="c091e-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="c091e-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c091e-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="c091e-138">Authorization</span></span> | <span data-ttu-id="c091e-139">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="c091e-139">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c091e-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c091e-140">Request body</span></span>

<span data-ttu-id="c091e-141">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c091e-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c091e-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="c091e-142">Response</span></span>

<span data-ttu-id="c091e-143">Se tiver êxito, este método retornará um código de resposta e `200 OK` o objeto [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c091e-143">If successful, this method returns a `200 OK` response code and the requested [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c091e-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c091e-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c091e-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c091e-145">Request</span></span>

<span data-ttu-id="c091e-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c091e-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c091e-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="c091e-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordauthenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/passwordMethods/{id}
```
# <a name="c"></a>[<span data-ttu-id="c091e-148">C#</span><span class="sxs-lookup"><span data-stu-id="c091e-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c091e-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c091e-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c091e-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c091e-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c091e-151">Java</span><span class="sxs-lookup"><span data-stu-id="c091e-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-passwordauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c091e-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="c091e-152">Response</span></span>

<span data-ttu-id="c091e-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c091e-153">The following is an example of the response.</span></span>

> <span data-ttu-id="c091e-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c091e-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
