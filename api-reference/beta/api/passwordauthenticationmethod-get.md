---
title: Obter passwordAuthenticationMethod
description: Recupere as propriedades e os relacionamentos do objeto passwordauthenticationmethod.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 93ac85f59cf82fffeb50ffa56c67324d4eae4f05
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48417916"
---
# <a name="get-passwordauthenticationmethod"></a><span data-ttu-id="cb912-103">Obter passwordAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="cb912-103">Get passwordAuthenticationMethod</span></span>

<span data-ttu-id="cb912-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb912-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb912-105">Recupere as propriedades e os relacionamentos de um objeto de [método de autenticação de senha](../resources/passwordauthenticationmethod.md) .</span><span class="sxs-lookup"><span data-stu-id="cb912-105">Retrieve the properties and relationships of a [password authentication method](../resources/passwordauthenticationmethod.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="cb912-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cb912-106">Permissions</span></span>

<span data-ttu-id="cb912-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb912-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cb912-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb912-109">Permission type</span></span>                        | <span data-ttu-id="cb912-110">Permissões que atuam em si (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cb912-110">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="cb912-111">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cb912-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="cb912-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb912-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb912-113">UserAuthenticationMethod. Read, UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="cb912-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="cb912-114">UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="cb912-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="cb912-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb912-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb912-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb912-116">Not supported.</span></span> | <span data-ttu-id="cb912-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb912-117">Not supported.</span></span> |
| <span data-ttu-id="cb912-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cb912-118">Application</span></span>                            | <span data-ttu-id="cb912-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb912-119">Not supported.</span></span> | <span data-ttu-id="cb912-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb912-120">Not supported.</span></span> |

<span data-ttu-id="cb912-121">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="cb912-121">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="cb912-122">Administrador global</span><span class="sxs-lookup"><span data-stu-id="cb912-122">Global admin</span></span>
* <span data-ttu-id="cb912-123">Leitor global</span><span class="sxs-lookup"><span data-stu-id="cb912-123">Global reader</span></span>
* <span data-ttu-id="cb912-124">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="cb912-124">Privileged authentication admin</span></span>
* <span data-ttu-id="cb912-125">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="cb912-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="cb912-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb912-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/passwordMethods/{id}
GET /users/{id | userPrincipalName}/authentication/passwordMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cb912-127">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cb912-127">Optional query parameters</span></span>

<span data-ttu-id="cb912-128">Este método não oferece suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cb912-128">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cb912-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb912-129">Request headers</span></span>

| <span data-ttu-id="cb912-130">Nome</span><span class="sxs-lookup"><span data-stu-id="cb912-130">Name</span></span>      |<span data-ttu-id="cb912-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb912-131">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cb912-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb912-132">Authorization</span></span> | <span data-ttu-id="cb912-133">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="cb912-133">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb912-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb912-134">Request body</span></span>

<span data-ttu-id="cb912-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cb912-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb912-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb912-136">Response</span></span>

<span data-ttu-id="cb912-137">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb912-137">If successful, this method returns a `200 OK` response code and the requested [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cb912-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cb912-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cb912-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb912-139">Request</span></span>

<span data-ttu-id="cb912-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb912-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cb912-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="cb912-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordauthenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/passwordMethods/{id}
```
# <a name="c"></a>[<span data-ttu-id="cb912-142">C#</span><span class="sxs-lookup"><span data-stu-id="cb912-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cb912-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cb912-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cb912-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cb912-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cb912-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb912-145">Response</span></span>

<span data-ttu-id="cb912-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cb912-146">The following is an example of the response.</span></span>

> <span data-ttu-id="cb912-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cb912-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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