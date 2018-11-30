---
title: Atualizar profilephoto
description: Atualize a foto entrou no **usuário**, ou do **grupo** de especificado ou **entre em contato**. Desde daí
ms.openlocfilehash: cf20ae6f59f0d912b8bd08a9be42591bb6f97127
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003877"
---
# <a name="update-profilephoto"></a><span data-ttu-id="1162b-104">Atualizar profilephoto</span><span class="sxs-lookup"><span data-stu-id="1162b-104">Update profilephoto</span></span>

<span data-ttu-id="1162b-p102">Atualize a foto do **user** conectado, ou do **group** ou **contact** especificado. Como atualmente há um limite de 4 MB para o tamanho total de cada solicitação REST, isso limita o tamanho da foto que você pode adicionar a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="1162b-p102">Update the photo for the signed-in **user**, or the specified **group** or **contact**. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the photo you can add to under 4MB.</span></span>

<span data-ttu-id="1162b-107">Você pode usar PATCH ou PUT para esta operação na versão 1.0.</span><span class="sxs-lookup"><span data-stu-id="1162b-107">You can use either PATCH or PUT for this operation in version 1.0.</span></span>

> <span data-ttu-id="1162b-108">**Observação** Esta operação na versão 1.0 é compatível com caixas de correio corporativas ou de estudante ou caixas de correio não pessoais dos usuários</span><span class="sxs-lookup"><span data-stu-id="1162b-108">**Note** This operation in version 1.0 supports only a user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="1162b-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="1162b-109">Permissions</span></span>
<span data-ttu-id="1162b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1162b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

- <span data-ttu-id="1162b-112">Foto do perfil de **usuário** conectado – User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1162b-112">Profile photo of the signed-in **user** - User.ReadWrite, User.ReadWrite.All</span></span>
- <span data-ttu-id="1162b-113">Foto do perfil de um **grupo** – Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1162b-113">Profile photo of a **group** - Group.ReadWrite.All</span></span>
- <span data-ttu-id="1162b-114">Foto de um **contato** – Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1162b-114">Photo of a **contact** - Contacts.ReadWrite</span></span>

> <span data-ttu-id="1162b-p104">**Observação:** para atualizar a foto de qualquer usuário na organização, o aplicativo deve ter a Permissão de aplicativo User.ReadWrite.All e chamar esta API usando a própria identidade, não em nome de um usuário. Para saber mais, veja como [obter acesso sem um usuário conectado](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="1162b-p104">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user. To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span>

## <a name="http-request"></a><span data-ttu-id="1162b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1162b-117">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="1162b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1162b-118">Request headers</span></span>
| <span data-ttu-id="1162b-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1162b-119">Header</span></span>       | <span data-ttu-id="1162b-120">Valor</span><span class="sxs-lookup"><span data-stu-id="1162b-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1162b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1162b-121">Authorization</span></span>  | <span data-ttu-id="1162b-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1162b-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1162b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1162b-124">Content-Type</span></span>  | <span data-ttu-id="1162b-p106">image/jpeg. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1162b-p106">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1162b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1162b-127">Request body</span></span>
<span data-ttu-id="1162b-128">Inclua os dados binários da foto no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1162b-128">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="1162b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1162b-129">Response</span></span>

<span data-ttu-id="1162b-130">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="1162b-130">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="1162b-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1162b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1162b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1162b-132">Request</span></span>
<span data-ttu-id="1162b-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1162b-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/v1.0/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
##### <a name="response"></a><span data-ttu-id="1162b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1162b-134">Response</span></span>
<span data-ttu-id="1162b-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1162b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
