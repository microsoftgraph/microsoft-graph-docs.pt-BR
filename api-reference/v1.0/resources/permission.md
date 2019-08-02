---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Permissão
localization_priority: Priority
description: O recurso Permission fornece informações sobre uma permissão de compartilhamento concedida a um recurso DriveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 95a5b9785285cd6286cf9ebefd8d62fa900c3d9d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035480"
---
# <a name="permission-resource-type"></a><span data-ttu-id="623ef-103">Tipo de recurso permission</span><span class="sxs-lookup"><span data-stu-id="623ef-103">Permission resource type</span></span>

<span data-ttu-id="623ef-104">O recurso **Permission** fornece informações sobre uma permissão de compartilhamento concedida a um recurso [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="623ef-104">The **Permission** resource provides information about a sharing permission granted for a [DriveItem](driveitem.md) resource.</span></span>

<span data-ttu-id="623ef-105">As permissões de compartilhamento têm várias formas diferentes.</span><span class="sxs-lookup"><span data-stu-id="623ef-105">Sharing permissions have a number of different forms.</span></span>
<span data-ttu-id="623ef-106">O recurso **Permission** representa estes diferentes formulários por meio de facetas do recurso.</span><span class="sxs-lookup"><span data-stu-id="623ef-106">The **Permission** resource represents these different forms through facets on the resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="623ef-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="623ef-107">JSON representation</span></span>

<span data-ttu-id="623ef-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="623ef-108">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "link",
    "grantedTo",
    "invitation",
    "inheritedFrom",
    "shareId"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.permission"
}-->
```json
{
  "id": "string (identifier)",
  "grantedTo": {"@odata.type": "microsoft.graph.identitySet"},
  "inheritedFrom": {"@odata.type": "microsoft.graph.itemReference"},
  "invitation": {"@odata.type": "microsoft.graph.sharingInvitation"},
  "link": {"@odata.type": "microsoft.graph.sharingLink"},
  "roles": ["string"],
  "shareId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="623ef-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="623ef-109">Properties</span></span>

| <span data-ttu-id="623ef-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="623ef-110">Property</span></span>      | <span data-ttu-id="623ef-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="623ef-111">Type</span></span>                                      | <span data-ttu-id="623ef-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="623ef-112">Description</span></span>
|:--------------|:------------------------------------------|:-----------------
| <span data-ttu-id="623ef-113">id</span><span class="sxs-lookup"><span data-stu-id="623ef-113">id</span></span>            | <span data-ttu-id="623ef-114">String</span><span class="sxs-lookup"><span data-stu-id="623ef-114">String</span></span>                                    | <span data-ttu-id="623ef-p102">O identificador exclusivo da permissão entre todas as permissões no item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="623ef-p102">The unique identifier of the permission among all permissions on the item. Read-only.</span></span>
| <span data-ttu-id="623ef-117">grantedTo</span><span class="sxs-lookup"><span data-stu-id="623ef-117">grantedTo</span></span>     | [<span data-ttu-id="623ef-118">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="623ef-118">IdentitySet</span></span>](identityset.md)             | <span data-ttu-id="623ef-p103">Para permissões de tipo de usuário, os detalhes de usuários e aplicativos para esta permissão. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="623ef-p103">For user type permissions, the details of the users & applications for this permission. Read-only.</span></span>
| <span data-ttu-id="623ef-121">invitation</span><span class="sxs-lookup"><span data-stu-id="623ef-121">invitation</span></span>    | <span data-ttu-id="623ef-122">[SharingInvitation][]</span><span class="sxs-lookup"><span data-stu-id="623ef-122">[SharingInvitation][]</span></span>                     | <span data-ttu-id="623ef-p104">Detalhes de um convite de compartilhamento associado para esta permissão. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="623ef-p104">Details of any associated sharing invitation for this permission. Read-only.</span></span>
| <span data-ttu-id="623ef-125">inheritedFrom</span><span class="sxs-lookup"><span data-stu-id="623ef-125">inheritedFrom</span></span> | [<span data-ttu-id="623ef-126">ItemReference</span><span class="sxs-lookup"><span data-stu-id="623ef-126">ItemReference</span></span>](itemreference.md)         | <span data-ttu-id="623ef-p105">Fornece uma referência para o ancestral da permissão atual, se ela for herdada de um ancestral. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="623ef-p105">Provides a reference to the ancestor of the current permission, if it is inherited from an ancestor. Read-only.</span></span>
| <span data-ttu-id="623ef-129">vínculo</span><span class="sxs-lookup"><span data-stu-id="623ef-129">link</span></span>          | <span data-ttu-id="623ef-130">[SharingLink][]</span><span class="sxs-lookup"><span data-stu-id="623ef-130">[SharingLink][]</span></span>                           | <span data-ttu-id="623ef-p106">Fornece os detalhes do link de permissão atual, caso se trate de permissões de tipo de link. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="623ef-p106">Provides the link details of the current permission, if it is a link type permissions. Read-only.</span></span>
| <span data-ttu-id="623ef-133">funções</span><span class="sxs-lookup"><span data-stu-id="623ef-133">roles</span></span>         | <span data-ttu-id="623ef-134">Coleção de Cadeias de Caracteres</span><span class="sxs-lookup"><span data-stu-id="623ef-134">Collection of String</span></span>                      | <span data-ttu-id="623ef-p107">O tipo de permissão, por exemplo, `read`. Veja abaixo a lista completa de funções. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="623ef-p107">The type of permission, e.g. `read`. See below for the full list of roles. Read-only.</span></span>
| <span data-ttu-id="623ef-138">shareId</span><span class="sxs-lookup"><span data-stu-id="623ef-138">shareId</span></span>       | <span data-ttu-id="623ef-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="623ef-139">String</span></span>                                    | <span data-ttu-id="623ef-p108">Um token exclusivo que pode ser usado para acessar esse item compartilhado por meio da [**API** Shares](../api/shares-get.md). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="623ef-p108">A unique token that can be used to access this shared item via the [**shares** API](../api/shares-get.md). Read-only.</span></span>

<span data-ttu-id="623ef-142">O recurso permission usa _facetas_ para fornecer informações sobre o tipo de permissão representado pelo recurso.</span><span class="sxs-lookup"><span data-stu-id="623ef-142">The permission resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="623ef-p109">Permissões com uma faceta [**link**][SharingLink] representam links de compartilhamento criados no item. Os links de compartilhamento contêm um token exclusivo que fornece acesso ao item para qualquer pessoa com o link.</span><span class="sxs-lookup"><span data-stu-id="623ef-p109">Permissions with a [**link**][SharingLink] facet represent sharing links created on the item. Sharing links contain a unique token that provides access to the item for anyone with the link.</span></span>

<span data-ttu-id="623ef-145">Permissões com uma faceta [**invitation**][SharingInvitation] representam permissões adicionadas convidando usuários ou grupos específicos para ter acesso ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="623ef-145">Permissions with an [**invitation**][SharingInvitation] facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

[SharingInvitation]: sharinginvitation.md
[SharingLink]: sharinglink.md

## <a name="roles-enumeration"></a><span data-ttu-id="623ef-148">Enumeração de funções</span><span class="sxs-lookup"><span data-stu-id="623ef-148">Roles enumeration</span></span>

| <span data-ttu-id="623ef-149">Função</span><span class="sxs-lookup"><span data-stu-id="623ef-149">Role</span></span>        | <span data-ttu-id="623ef-150">Detalhes</span><span class="sxs-lookup"><span data-stu-id="623ef-150">Details</span></span>                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | <span data-ttu-id="623ef-151">Fornece a capacidade de ler os metadados e o conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="623ef-151">Provides the ability to read the metadata and contents of the item.</span></span>            |
| `write`     | <span data-ttu-id="623ef-152">Fornece a capacidade de ler e modificar os metadados e o conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="623ef-152">Provides the ability to read and modify the metadata and contents of the item.</span></span> |
| `sp.owner`  | <span data-ttu-id="623ef-153">Para o SharePoint e o OneDrive for Business, isso representa a função de proprietário.</span><span class="sxs-lookup"><span data-stu-id="623ef-153">For SharePoint and OneDrive for Business this represents the owner role.</span></span>       |
| `sp.member` | <span data-ttu-id="623ef-154">Para o SharePoint e o OneDrive for Business, isso representa a função de membro.</span><span class="sxs-lookup"><span data-stu-id="623ef-154">For SharePoint and OneDrive for Business this represents the member role.</span></span>      |

## <a name="sharing-links"></a><span data-ttu-id="623ef-155">Links de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="623ef-155">Sharing links</span></span>
<span data-ttu-id="623ef-p110">O tipo mais comum de permissões são os links de compartilhamento. Esses links fornecem uma URL exclusiva que inclui o recurso que está sendo compartilhado e um token de autenticação que fornece acesso ao recurso. Os usuários não precisam entrar para acessar o conteúdo compartilhado com um link de compartilhamento. Os usuários podem compartilhar um link que concede acesso somente leitura ou acesso de gravação ao conteúdo.</span><span class="sxs-lookup"><span data-stu-id="623ef-p110">The most common type of permissions are sharing links. Sharing links provide a unique URL that includes both the resource being shared and an authentication token that provides access to the resource. Users don't need to sign-in to access the content shared with a sharing link. Users can share a link that gives read-only access to the content or writable access to the content.</span></span>

### <a name="view-link"></a><span data-ttu-id="623ef-160">Link de exibição</span><span class="sxs-lookup"><span data-stu-id="623ef-160">View Link</span></span>
<span data-ttu-id="623ef-161">Um link de exibição oferece acesso somente leitura a um item.</span><span class="sxs-lookup"><span data-stu-id="623ef-161">A view link provides read-only access to an item.</span></span>

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-view-link" } -->
```json
{
  "id": "1",
  "roles": ["read"],
  "link": {
    "type": "view",
    "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
    "application": { "id": "1234", "displayName": "Sample Application" }
  },
  "shareId": "!LKj1lkdlals90j1nlkascl"
}
```

### <a name="edit-link"></a><span data-ttu-id="623ef-162">Link de edição</span><span class="sxs-lookup"><span data-stu-id="623ef-162">Edit link</span></span>
<span data-ttu-id="623ef-163">Um link de edição fornece acesso de leitura e gravação a um item.</span><span class="sxs-lookup"><span data-stu-id="623ef-163">An edit link provides read and write access to an item.</span></span>

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-edit-link" } -->
```json
{
  "id": "2",
  "roles": ["write"],
  "link": {
    "type": "edit",
    "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
    "application": { "id": "1234", "displayName": "Sample Application" }
  },
  "shareId": "!LKj1lkdlals90j1nlkascl"
}
```

### <a name="sharing-invitation"></a><span data-ttu-id="623ef-164">Convite de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="623ef-164">Sharing Invitation</span></span>
<span data-ttu-id="623ef-p111">Além de criar links de compartilhamento, um usuário pode ser convidado pelo endereço de email. Nesse cenário, a permissão cria um convite que é enviado ao email do usuário.</span><span class="sxs-lookup"><span data-stu-id="623ef-p111">In addition to creating sharing links, a user can be invited by e-mail address. In this scenario the permission creates an invitation that is sent to the user's email.</span></span>

#### <a name="invitation-to-an-email-address"></a><span data-ttu-id="623ef-167">Convite para um endereço de email</span><span class="sxs-lookup"><span data-stu-id="623ef-167">Invitation to an email address</span></span>
<span data-ttu-id="623ef-168">Se a permissão for enviada por meio do endereço de email para um destinatário que não tem uma conta correspondente, a propriedade **grantedTo** não poderá ser definida até que o convite seja resgatado, o que ocorre na primeira vez que um usuário clica no link e entra na sessão.</span><span class="sxs-lookup"><span data-stu-id="623ef-168">If the permission was sent via an email address to a recipient who does not have a matching account, the **grantedTo** property may not be set until the invitation is redeemed, which occurs the first time a user clicks the link and signs in.</span></span>

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-invite-email" } -->
```json
{
  "id": "1",
  "roles": ["write"],
  "invitation": {
    "email": "jd@gmail.com",
    "signInRequired": true
  },
  "shareId": "FWxc1lasfdbEAGM5fI7B67aB5ZMPDMmQ11U"
}
```

<span data-ttu-id="623ef-169">Depois que o convite de compartilhamento tiver sido resgatado por um usuário, a propriedade **grantedTo** conterá as informações sobre a conta que resgatou as permissões:</span><span class="sxs-lookup"><span data-stu-id="623ef-169">After the sharing invitation has been redeemed by a user, the **grantedTo** property will contain the information about the account that redeemed the permissions:</span></span>

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-invite-redeemed" } -->
```json
{
  "id": "1",
  "roles": ["write"],
  "grantedTo": {
    "user": {
      "id": "5D33DD65C6932946",
      "displayName": "John Doe"
    }
  },
  "invitation": {
    "email": "jd@outlook.com",
    "signInRequired": true
  },
  "shareId": "FWxc1lasfdbEAGM5fI7B67aB5ZMPDMmQ11U"
}
```

## <a name="methods"></a><span data-ttu-id="623ef-170">Métodos</span><span class="sxs-lookup"><span data-stu-id="623ef-170">Methods</span></span>

| <span data-ttu-id="623ef-171">Método</span><span class="sxs-lookup"><span data-stu-id="623ef-171">Method</span></span>                                                   | <span data-ttu-id="623ef-172">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="623ef-172">REST Path</span></span>
|:---------------------------------------------------------|:-----------------------
| [<span data-ttu-id="623ef-173">Listar permissões</span><span class="sxs-lookup"><span data-stu-id="623ef-173">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="623ef-174">Obter permissão</span><span class="sxs-lookup"><span data-stu-id="623ef-174">Get permission</span></span>](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="623ef-175">Adicionar</span><span class="sxs-lookup"><span data-stu-id="623ef-175">Add</span></span>](../api/driveitem-invite.md)                        | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="623ef-176">Update</span><span class="sxs-lookup"><span data-stu-id="623ef-176">Update</span></span>](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="623ef-177">Delete</span><span class="sxs-lookup"><span data-stu-id="623ef-177">Delete</span></span>](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`


## <a name="remarks"></a><span data-ttu-id="623ef-178">Comentários</span><span class="sxs-lookup"><span data-stu-id="623ef-178">Remarks</span></span>

<span data-ttu-id="623ef-179">O OneDrive for Business e as bibliotecas de documentos do SharePoint não retornam a propriedade **inheritedFrom**.</span><span class="sxs-lookup"><span data-stu-id="623ef-179">OneDrive for Business and SharePoint document libraries do not return the **inheritedFrom** property.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The permission object provides information about permissions and roles and sharing information.",
  "keywords": "sharing,permissions,read,write,acl",
  "section": "documentation",
  "tocPath": "Resources/Permission"
} -->
