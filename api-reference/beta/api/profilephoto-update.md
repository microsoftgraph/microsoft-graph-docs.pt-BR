---
title: Atualizar profilephoto
description: Atualize a foto de qualquer usuário no locatário, incluindo o usuário conectado ou o grupo ou contato especificado. Desde lá
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: c36e5d21d3082404e6622332adc400896b46ff26
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978648"
---
# <a name="update-profilephoto"></a><span data-ttu-id="da794-104">Atualizar profilephoto</span><span class="sxs-lookup"><span data-stu-id="da794-104">Update profilephoto</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da794-105">Atualize a foto de qualquer usuário no locatário, incluindo o usuário conectado ou o grupo ou contato especificado.</span><span class="sxs-lookup"><span data-stu-id="da794-105">Update the photo for any user in the tenant including the signed-in user, or the specified group or contact.</span></span> <span data-ttu-id="da794-106">Como atualmente há um limite de 4 MB para o tamanho total de cada solicitação REST, isso limita o tamanho da foto que você pode adicionar a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="da794-106">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the photo you can add to under 4MB.</span></span>

<span data-ttu-id="da794-107">Use apenas o PUT para essa operação na versão beta.</span><span class="sxs-lookup"><span data-stu-id="da794-107">Use only PUT for this operation in the beta version.</span></span>

> <span data-ttu-id="da794-108">**Observação** A operação atualizar foto no beta oferece suporte somente às caixas de correio corporativa ou de estudante do usuário e não às caixas de correio pessoais.</span><span class="sxs-lookup"><span data-stu-id="da794-108">**Note** The update photo operation in beta supports only the user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="da794-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="da794-109">Permissions</span></span>
<span data-ttu-id="da794-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da794-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da794-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da794-112">Permission type</span></span>      | <span data-ttu-id="da794-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da794-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da794-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da794-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="da794-115">Foto de perfil do **usuário**conectado:</span><span class="sxs-lookup"><span data-stu-id="da794-115">Profile photo of the signed-in **user**:</span></span><br/><span data-ttu-id="da794-116">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="da794-116">User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="da794-117">Para recurso de **grupo**:</span><span class="sxs-lookup"><span data-stu-id="da794-117">For **group** resource:</span></span><br /><span data-ttu-id="da794-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da794-118">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="da794-119">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="da794-119">For **contact** resource:</span></span><br /><span data-ttu-id="da794-120">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da794-120">Contacts.ReadWrite</span></span> |
|<span data-ttu-id="da794-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da794-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da794-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da794-122">Not supported.</span></span> |
|<span data-ttu-id="da794-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da794-123">Application</span></span>                            | <span data-ttu-id="da794-124">Para recurso de **usuário**:</span><span class="sxs-lookup"><span data-stu-id="da794-124">For **user** resource:</span></span><br/><span data-ttu-id="da794-125">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da794-125">User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="da794-126">Para recurso de **grupo**:</span><span class="sxs-lookup"><span data-stu-id="da794-126">For **group** resource:</span></span><br /><span data-ttu-id="da794-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da794-127">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="da794-128">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="da794-128">For **contact** resource:</span></span><br /><span data-ttu-id="da794-129">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da794-129">Contacts.ReadWrite</span></span> |

> <span data-ttu-id="da794-130">**Observação:** para atualizar a foto de qualquer usuário na organização, o aplicativo deve ter a Permissão do aplicativo User.ReadWrite.All e chamar esta API usando a própria identidade, não em nome de um usuário.</span><span class="sxs-lookup"><span data-stu-id="da794-130">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user.</span></span> <span data-ttu-id="da794-131">Para saber mais, confira [obter acesso sem um usuário conectado](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="da794-131">To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span>

> <span data-ttu-id="da794-132">**Observação:**  No momento, há um [problema conhecido](https://docs.microsoft.com/en-us/graph/known-issues#groups) com o acesso a fotos de grupo usando permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="da794-132">**Note:**  There is currently a [known issue](https://docs.microsoft.com/en-us/graph/known-issues#groups) with accessing group photos using application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="da794-133">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da794-133">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="da794-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da794-134">Request headers</span></span>
| <span data-ttu-id="da794-135">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="da794-135">Header</span></span>       | <span data-ttu-id="da794-136">Valor</span><span class="sxs-lookup"><span data-stu-id="da794-136">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="da794-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="da794-137">Authorization</span></span>  | <span data-ttu-id="da794-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da794-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="da794-140">Content-Type</span><span class="sxs-lookup"><span data-stu-id="da794-140">Content-Type</span></span>  | <span data-ttu-id="da794-p106">image/jpeg. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da794-p106">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="da794-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da794-143">Request body</span></span>
<span data-ttu-id="da794-144">Inclua os dados binários da foto no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da794-144">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="da794-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="da794-145">Response</span></span>

<span data-ttu-id="da794-146">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="da794-146">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="da794-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da794-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da794-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da794-148">Request</span></span>
<span data-ttu-id="da794-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da794-149">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="da794-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="da794-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
# <a name="ctabcsharp"></a>[<span data-ttu-id="da794-151">C#</span><span class="sxs-lookup"><span data-stu-id="da794-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-profilephoto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="da794-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="da794-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-profilephoto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="da794-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="da794-153">Response</span></span>
<span data-ttu-id="da794-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da794-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
