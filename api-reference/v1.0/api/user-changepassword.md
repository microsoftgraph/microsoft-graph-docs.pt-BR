---
title: 'user: changePassword'
description: Atualize sua senha.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 2adf91adb5eab959dc981f0532c4017e838852ab
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441692"
---
# <a name="user-changepassword"></a><span data-ttu-id="4e0a8-103">user: changePassword</span><span class="sxs-lookup"><span data-stu-id="4e0a8-103">user: changePassword</span></span>

<span data-ttu-id="4e0a8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e0a8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4e0a8-105">Habilita o usuário a atualizar sua senha.</span><span class="sxs-lookup"><span data-stu-id="4e0a8-105">Enable the user to update their password.</span></span> <span data-ttu-id="4e0a8-106">Qualquer usuário pode atualizar sua senha sem pertencer a qualquer função de administrador.</span><span class="sxs-lookup"><span data-stu-id="4e0a8-106">Any user can update their password without belonging to any administrator role.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e0a8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="4e0a8-107">Permissions</span></span>
<span data-ttu-id="4e0a8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e0a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4e0a8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e0a8-110">Permission type</span></span>      | <span data-ttu-id="4e0a8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4e0a8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e0a8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e0a8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4e0a8-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4e0a8-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4e0a8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e0a8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e0a8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e0a8-115">Not supported.</span></span>    |
|<span data-ttu-id="4e0a8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4e0a8-116">Application</span></span> | <span data-ttu-id="4e0a8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e0a8-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e0a8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e0a8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/changePassword
```
## <a name="request-headers"></a><span data-ttu-id="4e0a8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4e0a8-119">Request headers</span></span>
| <span data-ttu-id="4e0a8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4e0a8-120">Header</span></span>       | <span data-ttu-id="4e0a8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4e0a8-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4e0a8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4e0a8-122">Authorization</span></span>  | <span data-ttu-id="4e0a8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4e0a8-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4e0a8-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="4e0a8-125">Content-type</span></span>  | <span data-ttu-id="4e0a8-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4e0a8-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4e0a8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e0a8-128">Request body</span></span>
<span data-ttu-id="4e0a8-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e0a8-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4e0a8-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4e0a8-130">Parameter</span></span>    | <span data-ttu-id="4e0a8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e0a8-131">Type</span></span>   |<span data-ttu-id="4e0a8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e0a8-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4e0a8-133">currentPassword</span><span class="sxs-lookup"><span data-stu-id="4e0a8-133">currentPassword</span></span> | <span data-ttu-id="4e0a8-134">String</span><span class="sxs-lookup"><span data-stu-id="4e0a8-134">String</span></span> | <span data-ttu-id="4e0a8-135">Sua senha atual.</span><span class="sxs-lookup"><span data-stu-id="4e0a8-135">Your current password.</span></span>|
| <span data-ttu-id="4e0a8-136">newPassword</span><span class="sxs-lookup"><span data-stu-id="4e0a8-136">newPassword</span></span> | <span data-ttu-id="4e0a8-137">String</span><span class="sxs-lookup"><span data-stu-id="4e0a8-137">String</span></span> | <span data-ttu-id="4e0a8-138">Sua nova senha.</span><span class="sxs-lookup"><span data-stu-id="4e0a8-138">Your new password.</span></span>|

## <a name="response"></a><span data-ttu-id="4e0a8-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e0a8-139">Response</span></span>

<span data-ttu-id="4e0a8-140">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4e0a8-140">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4e0a8-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4e0a8-141">Example</span></span>
<span data-ttu-id="4e0a8-142">O exemplo a seguir mostra uma solicitação para atualizar sua própria senha.</span><span class="sxs-lookup"><span data-stu-id="4e0a8-142">The following example shows a request to update your own password.</span></span>

### <a name="request"></a><span data-ttu-id="4e0a8-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e0a8-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4e0a8-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e0a8-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_changepassword"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/changePassword
Content-type: application/json

{
    "currentPassword": "xWwvJ]6NMw+bWH-d",
    "newPassword": "0eM85N54wFxWwvJ]"
}
```
# <a name="c"></a>[<span data-ttu-id="4e0a8-145">C#</span><span class="sxs-lookup"><span data-stu-id="4e0a8-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-changepassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e0a8-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e0a8-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-changepassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e0a8-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e0a8-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-changepassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4e0a8-148">Java</span><span class="sxs-lookup"><span data-stu-id="4e0a8-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-changepassword-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="4e0a8-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e0a8-149">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="4e0a8-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="4e0a8-150">See also</span></span>
+ [<span data-ttu-id="4e0a8-151">Atualizar o passwordProfile de um usuário para redefinir sua senha</span><span class="sxs-lookup"><span data-stu-id="4e0a8-151">Update the passwordProfile of a user to reset their password</span></span>](../api/user-update.md#example-3-update-the-passwordprofile-of-a-user-to-reset-their-password)

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


