---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Permissão
localization_priority: Priority
description: O recurso Permission fornece informações sobre uma permissão de compartilhamento concedida a um recurso DriveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5c4b881aaf10a56b65342dccebd417867c2b7b26
ms.sourcegitcommit: 9b507499fb1ec61b4de47f36f915ae29c8594459
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2020
ms.locfileid: "43934700"
---
# <a name="permission-resource-type"></a><span data-ttu-id="c0707-103">Tipo de recurso permission</span><span class="sxs-lookup"><span data-stu-id="c0707-103">Permission resource type</span></span>

<span data-ttu-id="c0707-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0707-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c0707-105">O recurso **Permission** fornece informações sobre uma permissão de compartilhamento concedida a um recurso [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="c0707-105">The **Permission** resource provides information about a sharing permission granted for a [DriveItem](driveitem.md) resource.</span></span>

<span data-ttu-id="c0707-106">As permissões de compartilhamento têm várias formas diferentes.</span><span class="sxs-lookup"><span data-stu-id="c0707-106">Sharing permissions have a number of different forms.</span></span>
<span data-ttu-id="c0707-107">O recurso **Permission** representa estes diferentes formulários por meio de facetas do recurso.</span><span class="sxs-lookup"><span data-stu-id="c0707-107">The **Permission** resource represents these different forms through facets on the resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0707-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c0707-108">JSON representation</span></span>

<span data-ttu-id="c0707-109">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="c0707-109">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "link",
    "grantedTo",
    "grantedToIdentities",
    "invitation",
    "inheritedFrom",
    "shareId",
    "expirationDateTime",
    "hasPassword"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.permission"
}-->
```json
{
  "id": "string (identifier)",
  "grantedTo": {"@odata.type": "microsoft.graph.identitySet"},
  "grantedToIdentities": [{"@odata.type": "microsoft.graph.identitySet"}],
  "inheritedFrom": {"@odata.type": "microsoft.graph.itemReference"},
  "invitation": {"@odata.type": "microsoft.graph.sharingInvitation"},
  "link": {"@odata.type": "microsoft.graph.sharingLink"},
  "roles": ["string"],
  "shareId": "string",
  "expirationDateTime": "string (timestamp)",
  "hasPassword": "boolean"
}
```

## <a name="properties"></a><span data-ttu-id="c0707-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c0707-110">Properties</span></span>

| <span data-ttu-id="c0707-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0707-111">Property</span></span>      | <span data-ttu-id="c0707-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0707-112">Type</span></span>                                      | <span data-ttu-id="c0707-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0707-113">Description</span></span>
|:--------------|:------------------------------------------|:-----------------
| <span data-ttu-id="c0707-114">id</span><span class="sxs-lookup"><span data-stu-id="c0707-114">id</span></span>            | <span data-ttu-id="c0707-115">String</span><span class="sxs-lookup"><span data-stu-id="c0707-115">String</span></span>                                    | <span data-ttu-id="c0707-p102">O identificador exclusivo da permissão entre todas as permissões no item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c0707-p102">The unique identifier of the permission among all permissions on the item. Read-only.</span></span>
| <span data-ttu-id="c0707-118">grantedTo</span><span class="sxs-lookup"><span data-stu-id="c0707-118">grantedTo</span></span>     | [<span data-ttu-id="c0707-119">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="c0707-119">IdentitySet</span></span>](identityset.md)             | <span data-ttu-id="c0707-p103">Para permissões de tipo de usuário, os detalhes de usuários e aplicativos para esta permissão. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c0707-p103">For user type permissions, the details of the users & applications for this permission. Read-only.</span></span>
| <span data-ttu-id="c0707-122">grantedToIdentities</span><span class="sxs-lookup"><span data-stu-id="c0707-122">grantedToIdentities</span></span> | <span data-ttu-id="c0707-123">Coleção([IdentitySet](identityset.md))</span><span class="sxs-lookup"><span data-stu-id="c0707-123">Collection([IdentitySet](identityset.md))</span></span> | <span data-ttu-id="c0707-124">Para permissões de tipo de link, os detalhes dos usuários aos quais a permissão foi concedida.</span><span class="sxs-lookup"><span data-stu-id="c0707-124">For link type permissions, the details of the users to whom permission was granted.</span></span> <span data-ttu-id="c0707-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c0707-125">Read-only.</span></span>
| <span data-ttu-id="c0707-126">invitation</span><span class="sxs-lookup"><span data-stu-id="c0707-126">invitation</span></span>    | <span data-ttu-id="c0707-127">[SharingInvitation][]</span><span class="sxs-lookup"><span data-stu-id="c0707-127">[SharingInvitation][]</span></span>                     | <span data-ttu-id="c0707-p105">Detalhes de um convite de compartilhamento associado para esta permissão. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c0707-p105">Details of any associated sharing invitation for this permission. Read-only.</span></span>
| <span data-ttu-id="c0707-130">inheritedFrom</span><span class="sxs-lookup"><span data-stu-id="c0707-130">inheritedFrom</span></span> | [<span data-ttu-id="c0707-131">ItemReference</span><span class="sxs-lookup"><span data-stu-id="c0707-131">ItemReference</span></span>](itemreference.md)         | <span data-ttu-id="c0707-p106">Fornece uma referência para o ancestral da permissão atual, se ela for herdada de um ancestral. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c0707-p106">Provides a reference to the ancestor of the current permission, if it is inherited from an ancestor. Read-only.</span></span>
| <span data-ttu-id="c0707-134">vínculo</span><span class="sxs-lookup"><span data-stu-id="c0707-134">link</span></span>          | <span data-ttu-id="c0707-135">[SharingLink][]</span><span class="sxs-lookup"><span data-stu-id="c0707-135">[SharingLink][]</span></span>                           | <span data-ttu-id="c0707-p107">Fornece os detalhes do link de permissão atual, caso se trate de permissões de tipo de link. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c0707-p107">Provides the link details of the current permission, if it is a link type permissions. Read-only.</span></span>
| <span data-ttu-id="c0707-138">funções</span><span class="sxs-lookup"><span data-stu-id="c0707-138">roles</span></span>         | <span data-ttu-id="c0707-139">Coleção de Cadeias de Caracteres</span><span class="sxs-lookup"><span data-stu-id="c0707-139">Collection of String</span></span>                      | <span data-ttu-id="c0707-p108">O tipo de permissão, por exemplo, `read`. Veja abaixo a lista completa de funções. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c0707-p108">The type of permission, e.g. `read`. See below for the full list of roles. Read-only.</span></span>
| <span data-ttu-id="c0707-143">shareId</span><span class="sxs-lookup"><span data-stu-id="c0707-143">shareId</span></span>       | <span data-ttu-id="c0707-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c0707-144">String</span></span>                                    | <span data-ttu-id="c0707-p109">Um token exclusivo que pode ser usado para acessar esse item compartilhado por meio da [**API** Shares](../api/shares-get.md). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c0707-p109">A unique token that can be used to access this shared item via the [**shares** API](../api/shares-get.md). Read-only.</span></span>
| <span data-ttu-id="c0707-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c0707-147">expirationDateTime</span></span>  | <span data-ttu-id="c0707-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0707-148">DateTimeOffset</span></span>              | <span data-ttu-id="c0707-149">Um formato yyyy-MM-ddTHH:mm:ssZ de DateTimeOffset indica o tempo de expiração da permissão.</span><span class="sxs-lookup"><span data-stu-id="c0707-149">A format of yyyy-MM-ddTHH:mm:ssZ of DateTimeOffset indicates the expiration time of the permission.</span></span> <span data-ttu-id="c0707-150">DateTime.MinValue indica que não há expiração definida para esta permissão.</span><span class="sxs-lookup"><span data-stu-id="c0707-150">DateTime.MinValue indicates there is no expiration set for this permission.</span></span> <span data-ttu-id="c0707-151">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c0707-151">Optional.</span></span>
| <span data-ttu-id="c0707-152">hasPassword</span><span class="sxs-lookup"><span data-stu-id="c0707-152">hasPassword</span></span>         | <span data-ttu-id="c0707-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0707-153">Boolean</span></span>                     | <span data-ttu-id="c0707-154">Isso indica se a senha está configurada para esta permissão, está sendo exibida apenas em resposta.</span><span class="sxs-lookup"><span data-stu-id="c0707-154">This indicates whether password is set for this permission, it's only showing in response.</span></span> <span data-ttu-id="c0707-155">Opcional e Somente leitura e somente para o OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="c0707-155">Optional and Read-only and for OneDrive Personal only.</span></span>

<span data-ttu-id="c0707-156">O recurso permission usa _facetas_ para fornecer informações sobre o tipo de permissão representado pelo recurso.</span><span class="sxs-lookup"><span data-stu-id="c0707-156">The permission resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="c0707-p112">Permissões com uma faceta [**link**][SharingLink] representam links de compartilhamento criados no item. Os links de compartilhamento contêm um token exclusivo que fornece acesso ao item para qualquer pessoa com o link.</span><span class="sxs-lookup"><span data-stu-id="c0707-p112">Permissions with a [**link**][SharingLink] facet represent sharing links created on the item. Sharing links contain a unique token that provides access to the item for anyone with the link.</span></span>

<span data-ttu-id="c0707-159">Permissões com uma faceta [**invitation**][SharingInvitation] representam permissões adicionadas convidando usuários ou grupos específicos para ter acesso ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="c0707-159">Permissions with an [**invitation**][SharingInvitation] facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

[SharingInvitation]: sharinginvitation.md
[SharingLink]: sharinglink.md

### <a name="roles-property-values"></a><span data-ttu-id="c0707-162">Valores de propriedades Roles</span><span class="sxs-lookup"><span data-stu-id="c0707-162">Roles property values</span></span>

| <span data-ttu-id="c0707-163">Função</span><span class="sxs-lookup"><span data-stu-id="c0707-163">Role</span></span>        | <span data-ttu-id="c0707-164">Detalhes</span><span class="sxs-lookup"><span data-stu-id="c0707-164">Details</span></span>                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | <span data-ttu-id="c0707-165">Fornece a capacidade de ler os metadados e o conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="c0707-165">Provides the ability to read the metadata and contents of the item.</span></span>            |
| `write`     | <span data-ttu-id="c0707-166">Fornece a capacidade de ler e modificar os metadados e o conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="c0707-166">Provides the ability to read and modify the metadata and contents of the item.</span></span> |
| `sp.owner`  | <span data-ttu-id="c0707-167">Para o SharePoint e o OneDrive for Business, isso representa a função de proprietário.</span><span class="sxs-lookup"><span data-stu-id="c0707-167">For SharePoint and OneDrive for Business this represents the owner role.</span></span>       |
| `sp.member` | <span data-ttu-id="c0707-168">Para o SharePoint e o OneDrive for Business, isso representa a função de membro.</span><span class="sxs-lookup"><span data-stu-id="c0707-168">For SharePoint and OneDrive for Business this represents the member role.</span></span>      |

## <a name="sharing-links"></a><span data-ttu-id="c0707-169">Links de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="c0707-169">Sharing links</span></span>
<span data-ttu-id="c0707-p113">O tipo mais comum de permissões são os links de compartilhamento. Esses links fornecem uma URL exclusiva que inclui o recurso que está sendo compartilhado e um token de autenticação que fornece acesso ao recurso. Os usuários não precisam entrar para acessar o conteúdo compartilhado com um link de compartilhamento. Os usuários podem compartilhar um link que concede acesso somente leitura ou acesso de gravação ao conteúdo.</span><span class="sxs-lookup"><span data-stu-id="c0707-p113">The most common type of permissions are sharing links. Sharing links provide a unique URL that includes both the resource being shared and an authentication token that provides access to the resource. Users don't need to sign-in to access the content shared with a sharing link. Users can share a link that gives read-only access to the content or writable access to the content.</span></span>

### <a name="view-link"></a><span data-ttu-id="c0707-174">Link de exibição</span><span class="sxs-lookup"><span data-stu-id="c0707-174">View Link</span></span>
<span data-ttu-id="c0707-175">Um link de exibição oferece acesso somente leitura a um item.</span><span class="sxs-lookup"><span data-stu-id="c0707-175">A view link provides read-only access to an item.</span></span>

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
  "shareId": "!LKj1lkdlals90j1nlkascl",
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

### <a name="edit-link"></a><span data-ttu-id="c0707-176">Link de edição</span><span class="sxs-lookup"><span data-stu-id="c0707-176">Edit link</span></span>
<span data-ttu-id="c0707-177">Um link de edição fornece acesso de leitura e gravação a um item.</span><span class="sxs-lookup"><span data-stu-id="c0707-177">An edit link provides read and write access to an item.</span></span>

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
  "shareId": "!LKj1lkdlals90j1nlkascl",
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```
### <a name="specific-people-link"></a><span data-ttu-id="c0707-178">Link de pessoas específicas</span><span class="sxs-lookup"><span data-stu-id="c0707-178">Specific people link</span></span>

<span data-ttu-id="c0707-179">Este link fornece acesso de leitura e gravação para as pessoas específicas na coleção `grantedToIdentities`.</span><span class="sxs-lookup"><span data-stu-id="c0707-179">This link provides read and write access to the specific people in the `grantedToIdentities` collection.</span></span>

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-people-link" } -->

```json
{
  "id": "3",
  "grantedToIdentities": [
    {
       "user": {
        "id": "35fij1974gb8832",
        "displayName": "Misty Suarez"
      }
    },
    {
       "user": {
        "id": "9397721fh4hgh73",
        "displayName": "Judith Clemons"
      }
    }
  ],
  "roles": ["write"],
  "link": {
    "webUrl": "https://contoso.sharepoint.com/:w:/t/design/a577ghg9hgh737613bmbjf839026561fmzhsr85ng9f3hjck2t5s",
    "application": { "id": "1234", "displayName": "Sample Application" }
  },
  "shareId": "!LKj1lkdlals90j1nlkascl",
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

### <a name="existing-access-link"></a><span data-ttu-id="c0707-180">Link de acesso existente</span><span class="sxs-lookup"><span data-stu-id="c0707-180">Existing access link</span></span>

<span data-ttu-id="c0707-181">Este link não concede privilégios adicionais ao usuário.</span><span class="sxs-lookup"><span data-stu-id="c0707-181">This link does not grant any additional privileges to the user.</span></span>

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-existing-link" } -->

```json
{
  "id": "00000000-0000-0000-0000-000000000000",
  "roles": ["read"],
  "link": {
    "scope": "existingAccess",
    "type": "view",
    "webUrl": "https://contoso.sharepoint.com/:w:/t/design/Shared%20Documents/SampleDoc.docx?d=w12345",
  },
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

### <a name="sharing-invitation"></a><span data-ttu-id="c0707-182">Convite de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="c0707-182">Sharing Invitation</span></span>
<span data-ttu-id="c0707-p114">Além de criar links de compartilhamento, um usuário pode ser convidado pelo endereço de email. Nesse cenário, a permissão cria um convite que é enviado ao email do usuário.</span><span class="sxs-lookup"><span data-stu-id="c0707-p114">In addition to creating sharing links, a user can be invited by e-mail address. In this scenario the permission creates an invitation that is sent to the user's email.</span></span>

#### <a name="invitation-to-an-email-address"></a><span data-ttu-id="c0707-185">Convite para um endereço de email</span><span class="sxs-lookup"><span data-stu-id="c0707-185">Invitation to an email address</span></span>
<span data-ttu-id="c0707-186">Se a permissão for enviada por meio do endereço de email para um destinatário que não tem uma conta correspondente, a propriedade **grantedTo** não poderá ser definida até que o convite seja resgatado, o que ocorre na primeira vez que um usuário clica no link e entra na sessão.</span><span class="sxs-lookup"><span data-stu-id="c0707-186">If the permission was sent via an email address to a recipient who does not have a matching account, the **grantedTo** property may not be set until the invitation is redeemed, which occurs the first time a user clicks the link and signs in.</span></span>

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-invite-email" } -->
```json
{
  "id": "1",
  "roles": ["write"],
  "invitation": {
    "email": "jd@gmail.com",
    "signInRequired": true
  },
  "shareId": "FWxc1lasfdbEAGM5fI7B67aB5ZMPDMmQ11U",
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

<span data-ttu-id="c0707-187">Depois que o convite de compartilhamento tiver sido resgatado por um usuário, a propriedade **grantedTo** conterá as informações sobre a conta que resgatou as permissões:</span><span class="sxs-lookup"><span data-stu-id="c0707-187">After the sharing invitation has been redeemed by a user, the **grantedTo** property will contain the information about the account that redeemed the permissions:</span></span>

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
  "shareId": "FWxc1lasfdbEAGM5fI7B67aB5ZMPDMmQ11U",
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

## <a name="methods"></a><span data-ttu-id="c0707-188">Métodos</span><span class="sxs-lookup"><span data-stu-id="c0707-188">Methods</span></span>

| <span data-ttu-id="c0707-189">Método</span><span class="sxs-lookup"><span data-stu-id="c0707-189">Method</span></span>                                                   | <span data-ttu-id="c0707-190">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="c0707-190">REST Path</span></span>
|:---------------------------------------------------------|:-----------------------
| [<span data-ttu-id="c0707-191">Listar permissões</span><span class="sxs-lookup"><span data-stu-id="c0707-191">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="c0707-192">Obter permissão</span><span class="sxs-lookup"><span data-stu-id="c0707-192">Get permission</span></span>](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="c0707-193">Adicionar</span><span class="sxs-lookup"><span data-stu-id="c0707-193">Add</span></span>](../api/driveitem-invite.md)                        | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="c0707-194">Update</span><span class="sxs-lookup"><span data-stu-id="c0707-194">Update</span></span>](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="c0707-195">Delete</span><span class="sxs-lookup"><span data-stu-id="c0707-195">Delete</span></span>](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="c0707-196">Adicionar usuários ao link de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="c0707-196">Add users to sharing link</span></span>](../api/permission-grant.md)  | `POST /shares/{encoded-sharing-url}/permission/grant`


## <a name="remarks"></a><span data-ttu-id="c0707-197">Comentários</span><span class="sxs-lookup"><span data-stu-id="c0707-197">Remarks</span></span>

<span data-ttu-id="c0707-198">O OneDrive for Business e as bibliotecas de documentos do SharePoint não retornam a propriedade **inheritedFrom**.</span><span class="sxs-lookup"><span data-stu-id="c0707-198">OneDrive for Business and SharePoint document libraries do not return the **inheritedFrom** property.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The permission object provides information about permissions and roles and sharing information.",
  "keywords": "sharing,permissions,read,write,acl",
  "section": "documentation",
  "tocPath": "Resources/Permission"
} -->
