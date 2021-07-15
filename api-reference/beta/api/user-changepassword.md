---
title: 'user: changePassword'
description: Atualize sua senha.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 7787ad62106cd5404bb0d5075d3d48d0ec1d6371
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442813"
---
# <a name="user-changepassword"></a><span data-ttu-id="04d74-103">user: changePassword</span><span class="sxs-lookup"><span data-stu-id="04d74-103">user: changePassword</span></span>

<span data-ttu-id="04d74-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04d74-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04d74-105">Habilita o usuário a atualizar sua senha.</span><span class="sxs-lookup"><span data-stu-id="04d74-105">Enable the user to update their password.</span></span> <span data-ttu-id="04d74-106">Qualquer usuário pode atualizar sua senha sem pertencer a qualquer função de administrador.</span><span class="sxs-lookup"><span data-stu-id="04d74-106">Any user can update their password without belonging to any administrator role.</span></span>

## <a name="permissions"></a><span data-ttu-id="04d74-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="04d74-107">Permissions</span></span>
<span data-ttu-id="04d74-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04d74-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="04d74-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04d74-110">Permission type</span></span>      | <span data-ttu-id="04d74-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="04d74-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04d74-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04d74-112">Delegated (work or school account)</span></span> | <span data-ttu-id="04d74-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="04d74-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="04d74-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04d74-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04d74-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04d74-115">Not supported.</span></span>    |
|<span data-ttu-id="04d74-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04d74-116">Application</span></span> | <span data-ttu-id="04d74-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04d74-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="04d74-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04d74-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/changePassword
```
## <a name="request-headers"></a><span data-ttu-id="04d74-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04d74-119">Request headers</span></span>
| <span data-ttu-id="04d74-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="04d74-120">Header</span></span>       | <span data-ttu-id="04d74-121">Valor</span><span class="sxs-lookup"><span data-stu-id="04d74-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="04d74-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="04d74-122">Authorization</span></span>  | <span data-ttu-id="04d74-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04d74-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="04d74-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="04d74-125">Content-type</span></span>  | <span data-ttu-id="04d74-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04d74-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="04d74-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04d74-128">Request body</span></span>
<span data-ttu-id="04d74-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="04d74-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="04d74-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="04d74-130">Parameter</span></span>    | <span data-ttu-id="04d74-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="04d74-131">Type</span></span>   |<span data-ttu-id="04d74-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="04d74-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="04d74-133">currentPassword</span><span class="sxs-lookup"><span data-stu-id="04d74-133">currentPassword</span></span> | <span data-ttu-id="04d74-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="04d74-134">String</span></span> | <span data-ttu-id="04d74-135">Sua senha atual.</span><span class="sxs-lookup"><span data-stu-id="04d74-135">Your current password.</span></span>|
| <span data-ttu-id="04d74-136">newPassword</span><span class="sxs-lookup"><span data-stu-id="04d74-136">newPassword</span></span> | <span data-ttu-id="04d74-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="04d74-137">String</span></span> | <span data-ttu-id="04d74-138">Sua nova senha.</span><span class="sxs-lookup"><span data-stu-id="04d74-138">Your new password.</span></span>|

## <a name="response"></a><span data-ttu-id="04d74-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="04d74-139">Response</span></span>

<span data-ttu-id="04d74-140">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="04d74-140">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="04d74-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04d74-141">Example</span></span>
<span data-ttu-id="04d74-142">O exemplo a seguir mostra uma solicitação para atualizar sua própria senha.</span><span class="sxs-lookup"><span data-stu-id="04d74-142">The following example shows a request to update your own password.</span></span>

### <a name="request"></a><span data-ttu-id="04d74-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04d74-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="04d74-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="04d74-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_changepassword"
}-->
```http
POST https://graph.microsoft.com/beta/me/changePassword
Content-type: application/json

{
    "currentPassword": "xWwvJ]6NMw+bWH-d",
    "newPassword": "0eM85N54wFxWwvJ]"
}
```
# <a name="c"></a>[<span data-ttu-id="04d74-145">C#</span><span class="sxs-lookup"><span data-stu-id="04d74-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-changepassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="04d74-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04d74-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-changepassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="04d74-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="04d74-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-changepassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="04d74-148">Java</span><span class="sxs-lookup"><span data-stu-id="04d74-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-changepassword-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="04d74-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="04d74-149">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="04d74-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="04d74-150">See also</span></span>
+ [<span data-ttu-id="04d74-151">Atualizar o passwordProfile de um usuário para redefinir sua senha</span><span class="sxs-lookup"><span data-stu-id="04d74-151">Update the passwordProfile of a user to reset their password</span></span>](../api/user-update.md#example-3-update-the-passwordprofile-of-a-user-to-reset-their-password)

<!-- uuid: a7c9a0de-8324-4f80-8d88-2e6d5838f3be
2021-06-24 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: changePassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


