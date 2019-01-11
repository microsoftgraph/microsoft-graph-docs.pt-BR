---
title: Atualizar profilephoto
description: Atualizar a foto para qualquer usuário no locatário incluindo assinado do usuário, ou o grupo especificado ou o contato. Desde daí
localization_priority: Normal
ms.openlocfilehash: e79a58d92276cc88884874c0a3339d52ac8c2847
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850880"
---
# <a name="update-profilephoto"></a><span data-ttu-id="44326-104">Atualizar profilephoto</span><span class="sxs-lookup"><span data-stu-id="44326-104">Update profilephoto</span></span>

> <span data-ttu-id="44326-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="44326-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44326-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="44326-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="44326-107">Atualizar a foto para qualquer usuário no locatário incluindo assinado do usuário, ou o grupo especificado ou o contato.</span><span class="sxs-lookup"><span data-stu-id="44326-107">Update the photo for any user in the tenant including the signed-in user, or the specified group or contact.</span></span> <span data-ttu-id="44326-108">Como no momento, há um limite de 4MB no tamanho total de cada solicitação REST, isso limita o tamanho da foto que você pode adicionar ao menos de 4MB.</span><span class="sxs-lookup"><span data-stu-id="44326-108">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the photo you can add to under 4MB.</span></span>

<span data-ttu-id="44326-109">Use apenas PUT para essa operação na versão beta.</span><span class="sxs-lookup"><span data-stu-id="44326-109">Use only PUT for this operation in the beta version.</span></span>

> <span data-ttu-id="44326-110">**Observação** A operação de atualização de foto no beta suporta apenas o usuário comercial ou caixas de correio da escola e caixas de correio não pessoais.</span><span class="sxs-lookup"><span data-stu-id="44326-110">**Note** The update photo operation in beta supports only the user's work or school mailboxes and not personal mailboxes.</span></span>

## <a name="permissions"></a><span data-ttu-id="44326-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="44326-111">Permissions</span></span>
<span data-ttu-id="44326-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44326-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44326-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="44326-114">Permission type</span></span>      | <span data-ttu-id="44326-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="44326-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44326-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="44326-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="44326-117">Foto de perfil do entrou no **usuário**:</span><span class="sxs-lookup"><span data-stu-id="44326-117">Profile photo of the signed-in **user**:</span></span><br/><span data-ttu-id="44326-118">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44326-118">User.ReadWrite, User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="44326-119">Para recurso de **grupo**:</span><span class="sxs-lookup"><span data-stu-id="44326-119">For **group** resource:</span></span><br /><span data-ttu-id="44326-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44326-120">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="44326-121">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="44326-121">For **contact** resource:</span></span><br /><span data-ttu-id="44326-122">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44326-122">Contacts.ReadWrite</span></span> |
|<span data-ttu-id="44326-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="44326-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44326-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44326-124">Not supported.</span></span> |
|<span data-ttu-id="44326-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="44326-125">Application</span></span>                            | <span data-ttu-id="44326-126">Para recurso de **usuário**:</span><span class="sxs-lookup"><span data-stu-id="44326-126">For **user** resource:</span></span><br/><span data-ttu-id="44326-127">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44326-127">User.ReadWrite.All</span></span><br /><br /><span data-ttu-id="44326-128">Para recurso de **grupo**:</span><span class="sxs-lookup"><span data-stu-id="44326-128">For **group** resource:</span></span><br /><span data-ttu-id="44326-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44326-129">Group.ReadWrite.All</span></span><br /><br /><span data-ttu-id="44326-130">Para recurso de **contato**:</span><span class="sxs-lookup"><span data-stu-id="44326-130">For **contact** resource:</span></span><br /><span data-ttu-id="44326-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44326-131">Contacts.ReadWrite</span></span> |

> <span data-ttu-id="44326-p105">**Observação:** para atualizar a foto de qualquer usuário na organização, o aplicativo deve ter a Permissão de aplicativo User.ReadWrite.All e chamar esta API usando a própria identidade, não em nome de um usuário. Para saber mais, veja como [obter acesso sem um usuário conectado](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="44326-p105">**Note** To update the photo of any user in the organization, your app must have the User.ReadWrite.All application permission and call this API under its own identity, not on behalf of a user. To learn more, see [get access without a signed-in user](/graph/auth-v2-service).</span></span>

## <a name="http-request"></a><span data-ttu-id="44326-134">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="44326-134">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="44326-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="44326-135">Request headers</span></span>
| <span data-ttu-id="44326-136">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="44326-136">Header</span></span>       | <span data-ttu-id="44326-137">Valor</span><span class="sxs-lookup"><span data-stu-id="44326-137">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="44326-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="44326-138">Authorization</span></span>  | <span data-ttu-id="44326-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44326-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="44326-141">Content-Type</span><span class="sxs-lookup"><span data-stu-id="44326-141">Content-Type</span></span>  | <span data-ttu-id="44326-p107">image/jpeg. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44326-p107">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="44326-144">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="44326-144">Request body</span></span>
<span data-ttu-id="44326-145">Inclua os dados binários da foto no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="44326-145">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="44326-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="44326-146">Response</span></span>

<span data-ttu-id="44326-147">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="44326-147">If successful, this method returns a `200 OK` response code.</span></span>
## <a name="example"></a><span data-ttu-id="44326-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44326-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44326-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44326-149">Request</span></span>
<span data-ttu-id="44326-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="44326-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_profilephoto"
}-->
```http
PUT https://graph.microsoft.com/beta/me/photo/$value
Content-type: image/jpeg

Binary data for the image

```
##### <a name="response"></a><span data-ttu-id="44326-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="44326-151">Response</span></span>
<span data-ttu-id="44326-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="44326-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
