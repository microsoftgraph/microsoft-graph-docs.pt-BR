---
title: Atualizar profilephoto
description: Atualizar a foto para qualquer usuário no locatário incluindo assinado do usuário, ou o grupo especificado ou o contato. Desde daí
localization_priority: Normal
ms.openlocfilehash: f8191716471cba565b27ef316b5b13e3b32ecaff
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521128"
---
# <a name="update-profilephoto"></a><span data-ttu-id="be9d4-104">Atualizar profilephoto</span><span class="sxs-lookup"><span data-stu-id="be9d4-104">Update profilephoto</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be9d4-105">Atualizar a foto para qualquer usuário no locatário incluindo assinado do usuário, ou o grupo especificado ou o contato.</span><span class="sxs-lookup"><span data-stu-id="be9d4-105">Update the photo for any user in the tenant including the signed-in user, or the specified group or contact.</span></span> <span data-ttu-id="be9d4-106">Como no momento, há um limite de 4MB no tamanho total de cada solicitação REST, isso limita o tamanho da foto que você pode adicionar ao menos de 4MB.</span><span class="sxs-lookup"><span data-stu-id="be9d4-106">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the photo you can add to under 4MB.</span></span>

<span data-ttu-id="be9d4-107">Use apenas PUT para essa operação na versão beta.</span><span class="sxs-lookup"><span data-stu-id="be9d4-107">Use only PUT for this operation in the beta version.</span></span>

> <span data-ttu-id="be9d4-108">**Observação** A operação de atualização de foto no beta suporta apenas o usuário comercial ou caixas de correio da escola e caixas de correio não pessoais.</span><span class="sxs-lookup"><span data-stu-id="be9d4-108">**Note** The update photo operation in beta supports only the user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="be9d4-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="be9d4-109">Permissions</span></span>
<span data-ttu-id="be9d4-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be9d4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be9d4-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be9d4-112">Permission type</span></span>      | <span data-ttu-id="be9d4-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="be9d4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be9d4-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be9d4-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="be9d4-115">Foto de perfil do entrou no **usuário**:</span><span class="sxs-lookup"><span data-stu-id="be9d4-115">Profile photo of the signed-in **user**:</span></span><br/><span data-ttu-id="be9d4-116">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be9d4-116">User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="be9d4-117">Para recurso de **grupo**:</span><span class="sxs-lookup"><span data-stu-id="be9d4-117">For **group** resource:</span></span><br /><span data-ttu-id="be9d4-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be9d4-118">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="be9d4-119">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="be9d4-119">For **contact** resource:</span></span><br /><span data-ttu-id="be9d4-120">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be9d4-120">Contacts.ReadWrite</span></span> |
|<span data-ttu-id="be9d4-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be9d4-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be9d4-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be9d4-122">Not supported.</span></span> |
|<span data-ttu-id="be9d4-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="be9d4-123">Application</span></span>                            | <span data-ttu-id="be9d4-124">Para recurso de **usuário**:</span><span class="sxs-lookup"><span data-stu-id="be9d4-124">For **user** resource:</span></span><br/><span data-ttu-id="be9d4-125">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be9d4-125">User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="be9d4-126">Para recurso de **grupo**:</span><span class="sxs-lookup"><span data-stu-id="be9d4-126">For **group** resource:</span></span><br /><span data-ttu-id="be9d4-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be9d4-127">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="be9d4-128">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="be9d4-128">For **contact** resource:</span></span><br /><span data-ttu-id="be9d4-129">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be9d4-129">Contacts.ReadWrite</span></span> |

> <span data-ttu-id="be9d4-p104">**Observação:** para atualizar a foto de qualquer usuário na organização, o aplicativo deve ter a Permissão de aplicativo User.ReadWrite.All e chamar esta API usando a própria identidade, não em nome de um usuário. Para saber mais, veja como [obter acesso sem um usuário conectado](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="be9d4-p104">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user. To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span>

## <a name="http-request"></a><span data-ttu-id="be9d4-132">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be9d4-132">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="be9d4-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be9d4-133">Request headers</span></span>
| <span data-ttu-id="be9d4-134">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="be9d4-134">Header</span></span>       | <span data-ttu-id="be9d4-135">Valor</span><span class="sxs-lookup"><span data-stu-id="be9d4-135">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="be9d4-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="be9d4-136">Authorization</span></span>  | <span data-ttu-id="be9d4-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be9d4-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="be9d4-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="be9d4-139">Content-Type</span></span>  | <span data-ttu-id="be9d4-p106">image/jpeg. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be9d4-p106">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="be9d4-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be9d4-142">Request body</span></span>
<span data-ttu-id="be9d4-143">Inclua os dados binários da foto no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="be9d4-143">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="be9d4-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="be9d4-144">Response</span></span>

<span data-ttu-id="be9d4-145">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="be9d4-145">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="be9d4-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="be9d4-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be9d4-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be9d4-147">Request</span></span>
<span data-ttu-id="be9d4-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="be9d4-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
##### <a name="response"></a><span data-ttu-id="be9d4-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="be9d4-149">Response</span></span>
<span data-ttu-id="be9d4-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="be9d4-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/profilephoto-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
