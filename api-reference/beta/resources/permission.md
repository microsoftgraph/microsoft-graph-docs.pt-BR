---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Permissão
localization_priority: Normal
ms.openlocfilehash: 6a5a0af9c95900232ff87aa7aedb731a83a91cc5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518846"
---
# <a name="permission-resource-type"></a><span data-ttu-id="1e5d6-102">Tipo de recurso permission</span><span class="sxs-lookup"><span data-stu-id="1e5d6-102">permission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e5d6-103">O recurso **Permission** fornece informações sobre uma permissão de compartilhamento concedida a um recurso [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="1e5d6-103">The **permission** resource provides information about a sharing permission granted for a [driveItem](driveitem.md) resource.</span></span>

<span data-ttu-id="1e5d6-104">As permissões de compartilhamento têm várias formas diferentes.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-104">Sharing permissions have a number of different forms.</span></span>
<span data-ttu-id="1e5d6-105">O recurso **Permission** representa estes diferentes formatos por meio de facetas do recurso.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-105">The **permission** resource represents these different forms through facets on the resource.</span></span>

><span data-ttu-id="1e5d6-106">**Observação:** OneDrive para negócios e SharePoint bibliotecas de documentos não retornou a propriedade **inheritedFrom** .</span><span class="sxs-lookup"><span data-stu-id="1e5d6-106">**Note:** OneDrive for Business and SharePoint document libraries do not return the **inheritedFrom** property.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e5d6-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1e5d6-107">JSON representation</span></span>

<span data-ttu-id="1e5d6-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="1e5d6-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1e5d6-109">Properties</span></span>

| <span data-ttu-id="1e5d6-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e5d6-110">Property</span></span>            | <span data-ttu-id="1e5d6-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e5d6-111">Type</span></span>                        | <span data-ttu-id="1e5d6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e5d6-112">Description</span></span>
|:--------------------|:----------------------------|:-------------------------
| <span data-ttu-id="1e5d6-113">id</span><span class="sxs-lookup"><span data-stu-id="1e5d6-113">id</span></span>                  | <span data-ttu-id="1e5d6-114">String</span><span class="sxs-lookup"><span data-stu-id="1e5d6-114">String</span></span>                      | <span data-ttu-id="1e5d6-p102">O identificador exclusivo da permissão entre todas as permissões no item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-p102">The unique identifier of the permission among all permissions on the item. Read-only.</span></span>
| <span data-ttu-id="1e5d6-117">grantedTo</span><span class="sxs-lookup"><span data-stu-id="1e5d6-117">grantedTo</span></span>           | <span data-ttu-id="1e5d6-118">[IdentitySet][]</span><span class="sxs-lookup"><span data-stu-id="1e5d6-118">[IdentitySet][]</span></span>             | <span data-ttu-id="1e5d6-p103">Para permissões de tipo de usuário, os detalhes de usuários e aplicativos para esta permissão. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-p103">For user type permissions, the details of the users & applications for this permission. Read-only.</span></span>
| <span data-ttu-id="1e5d6-121">grantedToIdentities</span><span class="sxs-lookup"><span data-stu-id="1e5d6-121">grantedToIdentities</span></span> | <span data-ttu-id="1e5d6-122">Coleção ([IdentitySet][])</span><span class="sxs-lookup"><span data-stu-id="1e5d6-122">Collection([IdentitySet][])</span></span> | <span data-ttu-id="1e5d6-123">Para obter permissões de tipo de link, os detalhes dos usuários aos quais a permissão foi concedida.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-123">For link type permissions, the details of the users to whom permission was granted.</span></span> <span data-ttu-id="1e5d6-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-124">Read-only.</span></span>
| <span data-ttu-id="1e5d6-125">invitation</span><span class="sxs-lookup"><span data-stu-id="1e5d6-125">invitation</span></span>          | <span data-ttu-id="1e5d6-126">[SharingInvitation][]</span><span class="sxs-lookup"><span data-stu-id="1e5d6-126">[SharingInvitation][]</span></span>       | <span data-ttu-id="1e5d6-p105">Detalhes de um convite de compartilhamento associado para esta permissão. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-p105">Details of any associated sharing invitation for this permission. Read-only.</span></span>
| <span data-ttu-id="1e5d6-129">inheritedFrom</span><span class="sxs-lookup"><span data-stu-id="1e5d6-129">inheritedFrom</span></span>       | <span data-ttu-id="1e5d6-130">[ItemReference][]</span><span class="sxs-lookup"><span data-stu-id="1e5d6-130">[ItemReference][]</span></span>           | <span data-ttu-id="1e5d6-p106">Fornece uma referência para o ancestral da permissão atual, se ela for herdada de um ancestral. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-p106">Provides a reference to the ancestor of the current permission, if it is inherited from an ancestor. Read-only.</span></span>
| <span data-ttu-id="1e5d6-133">vínculo</span><span class="sxs-lookup"><span data-stu-id="1e5d6-133">link</span></span>                | <span data-ttu-id="1e5d6-134">[SharingLink][]</span><span class="sxs-lookup"><span data-stu-id="1e5d6-134">[SharingLink][]</span></span>             | <span data-ttu-id="1e5d6-p107">Fornece os detalhes do link de permissão atual, caso se trate de permissões de tipo de link. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-p107">Provides the link details of the current permission, if it is a link type permissions. Read-only.</span></span>
| <span data-ttu-id="1e5d6-137">funções</span><span class="sxs-lookup"><span data-stu-id="1e5d6-137">roles</span></span>               | <span data-ttu-id="1e5d6-138">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="1e5d6-138">Collection(String)</span></span>          | <span data-ttu-id="1e5d6-p108">O tipo de permissão, por exemplo, `read`. Veja abaixo a lista completa de funções. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-p108">The type of permission, e.g. `read`. See below for the full list of roles. Read-only.</span></span>
| <span data-ttu-id="1e5d6-142">shareId</span><span class="sxs-lookup"><span data-stu-id="1e5d6-142">shareId</span></span>             | <span data-ttu-id="1e5d6-143">String</span><span class="sxs-lookup"><span data-stu-id="1e5d6-143">String</span></span>                      | <span data-ttu-id="1e5d6-p109">Um token exclusivo que pode ser usado para acessar esse item compartilhado por meio da \*\* [API][] Shares\*\*. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-p109">A unique token that can be used to access this shared item via the **[shares API][]**. Read-only.</span></span>
| <span data-ttu-id="1e5d6-146">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1e5d6-146">expirationDateTime</span></span>  | <span data-ttu-id="1e5d6-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e5d6-147">DateTimeOffset</span></span>              | <span data-ttu-id="1e5d6-148">Um formato AAAA-MM-ddTHH:mm:ssZ de DateTimeOffset indica a hora de expiração da permissão.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-148">A format of yyyy-MM-ddTHH:mm:ssZ of DateTimeOffset indicates the expiration time of the permission.</span></span> <span data-ttu-id="1e5d6-149">DateTime.MinValue indica que existem é nenhum vencimento definido para esta permissão.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-149">DateTime.MinValue indicates there is no expiration set for this permission.</span></span> <span data-ttu-id="1e5d6-150">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-150">Optional.</span></span>
| <span data-ttu-id="1e5d6-151">HasPassword</span><span class="sxs-lookup"><span data-stu-id="1e5d6-151">hasPassword</span></span>         | <span data-ttu-id="1e5d6-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="1e5d6-152">Boolean</span></span>                     | <span data-ttu-id="1e5d6-153">Isso indica que se a senha é definida para esta permissão, ele só Mostrar em resposta.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-153">This indicates whether password is set for this permission, it's only showing in response.</span></span> <span data-ttu-id="1e5d6-154">Opcional e somente leitura e para OneDrive pessoal somente.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-154">Optional and Read-only and for OneDrive Personal only.</span></span>

### <a name="roles-enumeration-values"></a><span data-ttu-id="1e5d6-155">Valores de enumeração de funções</span><span class="sxs-lookup"><span data-stu-id="1e5d6-155">Roles enumeration values</span></span>

| <span data-ttu-id="1e5d6-156">Valor</span><span class="sxs-lookup"><span data-stu-id="1e5d6-156">Value</span></span>        | <span data-ttu-id="1e5d6-157">Detalhes</span><span class="sxs-lookup"><span data-stu-id="1e5d6-157">Details</span></span>                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | <span data-ttu-id="1e5d6-158">Fornece a capacidade de ler os metadados e o conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-158">Provides the ability to read the metadata and contents of the item.</span></span>            |
| `write`     | <span data-ttu-id="1e5d6-159">Fornece a capacidade de ler e modificar os metadados e o conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-159">Provides the ability to read and modify the metadata and contents of the item.</span></span> |
| `sp.owner`  | <span data-ttu-id="1e5d6-160">Para o SharePoint e o OneDrive for Business, isso representa a função de proprietário.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-160">For SharePoint and OneDrive for Business this represents the owner role.</span></span>       |
| `sp.member` | <span data-ttu-id="1e5d6-161">Para o SharePoint e o OneDrive for Business, isso representa a função de membro.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-161">For SharePoint and OneDrive for Business this represents the member role.</span></span>      |

<span data-ttu-id="1e5d6-162">O recurso permission usa _facetas_ para fornecer informações sobre o tipo de permissão representado pelo recurso.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-162">The permission resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="1e5d6-163">Links de compartilhamento contêm um token exclusivo necessário para acessar o item.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-163">Sharing links contain a unique token required to access the item.</span></span>

<span data-ttu-id="1e5d6-164">Permissões com uma faceta [**invitation**][SharingInvitation] representam permissões adicionadas convidando usuários ou grupos específicos para ter acesso ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-164">Permissions with an [**invitation**][SharingInvitation] facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

## <a name="sharing-links"></a><span data-ttu-id="1e5d6-165">Links de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="1e5d6-165">Sharing links</span></span>

<span data-ttu-id="1e5d6-166">Permissões com um [**link**][SharingLink] faceta representam que compartilhamento links criados no item.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-166">Permissions with a [**link**][SharingLink] facet represent sharing links created on the item.</span></span>
<span data-ttu-id="1e5d6-167">Esses são os tipos mais comuns de permissões.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-167">These are the most common kinds of permissions.</span></span>
<span data-ttu-id="1e5d6-168">Compartilhamento de links fornecem uma URL exclusiva que pode ser usada para acessar um arquivo ou pasta.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-168">Sharing links provide a unique URL that can be used to access a file or folder.</span></span>
<span data-ttu-id="1e5d6-169">Eles podem ser configurados para conceder acesso de várias maneiras.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-169">They can be set up to grant access in a variety of ways.</span></span>
<span data-ttu-id="1e5d6-170">Por exemplo, você pode usar o [createLink][] API para criar um link que funciona para qualquer pessoa entrado na sua organização, ou você pode criar um link que funciona para qualquer pessoa, sem precisar entrar.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-170">For example, you can use the [createLink][] API to create a link that works for anyone signed into your organization, or you can create a link that works for anyone, without needing to sign in.</span></span>
<span data-ttu-id="1e5d6-171">Você pode usar a [Convidar][] API para criar um link que funciona somente para pessoas específicas, se eles estiverem em sua empresa ou não.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-171">You can use the [invite][] API to create a link that only works for specific people, whether they're in your company or not.</span></span>

<span data-ttu-id="1e5d6-172">Aqui estão alguns exemplos de links de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-172">Here are some examples of sharing links.</span></span>

### <a name="view-link"></a><span data-ttu-id="1e5d6-173">Link de exibição</span><span class="sxs-lookup"><span data-stu-id="1e5d6-173">View link</span></span>

<span data-ttu-id="1e5d6-174">Este link Exibir fornece acesso somente leitura para qualquer pessoa com o link.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-174">This view link provides read-only access to anyone with the link.</span></span>

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

### <a name="edit-link"></a><span data-ttu-id="1e5d6-175">Link de edição</span><span class="sxs-lookup"><span data-stu-id="1e5d6-175">Edit link</span></span>

<span data-ttu-id="1e5d6-176">Este link Editar fornece acesso de leitura e gravação para qualquer pessoa da organização com o link.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-176">This edit link provides read and write access to anyone in the organization with the link.</span></span>

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

### <a name="specific-people-link"></a><span data-ttu-id="1e5d6-177">Link de pessoas específicas</span><span class="sxs-lookup"><span data-stu-id="1e5d6-177">Specific people link</span></span>

<span data-ttu-id="1e5d6-178">Este link fornece acesso de leitura e gravação para as pessoas específicas no `grantedToIdentities` conjunto.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-178">This link provides read and write access to the specific people in the `grantedToIdentities` collection.</span></span>

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

## <a name="sharing-invitations"></a><span data-ttu-id="1e5d6-179">Convites de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="1e5d6-179">Sharing invitations</span></span>

<span data-ttu-id="1e5d6-180">Permissões enviadas pela [Convidar][] API podem ter informações adicionais no aspecto de[SharingInvitation] [convite].</span><span class="sxs-lookup"><span data-stu-id="1e5d6-180">Permissions sent by the [invite][] API may have additional information in the [invitation][SharingInvitation] facet.</span></span>
<span data-ttu-id="1e5d6-181">Se um convite foi enviado a um endereço de email que não corresponda a uma conta conhecida, a propriedade **grantedTo** não pode ser definida até que o convite for trocado, o que ocorre na primeira vez em que o usuário clica no link e entra no.</span><span class="sxs-lookup"><span data-stu-id="1e5d6-181">If an invitation was sent to an email address that doesn't match a known account, the **grantedTo** property may not be set until the invitation is redeemed, which occurs the first time the user clicks the link and signs in.</span></span>

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

<span data-ttu-id="1e5d6-182">Depois que o convite de compartilhamento tiver sido resgatado por um usuário, a propriedade **grantedTo** conterá as informações sobre a conta que resgatou as permissões:</span><span class="sxs-lookup"><span data-stu-id="1e5d6-182">After the sharing invitation has been redeemed by a user, the **grantedTo** property will contain the information about the account that redeemed the permissions:</span></span>

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

## <a name="methods"></a><span data-ttu-id="1e5d6-183">Métodos</span><span class="sxs-lookup"><span data-stu-id="1e5d6-183">Methods</span></span>

| <span data-ttu-id="1e5d6-184">Método</span><span class="sxs-lookup"><span data-stu-id="1e5d6-184">Method</span></span>                                                   | <span data-ttu-id="1e5d6-185">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="1e5d6-185">REST Path</span></span>
|:---------------------------------------------------------|:-----------------------
| [<span data-ttu-id="1e5d6-186">Listar permissões</span><span class="sxs-lookup"><span data-stu-id="1e5d6-186">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="1e5d6-187">Obter permissão</span><span class="sxs-lookup"><span data-stu-id="1e5d6-187">Get permission</span></span>](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| <span data-ttu-id="1e5d6-188">[Link Criar] [createLink]</span><span class="sxs-lookup"><span data-stu-id="1e5d6-188">[Create link][createLink]</span></span>                                | `POST /drive/items/{item-id}/createLink`
| <span data-ttu-id="1e5d6-189">[Convidar pessoas] [Convidar]</span><span class="sxs-lookup"><span data-stu-id="1e5d6-189">[Invite people][invite]</span></span>                                  | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="1e5d6-190">Update</span><span class="sxs-lookup"><span data-stu-id="1e5d6-190">Update</span></span>](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="1e5d6-191">Delete</span><span class="sxs-lookup"><span data-stu-id="1e5d6-191">Delete</span></span>](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`



[createLink]: ../api/driveitem-createlink.md
[IdentitySet]: identityset.md
[Convidar]: ../api/driveitem-invite.md
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
