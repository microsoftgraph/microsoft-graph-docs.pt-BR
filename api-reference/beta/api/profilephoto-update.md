---
title: Atualizar profilephoto
description: Atualiza a foto de qualquer usuário no locatário, incluindo o usuário conectado ou o grupo ou contato especificado. Desde lá
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: kevinbellinger
ms.openlocfilehash: 67ec3e6400e007e5c0638bea92097e9e4945e85e
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515706"
---
# <a name="update-profilephoto"></a><span data-ttu-id="af396-104">Atualizar profilephoto</span><span class="sxs-lookup"><span data-stu-id="af396-104">Update profilephoto</span></span>

<span data-ttu-id="af396-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af396-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af396-106">Atualize a foto para qualquer usuário no locatário, incluindo o usuário ou o grupo ou contato especificado.</span><span class="sxs-lookup"><span data-stu-id="af396-106">Update the photo for any user in the tenant, including the signed-in user or the specified group or contact.</span></span> <span data-ttu-id="af396-107">Como atualmente há um limite de 8 MB no tamanho total de cada solicitação REST, o tamanho da foto que você pode adicionar é limitado a menos de 8 MB.</span><span class="sxs-lookup"><span data-stu-id="af396-107">Because there is currently a limit of 8MB on the total size of each REST request, the size of the photo you can add is limited to under 8MB.</span></span>

<span data-ttu-id="af396-108">Use SOMENTE PUT para essa operação.</span><span class="sxs-lookup"><span data-stu-id="af396-108">Only use PUT for this operation.</span></span>

> <span data-ttu-id="af396-109">**Observação**: ao atualizar a foto **do usuário,** essa operação tenta primeiro atualizar a foto no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="af396-109">**Note**:  When updating the **user** photo, this operation first attempts to update the photo in Microsoft 365.</span></span> <span data-ttu-id="af396-110">Se isso falhar (devido ao usuário não ter uma caixa de correio), essa API tentará atualizar a foto no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="af396-110">If that fails (due to the user not having a mailbox), this API will attempt to update the photo in Azure Active Directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="af396-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="af396-111">Permissions</span></span>
<span data-ttu-id="af396-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af396-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af396-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af396-114">Permission type</span></span>      | <span data-ttu-id="af396-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="af396-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af396-116">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af396-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="af396-117">Foto de perfil do usuário **de entrada**:</span><span class="sxs-lookup"><span data-stu-id="af396-117">Profile photo of the signed-in **user**:</span></span><br/><span data-ttu-id="af396-118">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af396-118">User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="af396-119">Para recurso de **grupo**:</span><span class="sxs-lookup"><span data-stu-id="af396-119">For **group** resource:</span></span><br /><span data-ttu-id="af396-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af396-120">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="af396-121">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="af396-121">For **contact** resource:</span></span><br /><span data-ttu-id="af396-122">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="af396-122">Contacts.ReadWrite</span></span> |
|<span data-ttu-id="af396-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af396-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af396-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af396-124">Not supported.</span></span> |
|<span data-ttu-id="af396-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af396-125">Application</span></span>                            | <span data-ttu-id="af396-126">Para recurso de **usuário**:</span><span class="sxs-lookup"><span data-stu-id="af396-126">For **user** resource:</span></span><br/><span data-ttu-id="af396-127">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af396-127">User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="af396-128">Para recurso de **grupo**:</span><span class="sxs-lookup"><span data-stu-id="af396-128">For **group** resource:</span></span><br /><span data-ttu-id="af396-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af396-129">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="af396-130">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="af396-130">For **contact** resource:</span></span><br /><span data-ttu-id="af396-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="af396-131">Contacts.ReadWrite</span></span> |

> <span data-ttu-id="af396-132">**Observação:** para atualizar a foto de qualquer usuário na organização, o aplicativo deve ter a Permissão do aplicativo User.ReadWrite.All e chamar esta API usando a própria identidade, não em nome de um usuário.</span><span class="sxs-lookup"><span data-stu-id="af396-132">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user.</span></span> <span data-ttu-id="af396-133">Para saber mais, confira [obter acesso sem um usuário conectado](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="af396-133">To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span> <span data-ttu-id="af396-134">A atualização da foto do usuário in-loco requer apenas a permissão User.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="af396-134">Updating the photo of the signed-in user only requires User.ReadWrite permission.</span></span>

> <span data-ttu-id="af396-135">**Observação:** Há um [problema conhecido](/graph/known-issues#groups)ao acessar fotos de grupo usando permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="af396-135">**Note:**  There is currently a [known issue](/graph/known-issues#groups) with accessing group photos using application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="af396-136">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af396-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /me/photo/$value
PUT /users/{id | userPrincipalName}/photo/$value
PUT /groups/{id}/photo/$value
PUT /me/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PUT /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```

<span data-ttu-id="af396-137">Para atualizar a foto de uma equipe:</span><span class="sxs-lookup"><span data-stu-id="af396-137">To update the photo for a team:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PUT /groups/{teamId}/photo/$value
```

## <a name="request-headers"></a><span data-ttu-id="af396-138">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af396-138">Request headers</span></span>
| <span data-ttu-id="af396-139">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="af396-139">Header</span></span>       | <span data-ttu-id="af396-140">Valor</span><span class="sxs-lookup"><span data-stu-id="af396-140">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="af396-141">Autorização</span><span class="sxs-lookup"><span data-stu-id="af396-141">Authorization</span></span>  | <span data-ttu-id="af396-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af396-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="af396-144">Content-Type</span><span class="sxs-lookup"><span data-stu-id="af396-144">Content-Type</span></span>  | <span data-ttu-id="af396-p107">image/jpeg. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af396-p107">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="af396-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af396-147">Request body</span></span>
<span data-ttu-id="af396-148">Inclua os dados binários da foto no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="af396-148">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="af396-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="af396-149">Response</span></span>

<span data-ttu-id="af396-150">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="af396-150">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="af396-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af396-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="af396-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af396-152">Request</span></span>
<span data-ttu-id="af396-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="af396-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="af396-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="af396-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
# <a name="c"></a>[<span data-ttu-id="af396-155">C#</span><span class="sxs-lookup"><span data-stu-id="af396-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-profilephoto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="af396-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="af396-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-profilephoto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="af396-157">Java</span><span class="sxs-lookup"><span data-stu-id="af396-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-profilephoto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="af396-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="af396-158">Response</span></span>
<span data-ttu-id="af396-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="af396-159">The following is an example of the response.</span></span> 

><span data-ttu-id="af396-160">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="af396-160">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update profilephoto",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


