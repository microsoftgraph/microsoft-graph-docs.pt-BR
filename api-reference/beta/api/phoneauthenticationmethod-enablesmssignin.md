---
title: 'phoneAuthenticationMethod: enableSmsSignIn'
description: Habilite a entrada do SMS para um telefone celular.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d155bf20055bcd7fdd4a7629db5686c8a37103cf
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402657"
---
# <a name="phoneauthenticationmethod-enablesmssignin"></a><span data-ttu-id="5aba5-103">phoneAuthenticationMethod: enableSmsSignIn</span><span class="sxs-lookup"><span data-stu-id="5aba5-103">phoneAuthenticationMethod: enableSmsSignIn</span></span>

<span data-ttu-id="5aba5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5aba5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5aba5-105">Habilite a entrada do SMS para um `mobile` número de telefone existente.</span><span class="sxs-lookup"><span data-stu-id="5aba5-105">Enable SMS sign-in for an existing `mobile` phone number.</span></span> <span data-ttu-id="5aba5-106">Para ser habilitado com êxito:</span><span class="sxs-lookup"><span data-stu-id="5aba5-106">To be successfully enabled:</span></span>

* <span data-ttu-id="5aba5-107">O telefone deve ter `"phoneType": "mobile"` .</span><span class="sxs-lookup"><span data-stu-id="5aba5-107">The phone must have `"phoneType": "mobile"`.</span></span>
* <span data-ttu-id="5aba5-108">O telefone deve ser exclusivo no sistema de entrada do SMS (ninguém mais pode também usar esse número).</span><span class="sxs-lookup"><span data-stu-id="5aba5-108">The phone must be unique in the SMS sign-in system (no one else can also be using that number).</span></span>
* <span data-ttu-id="5aba5-109">O usuário deve estar habilitado para entrada do SMS na política de [métodos de autenticação](/azure/active-directory/authentication/concept-authentication-methods) .</span><span class="sxs-lookup"><span data-stu-id="5aba5-109">The user must be enabled for SMS sign-in in the [authentication methods](/azure/active-directory/authentication/concept-authentication-methods) policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="5aba5-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="5aba5-110">Permissions</span></span>

<span data-ttu-id="5aba5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5aba5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5aba5-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5aba5-113">Permission type</span></span>                        | <span data-ttu-id="5aba5-114">Permissões que atuam em si (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5aba5-114">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="5aba5-115">Permissões que atuam em outros (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5aba5-115">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="5aba5-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5aba5-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="5aba5-117">UserAuthenticationMethod. ReadWrite, UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5aba5-117">UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="5aba5-118">UserAuthenticationMethod. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5aba5-118">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="5aba5-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5aba5-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5aba5-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5aba5-120">Not supported.</span></span> | <span data-ttu-id="5aba5-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5aba5-121">Not supported.</span></span> |
| <span data-ttu-id="5aba5-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5aba5-122">Application</span></span>                            | <span data-ttu-id="5aba5-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5aba5-123">Not supported.</span></span> | <span data-ttu-id="5aba5-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5aba5-124">Not supported.</span></span> |

<span data-ttu-id="5aba5-125">Para cenários delegados em que um administrador está agindo em outro usuário, o administrador precisa [de uma das seguintes funções](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="5aba5-125">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="5aba5-126">Administrador global</span><span class="sxs-lookup"><span data-stu-id="5aba5-126">Global admin</span></span>
* <span data-ttu-id="5aba5-127">Administrador de autenticação privilegiada</span><span class="sxs-lookup"><span data-stu-id="5aba5-127">Privileged authentication admin</span></span>
* <span data-ttu-id="5aba5-128">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="5aba5-128">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="5aba5-129">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5aba5-129">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/authentication/phoneMethods/{id}/enableSmsSignIn
POST /users/{id}/authentication/phoneMethods/{id}/enableSmsSignIn
```

## <a name="request-headers"></a><span data-ttu-id="5aba5-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5aba5-130">Request headers</span></span>

| <span data-ttu-id="5aba5-131">Nome</span><span class="sxs-lookup"><span data-stu-id="5aba5-131">Name</span></span>          | <span data-ttu-id="5aba5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5aba5-132">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5aba5-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="5aba5-133">Authorization</span></span> | <span data-ttu-id="5aba5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5aba5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5aba5-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5aba5-136">Request body</span></span>

<span data-ttu-id="5aba5-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5aba5-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5aba5-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="5aba5-138">Response</span></span>

<span data-ttu-id="5aba5-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5aba5-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5aba5-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5aba5-141">Examples</span></span>

<span data-ttu-id="5aba5-142">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="5aba5-142">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="5aba5-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5aba5-143">Request</span></span>

<span data-ttu-id="5aba5-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5aba5-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5aba5-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="5aba5-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "phoneauthenticationmethod_enablesmssignin"
}-->

```http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7/enableSmsSignIn
```
# <a name="c"></a>[<span data-ttu-id="5aba5-146">C#</span><span class="sxs-lookup"><span data-stu-id="5aba5-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/phoneauthenticationmethod-enablesmssignin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5aba5-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5aba5-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/phoneauthenticationmethod-enablesmssignin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5aba5-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5aba5-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/phoneauthenticationmethod-enablesmssignin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5aba5-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="5aba5-149">Response</span></span>

<span data-ttu-id="5aba5-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5aba5-150">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phoneAuthenticationMethod: enableSmsSignIn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->