---
title: Atualizar profilephoto
description: Atualiza a foto de qualquer usuário no locatário, incluindo o usuário conectado ou o grupo ou contato especificado. Desde lá
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: bafdd48cf95f8f6c6eddb99a0cd4f4bb3138dd78
ms.sourcegitcommit: 41a5bd5868685c10181f6285d5ac91c6dad556e2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/04/2020
ms.locfileid: "45038678"
---
# <a name="update-profilephoto"></a><span data-ttu-id="f64b7-104">Atualizar profilephoto</span><span class="sxs-lookup"><span data-stu-id="f64b7-104">Update profilephoto</span></span>

<span data-ttu-id="f64b7-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f64b7-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f64b7-106">Update the photo for any user in the tenant including the signed-in user, or the specified group or contact.</span><span class="sxs-lookup"><span data-stu-id="f64b7-106">Update the photo for any user in the tenant including the signed-in user, or the specified group or contact.</span></span> <span data-ttu-id="f64b7-107">Since there is currently a limit of 8MB on the total size of each REST request, this limits the size of the photo you can add to under 8MB.</span><span class="sxs-lookup"><span data-stu-id="f64b7-107">Since there is currently a limit of 8MB on the total size of each REST request, this limits the size of the photo you can add to under 8MB.</span></span>

<span data-ttu-id="f64b7-108">Use apenas o PUT para essa operação na versão beta.</span><span class="sxs-lookup"><span data-stu-id="f64b7-108">Use only PUT for this operation in the beta version.</span></span>

> <span data-ttu-id="f64b7-109">**Observação**: ao atualizar a foto do **usuário** , essa operação primeiro tenta atualizar a foto no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f64b7-109">**Note**:  When updating the **user** photo, this operation first attempts to update the photo in Microsoft 365.</span></span> <span data-ttu-id="f64b7-110">Se isso falhar (porque o usuário não tem uma caixa de correio), essa API tentará atualizar a foto no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f64b7-110">If that fails (due to the user not having a mailbox), this API will attempt to update the photo in Azure Active Directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="f64b7-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="f64b7-111">Permissions</span></span>
<span data-ttu-id="f64b7-112">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="f64b7-112">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f64b7-113">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f64b7-113">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f64b7-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f64b7-114">Permission type</span></span>      | <span data-ttu-id="f64b7-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f64b7-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f64b7-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f64b7-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="f64b7-117">Foto de perfil do **usuário**conectado:</span><span class="sxs-lookup"><span data-stu-id="f64b7-117">Profile photo of the signed-in **user**:</span></span><br/><span data-ttu-id="f64b7-118">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f64b7-118">User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="f64b7-119">Para recurso de **grupo**:</span><span class="sxs-lookup"><span data-stu-id="f64b7-119">For **group** resource:</span></span><br /><span data-ttu-id="f64b7-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f64b7-120">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="f64b7-121">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="f64b7-121">For **contact** resource:</span></span><br /><span data-ttu-id="f64b7-122">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f64b7-122">Contacts.ReadWrite</span></span> |
|<span data-ttu-id="f64b7-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f64b7-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f64b7-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f64b7-124">Not supported.</span></span> |
|<span data-ttu-id="f64b7-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f64b7-125">Application</span></span>                            | <span data-ttu-id="f64b7-126">Para recurso de **usuário**:</span><span class="sxs-lookup"><span data-stu-id="f64b7-126">For **user** resource:</span></span><br/><span data-ttu-id="f64b7-127">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f64b7-127">User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="f64b7-128">Para recurso de **grupo**:</span><span class="sxs-lookup"><span data-stu-id="f64b7-128">For **group** resource:</span></span><br /><span data-ttu-id="f64b7-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f64b7-129">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="f64b7-130">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="f64b7-130">For **contact** resource:</span></span><br /><span data-ttu-id="f64b7-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f64b7-131">Contacts.ReadWrite</span></span> |

> <span data-ttu-id="f64b7-132">**Observação:** para atualizar a foto de qualquer usuário na organização, o aplicativo deve ter a Permissão do aplicativo User.ReadWrite.All e chamar esta API usando a própria identidade, não em nome de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f64b7-132">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user.</span></span> <span data-ttu-id="f64b7-133">Para saber mais, confira [obter acesso sem um usuário conectado](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="f64b7-133">To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span> <span data-ttu-id="f64b7-134">A atualização da foto do usuário conectado requer apenas a permissão User. ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="f64b7-134">Updating the photo of the signed-in user only requires User.ReadWrite permission.</span></span>

> <span data-ttu-id="f64b7-135">**Observação:** Há um [problema conhecido](/graph/known-issues#groups)ao acessar fotos de grupo usando permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f64b7-135">**Note:**  There is currently a [known issue](/graph/known-issues#groups) with accessing group photos using application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="f64b7-136">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f64b7-136">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="f64b7-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f64b7-137">Request headers</span></span>
| <span data-ttu-id="f64b7-138">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f64b7-138">Header</span></span>       | <span data-ttu-id="f64b7-139">Valor</span><span class="sxs-lookup"><span data-stu-id="f64b7-139">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f64b7-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="f64b7-140">Authorization</span></span>  | <span data-ttu-id="f64b7-141">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="f64b7-141">Bearer {token}.</span></span> <span data-ttu-id="f64b7-142">Required.</span><span class="sxs-lookup"><span data-stu-id="f64b7-142">Required.</span></span>  |
| <span data-ttu-id="f64b7-143">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f64b7-143">Content-Type</span></span>  | <span data-ttu-id="f64b7-144">image/jpeg.</span><span class="sxs-lookup"><span data-stu-id="f64b7-144">image/jpeg.</span></span> <span data-ttu-id="f64b7-145">Required.</span><span class="sxs-lookup"><span data-stu-id="f64b7-145">Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f64b7-146">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f64b7-146">Request body</span></span>
<span data-ttu-id="f64b7-147">Inclua os dados binários da foto no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f64b7-147">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="f64b7-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="f64b7-148">Response</span></span>

<span data-ttu-id="f64b7-149">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="f64b7-149">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f64b7-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f64b7-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f64b7-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f64b7-151">Request</span></span>
<span data-ttu-id="f64b7-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f64b7-152">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f64b7-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="f64b7-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
# <a name="c"></a>[<span data-ttu-id="f64b7-154">C#</span><span class="sxs-lookup"><span data-stu-id="f64b7-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-profilephoto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f64b7-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f64b7-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-profilephoto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f64b7-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="f64b7-156">Response</span></span>
<span data-ttu-id="f64b7-157">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="f64b7-157">Here is an example of the response.</span></span> <span data-ttu-id="f64b7-158">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="f64b7-158">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f64b7-159">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="f64b7-159">All of the properties will be returned from an actual call.</span></span>
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
