---
title: Atualizar profilephoto
description: Atualiza a foto de qualquer usuário no locatário, incluindo o usuário conectado ou o grupo ou contato especificado. Desde lá
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 6cc62c6f7ee588e04f9668456808aa89389a171f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455022"
---
# <a name="update-profilephoto"></a><span data-ttu-id="f1bda-104">Atualizar profilephoto</span><span class="sxs-lookup"><span data-stu-id="f1bda-104">Update profilephoto</span></span>

<span data-ttu-id="f1bda-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f1bda-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1bda-106">Atualiza a foto de qualquer usuário no locatário, incluindo o usuário conectado ou o grupo ou contato especificado.</span><span class="sxs-lookup"><span data-stu-id="f1bda-106">Update the photo for any user in the tenant including the signed-in user, or the specified group or contact.</span></span> <span data-ttu-id="f1bda-107">Como atualmente há um limite de 4 MB para o tamanho total de cada solicitação REST, isso limita o tamanho da foto que você pode adicionar a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="f1bda-107">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the photo you can add to under 4MB.</span></span>

<span data-ttu-id="f1bda-108">Use apenas o PUT para essa operação na versão beta.</span><span class="sxs-lookup"><span data-stu-id="f1bda-108">Use only PUT for this operation in the beta version.</span></span>

> <span data-ttu-id="f1bda-109">**Observação** A operação atualizar foto no beta oferece suporte somente às caixas de correio corporativa ou de estudante do usuário e não às caixas de correio pessoais.</span><span class="sxs-lookup"><span data-stu-id="f1bda-109">**Note** The update photo operation in beta supports only the user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1bda-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1bda-110">Permissions</span></span>
<span data-ttu-id="f1bda-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1bda-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1bda-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1bda-113">Permission type</span></span>      | <span data-ttu-id="f1bda-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1bda-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1bda-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1bda-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="f1bda-116">Foto de perfil do **usuário**conectado:</span><span class="sxs-lookup"><span data-stu-id="f1bda-116">Profile photo of the signed-in **user**:</span></span><br/><span data-ttu-id="f1bda-117">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f1bda-117">User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="f1bda-118">Para recurso de **grupo**:</span><span class="sxs-lookup"><span data-stu-id="f1bda-118">For **group** resource:</span></span><br /><span data-ttu-id="f1bda-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1bda-119">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="f1bda-120">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="f1bda-120">For **contact** resource:</span></span><br /><span data-ttu-id="f1bda-121">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1bda-121">Contacts.ReadWrite</span></span> |
|<span data-ttu-id="f1bda-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1bda-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1bda-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1bda-123">Not supported.</span></span> |
|<span data-ttu-id="f1bda-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1bda-124">Application</span></span>                            | <span data-ttu-id="f1bda-125">Para recurso de **usuário**:</span><span class="sxs-lookup"><span data-stu-id="f1bda-125">For **user** resource:</span></span><br/><span data-ttu-id="f1bda-126">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1bda-126">User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="f1bda-127">Para recurso de **grupo**:</span><span class="sxs-lookup"><span data-stu-id="f1bda-127">For **group** resource:</span></span><br /><span data-ttu-id="f1bda-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1bda-128">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="f1bda-129">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="f1bda-129">For **contact** resource:</span></span><br /><span data-ttu-id="f1bda-130">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f1bda-130">Contacts.ReadWrite</span></span> |

> <span data-ttu-id="f1bda-131">**Observação:** para atualizar a foto de qualquer usuário na organização, o aplicativo deve ter a Permissão do aplicativo User.ReadWrite.All e chamar esta API usando a própria identidade, não em nome de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f1bda-131">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user.</span></span> <span data-ttu-id="f1bda-132">Para saber mais, confira [obter acesso sem um usuário conectado](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="f1bda-132">To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span>

> <span data-ttu-id="f1bda-133">**Observação:** Há um [problema conhecido](/graph/known-issues#groups)ao acessar fotos de grupo usando permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f1bda-133">**Note:**  There is currently a [known issue](/graph/known-issues#groups) with accessing group photos using application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="f1bda-134">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1bda-134">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="f1bda-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1bda-135">Request headers</span></span>
| <span data-ttu-id="f1bda-136">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f1bda-136">Header</span></span>       | <span data-ttu-id="f1bda-137">Valor</span><span class="sxs-lookup"><span data-stu-id="f1bda-137">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f1bda-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1bda-138">Authorization</span></span>  | <span data-ttu-id="f1bda-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1bda-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f1bda-141">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f1bda-141">Content-Type</span></span>  | <span data-ttu-id="f1bda-p106">image/jpeg. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1bda-p106">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f1bda-144">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1bda-144">Request body</span></span>
<span data-ttu-id="f1bda-145">Inclua os dados binários da foto no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1bda-145">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="f1bda-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1bda-146">Response</span></span>

<span data-ttu-id="f1bda-147">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="f1bda-147">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="f1bda-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1bda-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1bda-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1bda-149">Request</span></span>
<span data-ttu-id="f1bda-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1bda-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f1bda-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1bda-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
# <a name="c"></a>[<span data-ttu-id="f1bda-152">C#</span><span class="sxs-lookup"><span data-stu-id="f1bda-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-profilephoto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1bda-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1bda-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-profilephoto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f1bda-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1bda-154">Response</span></span>
<span data-ttu-id="f1bda-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1bda-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
