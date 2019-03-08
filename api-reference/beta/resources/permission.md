---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Permissão
localization_priority: Normal
ms.openlocfilehash: 12390583dcb1a87a5c9492ae3dcbcb132a66f69c
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482074"
---
# <a name="permission-resource-type"></a><span data-ttu-id="d54b5-102">tipo de recurso Permission</span><span class="sxs-lookup"><span data-stu-id="d54b5-102">permission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d54b5-103">O recurso **Permission** fornece informações sobre uma permissão de compartilhamento concedida para um recurso [driveItem](driveitem.md) .</span><span class="sxs-lookup"><span data-stu-id="d54b5-103">The **permission** resource provides information about a sharing permission granted for a [driveItem](driveitem.md) resource.</span></span>

<span data-ttu-id="d54b5-104">As permissões de compartilhamento têm várias formas diferentes.</span><span class="sxs-lookup"><span data-stu-id="d54b5-104">Sharing permissions have a number of different forms.</span></span>
<span data-ttu-id="d54b5-105">O recurso **Permission** representa esses diferentes formatos através de facetas no recurso.</span><span class="sxs-lookup"><span data-stu-id="d54b5-105">The **permission** resource represents these different forms through facets on the resource.</span></span>

><span data-ttu-id="d54b5-106">**Observação:** As bibliotecas de documentos do OneDrive for Business e do SharePoint não retornam a propriedade **inheritedFrom** .</span><span class="sxs-lookup"><span data-stu-id="d54b5-106">**Note:** OneDrive for Business and SharePoint document libraries do not return the **inheritedFrom** property.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d54b5-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d54b5-107">JSON representation</span></span>

<span data-ttu-id="d54b5-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d54b5-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="d54b5-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d54b5-109">Properties</span></span>

| <span data-ttu-id="d54b5-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d54b5-110">Property</span></span>            | <span data-ttu-id="d54b5-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d54b5-111">Type</span></span>                        | <span data-ttu-id="d54b5-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d54b5-112">Description</span></span>
|:--------------------|:----------------------------|:-------------------------
| <span data-ttu-id="d54b5-113">id</span><span class="sxs-lookup"><span data-stu-id="d54b5-113">id</span></span>                  | <span data-ttu-id="d54b5-114">String</span><span class="sxs-lookup"><span data-stu-id="d54b5-114">String</span></span>                      | <span data-ttu-id="d54b5-p102">O identificador exclusivo da permissão entre todas as permissões no item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d54b5-p102">The unique identifier of the permission among all permissions on the item. Read-only.</span></span>
| <span data-ttu-id="d54b5-117">grantedTo</span><span class="sxs-lookup"><span data-stu-id="d54b5-117">grantedTo</span></span>           | <span data-ttu-id="d54b5-118">[IdentitySet][]</span><span class="sxs-lookup"><span data-stu-id="d54b5-118">[IdentitySet][]</span></span>             | <span data-ttu-id="d54b5-p103">Para permissões de tipo de usuário, os detalhes de usuários e aplicativos para esta permissão. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d54b5-p103">For user type permissions, the details of the users & applications for this permission. Read-only.</span></span>
| <span data-ttu-id="d54b5-121">grantedToIdentities</span><span class="sxs-lookup"><span data-stu-id="d54b5-121">grantedToIdentities</span></span> | <span data-ttu-id="d54b5-122">Coleção ([identityset][])</span><span class="sxs-lookup"><span data-stu-id="d54b5-122">Collection([IdentitySet][])</span></span> | <span data-ttu-id="d54b5-123">Para permissões de tipo de link, os detalhes dos usuários aos quais a permissão foi concedida.</span><span class="sxs-lookup"><span data-stu-id="d54b5-123">For link type permissions, the details of the users to whom permission was granted.</span></span> <span data-ttu-id="d54b5-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d54b5-124">Read-only.</span></span>
| <span data-ttu-id="d54b5-125">invitation</span><span class="sxs-lookup"><span data-stu-id="d54b5-125">invitation</span></span>          | <span data-ttu-id="d54b5-126">[SharingInvitation][]</span><span class="sxs-lookup"><span data-stu-id="d54b5-126">[SharingInvitation][]</span></span>       | <span data-ttu-id="d54b5-p105">Detalhes de um convite de compartilhamento associado para esta permissão. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d54b5-p105">Details of any associated sharing invitation for this permission. Read-only.</span></span>
| <span data-ttu-id="d54b5-129">inheritedFrom</span><span class="sxs-lookup"><span data-stu-id="d54b5-129">inheritedFrom</span></span>       | <span data-ttu-id="d54b5-130">[ItemReference][]</span><span class="sxs-lookup"><span data-stu-id="d54b5-130">[ItemReference][]</span></span>           | <span data-ttu-id="d54b5-p106">Fornece uma referência para o ancestral da permissão atual, se ela for herdada de um ancestral. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d54b5-p106">Provides a reference to the ancestor of the current permission, if it is inherited from an ancestor. Read-only.</span></span>
| <span data-ttu-id="d54b5-133">link</span><span class="sxs-lookup"><span data-stu-id="d54b5-133">link</span></span>                | <span data-ttu-id="d54b5-134">[SharingLink][]</span><span class="sxs-lookup"><span data-stu-id="d54b5-134">[SharingLink][]</span></span>             | <span data-ttu-id="d54b5-p107">Fornece os detalhes do link de permissão atual, caso se trate de permissões de tipo de link. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d54b5-p107">Provides the link details of the current permission, if it is a link type permissions. Read-only.</span></span>
| <span data-ttu-id="d54b5-137">funções</span><span class="sxs-lookup"><span data-stu-id="d54b5-137">roles</span></span>               | <span data-ttu-id="d54b5-138">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="d54b5-138">Collection(String)</span></span>          | <span data-ttu-id="d54b5-p108">O tipo de permissão, por exemplo, `read`. Veja abaixo a lista completa de funções. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d54b5-p108">The type of permission, e.g. `read`. See below for the full list of roles. Read-only.</span></span>
| <span data-ttu-id="d54b5-142">shareId</span><span class="sxs-lookup"><span data-stu-id="d54b5-142">shareId</span></span>             | <span data-ttu-id="d54b5-143">String</span><span class="sxs-lookup"><span data-stu-id="d54b5-143">String</span></span>                      | <span data-ttu-id="d54b5-144">Um token exclusivo que pode ser usado para acessar esse item compartilhado por meio da **[API][]** de compartilhamentos.</span><span class="sxs-lookup"><span data-stu-id="d54b5-144">A unique token that can be used to access this shared item via the **[shares API][]**.</span></span> <span data-ttu-id="d54b5-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d54b5-145">Read-only.</span></span>
| <span data-ttu-id="d54b5-146">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d54b5-146">expirationDateTime</span></span>  | <span data-ttu-id="d54b5-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d54b5-147">DateTimeOffset</span></span>              | <span data-ttu-id="d54b5-148">Um formato de yyyy-MM-ddTHH: mm: ssZ de DateTimeOffset indica o tempo de expiração da permissão.</span><span class="sxs-lookup"><span data-stu-id="d54b5-148">A format of yyyy-MM-ddTHH:mm:ssZ of DateTimeOffset indicates the expiration time of the permission.</span></span> <span data-ttu-id="d54b5-149">DateTime. MinValue indica que não há validade configurada para essa permissão.</span><span class="sxs-lookup"><span data-stu-id="d54b5-149">DateTime.MinValue indicates there is no expiration set for this permission.</span></span> <span data-ttu-id="d54b5-150">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d54b5-150">Optional.</span></span>
| <span data-ttu-id="d54b5-151">hasPassword</span><span class="sxs-lookup"><span data-stu-id="d54b5-151">hasPassword</span></span>         | <span data-ttu-id="d54b5-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="d54b5-152">Boolean</span></span>                     | <span data-ttu-id="d54b5-153">Isso indica se a senha está definida para essa permissão, ela só será mostrada em resposta.</span><span class="sxs-lookup"><span data-stu-id="d54b5-153">This indicates whether password is set for this permission, it's only showing in response.</span></span> <span data-ttu-id="d54b5-154">Opcional e somente leitura e somente para o OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="d54b5-154">Optional and Read-only and for OneDrive Personal only.</span></span>

### <a name="roles-enumeration-values"></a><span data-ttu-id="d54b5-155">Valores de enumeração de funções</span><span class="sxs-lookup"><span data-stu-id="d54b5-155">Roles enumeration values</span></span>

| <span data-ttu-id="d54b5-156">Valor</span><span class="sxs-lookup"><span data-stu-id="d54b5-156">Value</span></span>        | <span data-ttu-id="d54b5-157">Detalhes</span><span class="sxs-lookup"><span data-stu-id="d54b5-157">Details</span></span>                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | <span data-ttu-id="d54b5-158">Fornece a capacidade de ler os metadados e o conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="d54b5-158">Provides the ability to read the metadata and contents of the item.</span></span>            |
| `write`     | <span data-ttu-id="d54b5-159">Fornece a capacidade de ler e modificar os metadados e o conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="d54b5-159">Provides the ability to read and modify the metadata and contents of the item.</span></span> |
| `sp.owner`  | <span data-ttu-id="d54b5-160">Para o SharePoint e o OneDrive for Business, isso representa a função de proprietário.</span><span class="sxs-lookup"><span data-stu-id="d54b5-160">For SharePoint and OneDrive for Business this represents the owner role.</span></span>       |
| `sp.member` | <span data-ttu-id="d54b5-161">Para o SharePoint e o OneDrive for Business, isso representa a função de membro.</span><span class="sxs-lookup"><span data-stu-id="d54b5-161">For SharePoint and OneDrive for Business this represents the member role.</span></span>      |

<span data-ttu-id="d54b5-162">O recurso permission usa _facetas_ para fornecer informações sobre o tipo de permissão representado pelo recurso.</span><span class="sxs-lookup"><span data-stu-id="d54b5-162">The permission resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="d54b5-163">Links de compartilhamento contêm um token exclusivo necessário para acessar o item.</span><span class="sxs-lookup"><span data-stu-id="d54b5-163">Sharing links contain a unique token required to access the item.</span></span>

<span data-ttu-id="d54b5-164">Permissões com uma faceta [**invitation**][SharingInvitation] representam permissões adicionadas convidando usuários ou grupos específicos para ter acesso ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="d54b5-164">Permissions with an [**invitation**][SharingInvitation] facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

## <a name="sharing-links"></a><span data-ttu-id="d54b5-165">Links de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="d54b5-165">Sharing links</span></span>

<span data-ttu-id="d54b5-166">Permissões com uma faceta [**link**][SharingLink] representam links de compartilhamento criados no item.</span><span class="sxs-lookup"><span data-stu-id="d54b5-166">Permissions with a [**link**][SharingLink] facet represent sharing links created on the item.</span></span>
<span data-ttu-id="d54b5-167">Estes são os tipos de permissões mais comuns.</span><span class="sxs-lookup"><span data-stu-id="d54b5-167">These are the most common kinds of permissions.</span></span>
<span data-ttu-id="d54b5-168">Links de compartilhamento fornecem uma URL exclusiva que pode ser usada para acessar um arquivo ou uma pasta.</span><span class="sxs-lookup"><span data-stu-id="d54b5-168">Sharing links provide a unique URL that can be used to access a file or folder.</span></span>
<span data-ttu-id="d54b5-169">Eles podem ser configurados para conceder acesso de várias maneiras.</span><span class="sxs-lookup"><span data-stu-id="d54b5-169">They can be set up to grant access in a variety of ways.</span></span>
<span data-ttu-id="d54b5-170">Por exemplo, você pode usar a [][] API CreateLink para criar um link que funcione para qualquer pessoa que se inscreveu em sua organização ou pode criar um link que funcione para qualquer pessoa, sem precisar entrar.</span><span class="sxs-lookup"><span data-stu-id="d54b5-170">For example, you can use the [createLink][] API to create a link that works for anyone signed into your organization, or you can create a link that works for anyone, without needing to sign in.</span></span>
<span data-ttu-id="d54b5-171">Você pode usar a API [INVITE][] para criar um link que funciona apenas para pessoas específicas, seja em sua empresa ou não.</span><span class="sxs-lookup"><span data-stu-id="d54b5-171">You can use the [invite][] API to create a link that only works for specific people, whether they're in your company or not.</span></span>

<span data-ttu-id="d54b5-172">Aqui estão alguns exemplos de links de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="d54b5-172">Here are some examples of sharing links.</span></span>

### <a name="view-link"></a><span data-ttu-id="d54b5-173">Link de exibição</span><span class="sxs-lookup"><span data-stu-id="d54b5-173">View link</span></span>

<span data-ttu-id="d54b5-174">Este link de exibição fornece acesso somente leitura a qualquer pessoa com o link.</span><span class="sxs-lookup"><span data-stu-id="d54b5-174">This view link provides read-only access to anyone with the link.</span></span>

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-view-link" } -->

```json
{
  "id": "1",
  "roles": ["read"],
  "link": {
    "scope": "anonymous",
    "type": "view",
    "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
    "application": { "id": "1234", "displayName": "Sample Application" }
  },
  "shareId": "!LKj1lkdlals90j1nlkascl",
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

### <a name="edit-link"></a><span data-ttu-id="d54b5-175">Link de edição</span><span class="sxs-lookup"><span data-stu-id="d54b5-175">Edit link</span></span>

<span data-ttu-id="d54b5-176">Este link de edição fornece acesso de leitura e gravação a qualquer pessoa na organização com o link.</span><span class="sxs-lookup"><span data-stu-id="d54b5-176">This edit link provides read and write access to anyone in the organization with the link.</span></span>

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-edit-link" } -->

```json
{
  "id": "2ceefb3g32hh",
  "roles": ["write"],
  "link": {
    "scope": "organization",
    "type": "edit",
    "webUrl": "https://contoso.sharepoint.com/:w:/t/design/fj277ghautbb422707565gnvg23",
    "application": { "id": "1234", "displayName": "Sample Application" }
  },
  "shareId": "!LKj1lkdlals90j1nlkascl",
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

### <a name="specific-people-link"></a><span data-ttu-id="d54b5-177">Link de pessoas específico</span><span class="sxs-lookup"><span data-stu-id="d54b5-177">Specific people link</span></span>

<span data-ttu-id="d54b5-178">Este link fornece acesso de leitura e gravação às pessoas específicas na `grantedToIdentities` coleção.</span><span class="sxs-lookup"><span data-stu-id="d54b5-178">This link provides read and write access to the specific people in the `grantedToIdentities` collection.</span></span>

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

## <a name="sharing-invitations"></a><span data-ttu-id="d54b5-179">Compartilhar convites</span><span class="sxs-lookup"><span data-stu-id="d54b5-179">Sharing invitations</span></span>

<span data-ttu-id="d54b5-180">As permissões enviadas pela API [INVITE][] podem ter mais informações na faceta [][SharingInvitation] do convite.</span><span class="sxs-lookup"><span data-stu-id="d54b5-180">Permissions sent by the [invite][] API may have additional information in the [invitation][SharingInvitation] facet.</span></span>
<span data-ttu-id="d54b5-181">Se um convite foi enviado a um endereço de email que não corresponde a uma conta conhecida \*\*\*\* , a propriedade concedidoto pode não ser definida até que o convite seja resgatado, que ocorre na primeira vez que o usuário clica no link e entra no.</span><span class="sxs-lookup"><span data-stu-id="d54b5-181">If an invitation was sent to an email address that doesn't match a known account, the **grantedTo** property may not be set until the invitation is redeemed, which occurs the first time the user clicks the link and signs in.</span></span>

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-invite-email" } -->

```json
{
  "id": "1",
  "roles": ["write"],
  "invitation": {
    "email": "jd@fabrikam.com",
    "signInRequired": true
  },
  "shareId": "FWxc1lasfdbEAGM5fI7B67aB5ZMPDMmQ11U",
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

<span data-ttu-id="d54b5-182">Depois que o convite de compartilhamento tiver sido resgatado por um usuário, a propriedade **grantedTo** conterá as informações sobre a conta que resgatou as permissões:</span><span class="sxs-lookup"><span data-stu-id="d54b5-182">After the sharing invitation has been redeemed by a user, the **grantedTo** property will contain the information about the account that redeemed the permissions:</span></span>

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
    "email": "jd@fabrikam.com",
    "signInRequired": true
  },
  "shareId": "FWxc1lasfdbEAGM5fI7B67aB5ZMPDMmQ11U",
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

## <a name="methods"></a><span data-ttu-id="d54b5-183">Métodos</span><span class="sxs-lookup"><span data-stu-id="d54b5-183">Methods</span></span>

| <span data-ttu-id="d54b5-184">Método</span><span class="sxs-lookup"><span data-stu-id="d54b5-184">Method</span></span>                                                   | <span data-ttu-id="d54b5-185">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="d54b5-185">REST Path</span></span>
|:---------------------------------------------------------|:-----------------------
| [<span data-ttu-id="d54b5-186">Listar permissões</span><span class="sxs-lookup"><span data-stu-id="d54b5-186">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="d54b5-187">Obter permissão</span><span class="sxs-lookup"><span data-stu-id="d54b5-187">Get permission</span></span>](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| <span data-ttu-id="d54b5-188">[Criar link] [CreateLink]</span><span class="sxs-lookup"><span data-stu-id="d54b5-188">[Create link][createLink]</span></span>                                | `POST /drive/items/{item-id}/createLink`
| <span data-ttu-id="d54b5-189">[Convidar pessoas] [convidar]</span><span class="sxs-lookup"><span data-stu-id="d54b5-189">[Invite people][invite]</span></span>                                  | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="d54b5-190">Atualizar</span><span class="sxs-lookup"><span data-stu-id="d54b5-190">Update</span></span>](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="d54b5-191">Delete</span><span class="sxs-lookup"><span data-stu-id="d54b5-191">Delete</span></span>](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`



[createLink]: ../api/driveitem-createlink.md
[IdentitySet]: identityset.md
[Alguém]: ../api/driveitem-invite.md
[invite]: ../api/driveitem-invite.md
[ItemReference]: itemreference.md
[API de compartilhamentos]: ../api/shares-get.md
[shares API]: ../api/shares-get.md
[SharingInvitation]: sharinginvitation.md
[SharingLink]: sharinglink.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The permission object provides information about permissions and roles and sharing information.",
  "keywords": "sharing,permissions,read,write,acl",
  "section": "documentation",
  "tocPath": "Resources/Permission",
  "suppressions": [
    "Error: /api-reference/beta/resources/permission.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
