---
title: Listar phoneMethods
description: Recupere uma lista de objetos de método de autenticação de telefone.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e02337150622f3868a6f4008766781f8800862ee
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805824"
---
# <a name="list-phonemethods"></a><span data-ttu-id="790a3-103">Listar phoneMethods</span><span class="sxs-lookup"><span data-stu-id="790a3-103">List phoneMethods</span></span>

<span data-ttu-id="790a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="790a3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="790a3-105">Recupere uma lista de objetos de [método de autenticação de telefone](../resources/phoneauthenticationmethod.md) .</span><span class="sxs-lookup"><span data-stu-id="790a3-105">Retrieve a list of [phone authentication method](../resources/phoneauthenticationmethod.md) objects.</span></span> <span data-ttu-id="790a3-106">Isso retornará até três objetos, uma vez que um usuário pode ter até três telefones utilizáveis para autenticação.</span><span class="sxs-lookup"><span data-stu-id="790a3-106">This will return up to three objects, as a user can have up to three phones usable for authentication.</span></span>

## <a name="permissions"></a><span data-ttu-id="790a3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="790a3-107">Permissions</span></span>

<span data-ttu-id="790a3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="790a3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="790a3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="790a3-110">Permission type</span></span>                        | <span data-ttu-id="790a3-111">Permissões que atuam em si (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="790a3-111">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="790a3-112">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="790a3-112">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="790a3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="790a3-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="790a3-114">UserAuthenticationMethod. Read, UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="790a3-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="790a3-115">UserAuthenticationMethod. Read. All, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="790a3-115">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="790a3-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="790a3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="790a3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="790a3-117">Not supported.</span></span> | <span data-ttu-id="790a3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="790a3-118">Not supported.</span></span> |
| <span data-ttu-id="790a3-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="790a3-119">Application</span></span>                            | <span data-ttu-id="790a3-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="790a3-120">Not supported.</span></span> | <span data-ttu-id="790a3-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="790a3-121">Not supported.</span></span> |

<span data-ttu-id="790a3-122">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="790a3-122">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="790a3-123">Administrador global</span><span class="sxs-lookup"><span data-stu-id="790a3-123">Global admin</span></span>
* <span data-ttu-id="790a3-124">Leitor global</span><span class="sxs-lookup"><span data-stu-id="790a3-124">Global reader</span></span>
* <span data-ttu-id="790a3-125">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="790a3-125">Privileged authentication admin</span></span>
* <span data-ttu-id="790a3-126">Administrador de autenticação (apenas Ver os números de telefone mascarados)</span><span class="sxs-lookup"><span data-stu-id="790a3-126">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="790a3-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="790a3-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/phoneMethods
GET /users/{id}/authentication/phoneMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="790a3-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="790a3-128">Optional query parameters</span></span>

<span data-ttu-id="790a3-129">Este método não oferece suporte a parâmetros de consulta opcionais para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="790a3-129">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="790a3-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="790a3-130">Request headers</span></span>

| <span data-ttu-id="790a3-131">Nome</span><span class="sxs-lookup"><span data-stu-id="790a3-131">Name</span></span>      |<span data-ttu-id="790a3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="790a3-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="790a3-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="790a3-133">Authorization</span></span> | <span data-ttu-id="790a3-134">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="790a3-134">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="790a3-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="790a3-135">Request body</span></span>

<span data-ttu-id="790a3-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="790a3-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="790a3-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="790a3-137">Response</span></span>

<span data-ttu-id="790a3-138">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="790a3-138">If successful, this method returns a `200 OK` response code and a collection of [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="790a3-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="790a3-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="790a3-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="790a3-140">Request</span></span>

<span data-ttu-id="790a3-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="790a3-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="790a3-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="790a3-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_phonemethods"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/phoneMethods
```
# <a name="c"></a>[<span data-ttu-id="790a3-143">C#</span><span class="sxs-lookup"><span data-stu-id="790a3-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-phonemethods-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="790a3-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="790a3-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-phonemethods-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="790a3-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="790a3-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-phonemethods-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="790a3-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="790a3-146">Response</span></span>

<span data-ttu-id="790a3-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="790a3-147">The following is an example of the response.</span></span>

> <span data-ttu-id="790a3-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="790a3-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
