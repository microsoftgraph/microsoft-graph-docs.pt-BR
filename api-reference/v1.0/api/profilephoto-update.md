---
title: Atualizar profilephoto
description: Atualize a foto do **usuário** conectado, ou do **grupo** ou **cotato** especificado. Desde lá
localization_priority: Priority
author: kevinbellinger
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 8797b12d070b582a551486ac25678c4f1794adf5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048663"
---
# <a name="update-profilephoto"></a><span data-ttu-id="024ae-104">Atualizar profilephoto</span><span class="sxs-lookup"><span data-stu-id="024ae-104">Update profilephoto</span></span>

<span data-ttu-id="024ae-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="024ae-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="024ae-p102">Atualize a foto do **user** conectado, ou do **group** ou **contact** especificado. Como atualmente há um limite de 4 MB para o tamanho total de cada solicitação REST, isso limita o tamanho da foto que você pode adicionar a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="024ae-p102">Update the photo for the signed-in **user**, or the specified **group** or **contact**. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the photo you can add to under 4MB.</span></span>

<span data-ttu-id="024ae-108">Você pode usar PATCH ou PUT para esta operação na versão 1.0.</span><span class="sxs-lookup"><span data-stu-id="024ae-108">You can use either PATCH or PUT for this operation in version 1.0.</span></span>

> <span data-ttu-id="024ae-109">**Observação** Esta operação na versão 1.0 é compatível com caixas de correio corporativas ou de estudante ou caixas de correio não pessoais dos usuários</span><span class="sxs-lookup"><span data-stu-id="024ae-109">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="024ae-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="024ae-110">Permissions</span></span>
<span data-ttu-id="024ae-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="024ae-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

- <span data-ttu-id="024ae-113">Foto do perfil do **usuário** conectado – User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="024ae-113">Profile photo of the signed-in **user** - User.ReadWrite, User.ReadWrite.All</span></span>
- <span data-ttu-id="024ae-114">Foto do perfil de um **grupo** – Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="024ae-114">Profile photo of a **group** - Group.ReadWrite.All</span></span>
- <span data-ttu-id="024ae-115">Foto de um **contato** – Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="024ae-115">Photo of a **contact** - Contacts.ReadWrite</span></span>

> <span data-ttu-id="024ae-116">**Observação:** para atualizar a foto de qualquer usuário na organização, o aplicativo deve ter a Permissão do aplicativo User.ReadWrite.All e chamar esta API usando a própria identidade, não em nome de um usuário.</span><span class="sxs-lookup"><span data-stu-id="024ae-116">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user.</span></span> <span data-ttu-id="024ae-117">Para saber mais, confira [obter acesso sem um usuário conectado](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="024ae-117">To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span>

> <span data-ttu-id="024ae-118">**Observação:** Há um [problema conhecido](/graph/known-issues#groups)ao acessar fotos de grupo usando permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="024ae-118">**Note:**  There is currently a [known issue](/graph/known-issues#groups) with accessing group photos using application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="024ae-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="024ae-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/photo/$value
PATCH /users/{id | userPrincipalName}/photo/$value
PATCH /groups/{id}/photo/$value
PATCH /me/contacts/{id}/photo/$value
PATCH /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PATCH /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PATCH /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value

PUT /me/photo/$value
PUT /users/{id | userPrincipalName}/photo/$value
PUT /groups/{id}/photo/$value
PUT /me/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contacts/{id}/photo/$value
PUT /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
PUT /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```
## <a name="request-headers"></a><span data-ttu-id="024ae-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="024ae-120">Request headers</span></span>
| <span data-ttu-id="024ae-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="024ae-121">Header</span></span>       | <span data-ttu-id="024ae-122">Valor</span><span class="sxs-lookup"><span data-stu-id="024ae-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="024ae-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="024ae-123">Authorization</span></span>  | <span data-ttu-id="024ae-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="024ae-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="024ae-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="024ae-126">Content-Type</span></span>  | <span data-ttu-id="024ae-p106">image/jpeg. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="024ae-p106">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="024ae-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="024ae-129">Request body</span></span>
<span data-ttu-id="024ae-130">Inclua os dados binários da foto no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="024ae-130">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="024ae-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="024ae-131">Response</span></span>

<span data-ttu-id="024ae-132">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="024ae-132">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="024ae-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="024ae-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="024ae-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="024ae-134">Request</span></span>
<span data-ttu-id="024ae-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="024ae-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="024ae-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="024ae-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/v1.0/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
# <a name="c"></a>[<span data-ttu-id="024ae-137">C#</span><span class="sxs-lookup"><span data-stu-id="024ae-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-profilephoto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="024ae-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="024ae-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-profilephoto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="024ae-139">Java</span><span class="sxs-lookup"><span data-stu-id="024ae-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-profilephoto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="024ae-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="024ae-140">Response</span></span>
<span data-ttu-id="024ae-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="024ae-141">Here is an example of the response.</span></span> <span data-ttu-id="024ae-142">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="024ae-142">Note: The response object shown here might be shortened for readability.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update profilephoto",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

