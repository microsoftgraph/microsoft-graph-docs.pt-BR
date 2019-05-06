---
title: Atualizar profilephoto
description: Atualize a foto de qualquer usuário no locatário, incluindo o usuário conectado ou o grupo ou contato especificado. Desde lá
localization_priority: Normal
ms.openlocfilehash: eb094fa7dfd8fdac18fe5fcdb975ed73cf90470b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593684"
---
# <a name="update-profilephoto"></a><span data-ttu-id="c0495-104">Atualizar profilephoto</span><span class="sxs-lookup"><span data-stu-id="c0495-104">Update profilephoto</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0495-105">Atualize a foto de qualquer usuário no locatário, incluindo o usuário conectado ou o grupo ou contato especificado.</span><span class="sxs-lookup"><span data-stu-id="c0495-105">Update the photo for any user in the tenant including the signed-in user, or the specified group or contact.</span></span> <span data-ttu-id="c0495-106">Como atualmente há um limite de 4 MB para o tamanho total de cada solicitação REST, isso limita o tamanho da foto que você pode adicionar a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="c0495-106">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the photo you can add to under 4MB.</span></span>

<span data-ttu-id="c0495-107">Use apenas o PUT para essa operação na versão beta.</span><span class="sxs-lookup"><span data-stu-id="c0495-107">Use only PUT for this operation in the beta version.</span></span>

> <span data-ttu-id="c0495-108">**Observação** A operação atualizar foto no beta oferece suporte somente às caixas de correio corporativa ou de estudante do usuário e não às caixas de correio pessoais.</span><span class="sxs-lookup"><span data-stu-id="c0495-108">**Note** The update photo operation in beta supports only the user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0495-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0495-109">Permissions</span></span>
<span data-ttu-id="c0495-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0495-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0495-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0495-112">Permission type</span></span>      | <span data-ttu-id="c0495-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0495-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0495-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0495-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="c0495-115">Foto de perfil do **usuário**conectado:</span><span class="sxs-lookup"><span data-stu-id="c0495-115">Profile photo of the signed-in **user**:</span></span><br/><span data-ttu-id="c0495-116">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c0495-116">User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="c0495-117">Para recurso de **grupo**:</span><span class="sxs-lookup"><span data-stu-id="c0495-117">For **group** resource:</span></span><br /><span data-ttu-id="c0495-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0495-118">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="c0495-119">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="c0495-119">For **contact** resource:</span></span><br /><span data-ttu-id="c0495-120">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0495-120">Contacts.ReadWrite</span></span> |
|<span data-ttu-id="c0495-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0495-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0495-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0495-122">Not supported.</span></span> |
|<span data-ttu-id="c0495-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0495-123">Application</span></span>                            | <span data-ttu-id="c0495-124">Para recurso de **usuário**:</span><span class="sxs-lookup"><span data-stu-id="c0495-124">For **user** resource:</span></span><br/><span data-ttu-id="c0495-125">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0495-125">User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="c0495-126">Para recurso de **grupo**:</span><span class="sxs-lookup"><span data-stu-id="c0495-126">For **group** resource:</span></span><br /><span data-ttu-id="c0495-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0495-127">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="c0495-128">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="c0495-128">For **contact** resource:</span></span><br /><span data-ttu-id="c0495-129">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0495-129">Contacts.ReadWrite</span></span> |

> <span data-ttu-id="c0495-130">**Observação:** para atualizar a foto de qualquer usuário na organização, o aplicativo deve ter a Permissão do aplicativo User.ReadWrite.All e chamar esta API usando a própria identidade, não em nome de um usuário.</span><span class="sxs-lookup"><span data-stu-id="c0495-130">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user.</span></span> <span data-ttu-id="c0495-131">Para saber mais, confira [obter acesso sem um usuário conectado](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="c0495-131">To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span>

## <a name="http-request"></a><span data-ttu-id="c0495-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0495-132">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="c0495-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0495-133">Request headers</span></span>
| <span data-ttu-id="c0495-134">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c0495-134">Header</span></span>       | <span data-ttu-id="c0495-135">Valor</span><span class="sxs-lookup"><span data-stu-id="c0495-135">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c0495-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0495-136">Authorization</span></span>  | <span data-ttu-id="c0495-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0495-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c0495-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c0495-139">Content-Type</span></span>  | <span data-ttu-id="c0495-p106">image/jpeg. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0495-p106">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c0495-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0495-142">Request body</span></span>
<span data-ttu-id="c0495-143">Inclua os dados binários da foto no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0495-143">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="c0495-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0495-144">Response</span></span>

<span data-ttu-id="c0495-145">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="c0495-145">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="c0495-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0495-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0495-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0495-147">Request</span></span>
<span data-ttu-id="c0495-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0495-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
##### <a name="response"></a><span data-ttu-id="c0495-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0495-149">Response</span></span>
<span data-ttu-id="c0495-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0495-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c0495-153">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="c0495-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c0495-154">Basic</span><span class="sxs-lookup"><span data-stu-id="c0495-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_profilephoto-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c0495-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0495-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_profilephoto-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/profilephoto-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/profilephoto-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
