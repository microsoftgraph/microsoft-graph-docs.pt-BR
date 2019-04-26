---
title: Atualizar profilephoto
description: Atualize a foto de qualquer usuário no locatário, incluindo o usuário conectado ou o grupo ou contato especificado. Como não há
localization_priority: Normal
ms.openlocfilehash: 1cf4d99f55768a6fad868d91d526fc5fd0b7b5ca
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332049"
---
# <a name="update-profilephoto"></a><span data-ttu-id="f2d52-104">Atualizar profilephoto</span><span class="sxs-lookup"><span data-stu-id="f2d52-104">Update profilephoto</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2d52-105">Atualize a foto de qualquer usuário no locatário, incluindo o usuário conectado ou o grupo ou contato especificado.</span><span class="sxs-lookup"><span data-stu-id="f2d52-105">Update the photo for any user in the tenant including the signed-in user, or the specified group or contact.</span></span> <span data-ttu-id="f2d52-106">Como atualmente há um limite de 4 MB para o tamanho total de cada solicitação REST, isso limita o tamanho da foto que você pode adicionar a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="f2d52-106">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the photo you can add to under 4MB.</span></span>

<span data-ttu-id="f2d52-107">Use apenas o PUT para essa operação na versão beta.</span><span class="sxs-lookup"><span data-stu-id="f2d52-107">Use only PUT for this operation in the beta version.</span></span>

> <span data-ttu-id="f2d52-108">**Observação** A operação atualizar foto no beta oferece suporte somente às caixas de correio corporativa ou de estudante do usuário e não às caixas de correio pessoais.</span><span class="sxs-lookup"><span data-stu-id="f2d52-108">**Note** The update photo operation in beta supports only the user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2d52-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="f2d52-109">Permissions</span></span>
<span data-ttu-id="f2d52-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2d52-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2d52-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2d52-112">Permission type</span></span>      | <span data-ttu-id="f2d52-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f2d52-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2d52-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2d52-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="f2d52-115">Foto de perfil do **usuário**conectado:</span><span class="sxs-lookup"><span data-stu-id="f2d52-115">Profile photo of the signed-in **user**:</span></span><br/><span data-ttu-id="f2d52-116">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f2d52-116">User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="f2d52-117">Para recurso de **grupo**:</span><span class="sxs-lookup"><span data-stu-id="f2d52-117">For **group** resource:</span></span><br /><span data-ttu-id="f2d52-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2d52-118">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="f2d52-119">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="f2d52-119">For **contact** resource:</span></span><br /><span data-ttu-id="f2d52-120">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2d52-120">Contacts.ReadWrite</span></span> |
|<span data-ttu-id="f2d52-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2d52-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2d52-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2d52-122">Not supported.</span></span> |
|<span data-ttu-id="f2d52-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2d52-123">Application</span></span>                            | <span data-ttu-id="f2d52-124">Para recurso de **usuário**:</span><span class="sxs-lookup"><span data-stu-id="f2d52-124">For **user** resource:</span></span><br/><span data-ttu-id="f2d52-125">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2d52-125">User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="f2d52-126">Para recurso de **grupo**:</span><span class="sxs-lookup"><span data-stu-id="f2d52-126">For **group** resource:</span></span><br /><span data-ttu-id="f2d52-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2d52-127">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="f2d52-128">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="f2d52-128">For **contact** resource:</span></span><br /><span data-ttu-id="f2d52-129">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2d52-129">Contacts.ReadWrite</span></span> |

> <span data-ttu-id="f2d52-130">**Observação** Para atualizar a foto de qualquer usuário na organização, seu aplicativo deve ter a permissão User. ReadWrite. All e chamar essa API com sua própria identidade, e não em nome de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f2d52-130">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user.</span></span> <span data-ttu-id="f2d52-131">Para saber mais, confira [obter acesso sem um usuário conectado](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="f2d52-131">To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span>

## <a name="http-request"></a><span data-ttu-id="f2d52-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2d52-132">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="f2d52-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2d52-133">Request headers</span></span>
| <span data-ttu-id="f2d52-134">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2d52-134">Header</span></span>       | <span data-ttu-id="f2d52-135">Valor</span><span class="sxs-lookup"><span data-stu-id="f2d52-135">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f2d52-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2d52-136">Authorization</span></span>  | <span data-ttu-id="f2d52-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2d52-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f2d52-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f2d52-139">Content-Type</span></span>  | <span data-ttu-id="f2d52-p106">image/jpeg. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2d52-p106">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f2d52-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2d52-142">Request body</span></span>
<span data-ttu-id="f2d52-143">Inclua os dados binários da foto no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2d52-143">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="f2d52-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2d52-144">Response</span></span>

<span data-ttu-id="f2d52-145">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="f2d52-145">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="f2d52-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2d52-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f2d52-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2d52-147">Request</span></span>
<span data-ttu-id="f2d52-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2d52-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
##### <a name="response"></a><span data-ttu-id="f2d52-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2d52-149">Response</span></span>
<span data-ttu-id="f2d52-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2d52-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
