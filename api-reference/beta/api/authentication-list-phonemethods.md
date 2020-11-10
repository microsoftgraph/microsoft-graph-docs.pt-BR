---
title: Listar phoneMethods
description: Recupere uma lista de objetos de método de autenticação de telefone.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b8cb8adb91d2d213f54d2854c85cd77b998d04ea
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961432"
---
# <a name="list-phonemethods"></a><span data-ttu-id="1043d-103">Listar phoneMethods</span><span class="sxs-lookup"><span data-stu-id="1043d-103">List phoneMethods</span></span>

<span data-ttu-id="1043d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1043d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1043d-105">Recupere uma lista de objetos de [método de autenticação de telefone](../resources/phoneauthenticationmethod.md) .</span><span class="sxs-lookup"><span data-stu-id="1043d-105">Retrieve a list of [phone authentication method](../resources/phoneauthenticationmethod.md) objects.</span></span> <span data-ttu-id="1043d-106">Isso retornará até três objetos, uma vez que um usuário pode ter até três telefones utilizáveis para autenticação.</span><span class="sxs-lookup"><span data-stu-id="1043d-106">This will return up to three objects, as a user can have up to three phones usable for authentication.</span></span>

## <a name="permissions"></a><span data-ttu-id="1043d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="1043d-107">Permissions</span></span>

<span data-ttu-id="1043d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1043d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1043d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1043d-110">Permission type</span></span>                        | <span data-ttu-id="1043d-111">Permissões que atuam em si (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1043d-111">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="1043d-112">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1043d-112">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="1043d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1043d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1043d-114">UserAuthenticationMethod. Read, UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1043d-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="1043d-115">UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1043d-115">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="1043d-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1043d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1043d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1043d-117">Not supported.</span></span> | <span data-ttu-id="1043d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1043d-118">Not supported.</span></span> |
| <span data-ttu-id="1043d-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1043d-119">Application</span></span>                            | <span data-ttu-id="1043d-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1043d-120">Not supported.</span></span> | <span data-ttu-id="1043d-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1043d-121">Not supported.</span></span> |

<span data-ttu-id="1043d-122">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="1043d-122">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="1043d-123">Administrador global</span><span class="sxs-lookup"><span data-stu-id="1043d-123">Global admin</span></span>
* <span data-ttu-id="1043d-124">Leitor global</span><span class="sxs-lookup"><span data-stu-id="1043d-124">Global reader</span></span>
* <span data-ttu-id="1043d-125">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="1043d-125">Privileged authentication admin</span></span>
* <span data-ttu-id="1043d-126">Administrador de autenticação (apenas Ver os números de telefone mascarados)</span><span class="sxs-lookup"><span data-stu-id="1043d-126">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="1043d-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1043d-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/phoneMethods
GET /users/{id | userPrincipalName}/authentication/phoneMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1043d-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1043d-128">Optional query parameters</span></span>

<span data-ttu-id="1043d-129">Este método não oferece suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1043d-129">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1043d-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1043d-130">Request headers</span></span>

| <span data-ttu-id="1043d-131">Nome</span><span class="sxs-lookup"><span data-stu-id="1043d-131">Name</span></span>      |<span data-ttu-id="1043d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1043d-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1043d-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="1043d-133">Authorization</span></span> | <span data-ttu-id="1043d-134">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="1043d-134">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1043d-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1043d-135">Request body</span></span>

<span data-ttu-id="1043d-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1043d-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1043d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1043d-137">Response</span></span>

<span data-ttu-id="1043d-138">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1043d-138">If successful, this method returns a `200 OK` response code and a collection of [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1043d-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1043d-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1043d-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1043d-140">Request</span></span>

<span data-ttu-id="1043d-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1043d-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1043d-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="1043d-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_phonemethods"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/phoneMethods
```
# <a name="c"></a>[<span data-ttu-id="1043d-143">C#</span><span class="sxs-lookup"><span data-stu-id="1043d-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-phonemethods-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1043d-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1043d-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-phonemethods-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1043d-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1043d-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-phonemethods-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1043d-146">Java</span><span class="sxs-lookup"><span data-stu-id="1043d-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-phonemethods-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1043d-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="1043d-147">Response</span></span>

<span data-ttu-id="1043d-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1043d-148">The following is an example of the response.</span></span>

> <span data-ttu-id="1043d-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1043d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "phoneNumber": "+1 2065555555",
      "phoneType": "mobile",
      "smsSignInState": "ready",
      "id": "3179e48a-750b-4051-897c-87b9720928f7"
    },
    {
      "phoneNumber": "+1 2065555556",
      "phoneType": "alternateMobile",
      "smsSignInState": "notSupported",
      "id": "b6332ec1-7057-4abe-9331-3d72feddfe41"
    },
    {
      "phoneNumber": "+1 2065555557",
      "phoneType": "office",
      "smsSignInState": "notSupported",
      "id": "e37fc753-ff3b-4958-9484-eaa9425c82bc"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List phoneMethods",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
