---
title: Atualizar profilephoto
description: Atualiza a foto de qualquer usuário no locatário, incluindo o usuário conectado ou o grupo ou contato especificado. Desde lá
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: kevinbellinger
ms.openlocfilehash: 5ba0cb3b88e5048141cea8085550a4c3e389130e
ms.sourcegitcommit: c6e8a2097267ace4c78124be48646f9129114b26
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/03/2020
ms.locfileid: "47340016"
---
# <a name="update-profilephoto"></a><span data-ttu-id="4ca22-104">Atualizar profilephoto</span><span class="sxs-lookup"><span data-stu-id="4ca22-104">Update profilephoto</span></span>

<span data-ttu-id="4ca22-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ca22-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ca22-p102">Atualize a foto de qualquer usuário no locatário, incluindo o usuário conectado ou o grupo ou o contato especificado. Como há no momento um limite de 8MB no tamanho total de cada solicitação REST, o tamanho da foto que você pode adicionar está limitado em 8 MB.</span><span class="sxs-lookup"><span data-stu-id="4ca22-p102">Update the photo for any user in the tenant, including the signed-in user or the specified group or contact. Because there is currently a limit of 8MB on the total size of each REST request, the size of the photo you can add is limited to under 8MB.</span></span>

<span data-ttu-id="4ca22-108">Use PUT somente para esta operação.</span><span class="sxs-lookup"><span data-stu-id="4ca22-108">Only use PUT for this operation.</span></span>

> <span data-ttu-id="4ca22-109">**Observação**: ao atualizar a foto do **usuário** , essa operação primeiro tenta atualizar a foto no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4ca22-109">**Note**:  When updating the **user** photo, this operation first attempts to update the photo in Microsoft 365.</span></span> <span data-ttu-id="4ca22-110">Se isso falhar (porque o usuário não tem uma caixa de correio), essa API tentará atualizar a foto no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4ca22-110">If that fails (due to the user not having a mailbox), this API will attempt to update the photo in Azure Active Directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ca22-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="4ca22-111">Permissions</span></span>
<span data-ttu-id="4ca22-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ca22-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ca22-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ca22-114">Permission type</span></span>      | <span data-ttu-id="4ca22-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4ca22-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ca22-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ca22-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="4ca22-117">Foto de perfil do **usuário**conectado:</span><span class="sxs-lookup"><span data-stu-id="4ca22-117">Profile photo of the signed-in **user**:</span></span><br/><span data-ttu-id="4ca22-118">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4ca22-118">User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="4ca22-119">Para recurso de **grupo**:</span><span class="sxs-lookup"><span data-stu-id="4ca22-119">For **group** resource:</span></span><br /><span data-ttu-id="4ca22-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ca22-120">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="4ca22-121">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="4ca22-121">For **contact** resource:</span></span><br /><span data-ttu-id="4ca22-122">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ca22-122">Contacts.ReadWrite</span></span> |
|<span data-ttu-id="4ca22-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ca22-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ca22-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ca22-124">Not supported.</span></span> |
|<span data-ttu-id="4ca22-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ca22-125">Application</span></span>                            | <span data-ttu-id="4ca22-126">Para recurso de **usuário**:</span><span class="sxs-lookup"><span data-stu-id="4ca22-126">For **user** resource:</span></span><br/><span data-ttu-id="4ca22-127">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ca22-127">User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="4ca22-128">Para recurso de **grupo**:</span><span class="sxs-lookup"><span data-stu-id="4ca22-128">For **group** resource:</span></span><br /><span data-ttu-id="4ca22-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ca22-129">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="4ca22-130">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="4ca22-130">For **contact** resource:</span></span><br /><span data-ttu-id="4ca22-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ca22-131">Contacts.ReadWrite</span></span> |

> <span data-ttu-id="4ca22-132">**Observação:** para atualizar a foto de qualquer usuário na organização, o aplicativo deve ter a Permissão do aplicativo User.ReadWrite.All e chamar esta API usando a própria identidade, não em nome de um usuário.</span><span class="sxs-lookup"><span data-stu-id="4ca22-132">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user.</span></span> <span data-ttu-id="4ca22-133">Para saber mais, confira [obter acesso sem um usuário conectado](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="4ca22-133">To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span> <span data-ttu-id="4ca22-134">A atualização da foto do usuário conectado requer apenas a permissão User. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="4ca22-134">Updating the photo of the signed-in user only requires User.ReadWrite permission.</span></span>

> <span data-ttu-id="4ca22-135">**Observação:** Há um [problema conhecido](/graph/known-issues#groups)ao acessar fotos de grupo usando permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4ca22-135">**Note:**  There is currently a [known issue](/graph/known-issues#groups) with accessing group photos using application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="4ca22-136">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ca22-136">HTTP request</span></span>
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

<span data-ttu-id="4ca22-137">Para atualizar a foto de uma equipe:</span><span class="sxs-lookup"><span data-stu-id="4ca22-137">To update the photo for a team:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PUT /groups/{teamId}/photo/$value`
```

## <a name="request-headers"></a><span data-ttu-id="4ca22-138">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ca22-138">Request headers</span></span>
| <span data-ttu-id="4ca22-139">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4ca22-139">Header</span></span>       | <span data-ttu-id="4ca22-140">Valor</span><span class="sxs-lookup"><span data-stu-id="4ca22-140">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4ca22-141">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ca22-141">Authorization</span></span>  | <span data-ttu-id="4ca22-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ca22-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4ca22-144">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4ca22-144">Content-Type</span></span>  | <span data-ttu-id="4ca22-p107">image/jpeg. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ca22-p107">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4ca22-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ca22-147">Request body</span></span>
<span data-ttu-id="4ca22-148">Inclua os dados binários da foto no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ca22-148">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="4ca22-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ca22-149">Response</span></span>

<span data-ttu-id="4ca22-150">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="4ca22-150">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4ca22-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ca22-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="4ca22-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ca22-152">Request</span></span>
<span data-ttu-id="4ca22-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ca22-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4ca22-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ca22-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
# <a name="c"></a>[<span data-ttu-id="4ca22-155">C#</span><span class="sxs-lookup"><span data-stu-id="4ca22-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-profilephoto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ca22-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ca22-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-profilephoto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="4ca22-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ca22-157">Response</span></span>
<span data-ttu-id="4ca22-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4ca22-158">The following is an example of the response.</span></span> 

><span data-ttu-id="4ca22-159">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4ca22-159">**Note:** The response object shown here might be shortened for readability.</span></span>
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
