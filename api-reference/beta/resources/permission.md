---
author: JeremyKelley
ms.author: JeremyKelley
title: tipo de recurso Permission
description: recurso Permission representando uma permissão de compartilhamento concedida para um driveItem
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: c35134e39618121f9aa7b29c490a6d8427b4a373
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108197"
---
# <a name="permission-resource-type"></a><span data-ttu-id="acdc0-103">tipo de recurso Permission</span><span class="sxs-lookup"><span data-stu-id="acdc0-103">permission resource type</span></span>

<span data-ttu-id="acdc0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acdc0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acdc0-105">O recurso **Permission** fornece informações sobre uma permissão de compartilhamento concedida para um recurso [driveItem](driveitem.md) .</span><span class="sxs-lookup"><span data-stu-id="acdc0-105">The **permission** resource provides information about a sharing permission granted for a [driveItem](driveitem.md) resource.</span></span>

<span data-ttu-id="acdc0-106">As permissões de compartilhamento têm várias formas diferentes.</span><span class="sxs-lookup"><span data-stu-id="acdc0-106">Sharing permissions have a number of different forms.</span></span>
<span data-ttu-id="acdc0-107">O recurso **Permission** representa esses diferentes formatos através de facetas no recurso.</span><span class="sxs-lookup"><span data-stu-id="acdc0-107">The **permission** resource represents these different forms through facets on the resource.</span></span>

><span data-ttu-id="acdc0-108">**Observação:** As bibliotecas de documentos do OneDrive for Business e do SharePoint não retornam a propriedade **inheritedFrom** .</span><span class="sxs-lookup"><span data-stu-id="acdc0-108">**Note:** OneDrive for Business and SharePoint document libraries do not return the **inheritedFrom** property.</span></span>

## <a name="json-representation"></a><span data-ttu-id="acdc0-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="acdc0-109">JSON representation</span></span>

<span data-ttu-id="acdc0-110">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="acdc0-110">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="acdc0-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="acdc0-111">Properties</span></span>

| <span data-ttu-id="acdc0-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="acdc0-112">Property</span></span>            | <span data-ttu-id="acdc0-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="acdc0-113">Type</span></span>                        | <span data-ttu-id="acdc0-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="acdc0-114">Description</span></span>
|:--------------------|:----------------------------|:-------------------------
| <span data-ttu-id="acdc0-115">id</span><span class="sxs-lookup"><span data-stu-id="acdc0-115">id</span></span>                  | <span data-ttu-id="acdc0-116">String</span><span class="sxs-lookup"><span data-stu-id="acdc0-116">String</span></span>                      | <span data-ttu-id="acdc0-p102">O identificador exclusivo da permissão entre todas as permissões no item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acdc0-p102">The unique identifier of the permission among all permissions on the item. Read-only.</span></span>
| <span data-ttu-id="acdc0-119">grantedTo</span><span class="sxs-lookup"><span data-stu-id="acdc0-119">grantedTo</span></span>           | <span data-ttu-id="acdc0-120">[IdentitySet][]</span><span class="sxs-lookup"><span data-stu-id="acdc0-120">[IdentitySet][]</span></span>             | <span data-ttu-id="acdc0-p103">Para permissões de tipo de usuário, os detalhes de usuários e aplicativos para esta permissão. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acdc0-p103">For user type permissions, the details of the users & applications for this permission. Read-only.</span></span>
| <span data-ttu-id="acdc0-123">grantedToIdentities</span><span class="sxs-lookup"><span data-stu-id="acdc0-123">grantedToIdentities</span></span> | <span data-ttu-id="acdc0-124">Coleção([IdentitySet][])</span><span class="sxs-lookup"><span data-stu-id="acdc0-124">Collection([IdentitySet][])</span></span> | <span data-ttu-id="acdc0-125">Para permissões de tipo de link, os detalhes dos usuários aos quais a permissão foi concedida.</span><span class="sxs-lookup"><span data-stu-id="acdc0-125">For link type permissions, the details of the users to whom permission was granted.</span></span> <span data-ttu-id="acdc0-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acdc0-126">Read-only.</span></span>
| <span data-ttu-id="acdc0-127">invitation</span><span class="sxs-lookup"><span data-stu-id="acdc0-127">invitation</span></span>          | <span data-ttu-id="acdc0-128">[SharingInvitation][]</span><span class="sxs-lookup"><span data-stu-id="acdc0-128">[SharingInvitation][]</span></span>       | <span data-ttu-id="acdc0-p105">Detalhes de um convite de compartilhamento associado para esta permissão. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acdc0-p105">Details of any associated sharing invitation for this permission. Read-only.</span></span>
| <span data-ttu-id="acdc0-131">inheritedFrom</span><span class="sxs-lookup"><span data-stu-id="acdc0-131">inheritedFrom</span></span>       | <span data-ttu-id="acdc0-132">[ItemReference][]</span><span class="sxs-lookup"><span data-stu-id="acdc0-132">[ItemReference][]</span></span>           | <span data-ttu-id="acdc0-p106">Fornece uma referência para o ancestral da permissão atual, se ela for herdada de um ancestral. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acdc0-p106">Provides a reference to the ancestor of the current permission, if it is inherited from an ancestor. Read-only.</span></span>
| <span data-ttu-id="acdc0-135">vínculo</span><span class="sxs-lookup"><span data-stu-id="acdc0-135">link</span></span>                | <span data-ttu-id="acdc0-136">[SharingLink][]</span><span class="sxs-lookup"><span data-stu-id="acdc0-136">[SharingLink][]</span></span>             | <span data-ttu-id="acdc0-p107">Fornece os detalhes do link de permissão atual, caso se trate de permissões de tipo de link. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acdc0-p107">Provides the link details of the current permission, if it is a link type permissions. Read-only.</span></span>
| <span data-ttu-id="acdc0-139">funções</span><span class="sxs-lookup"><span data-stu-id="acdc0-139">roles</span></span>               | <span data-ttu-id="acdc0-140">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="acdc0-140">Collection(String)</span></span>          | <span data-ttu-id="acdc0-p108">O tipo de permissão, por exemplo, `read`. Veja abaixo a lista completa de funções. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acdc0-p108">The type of permission, e.g. `read`. See below for the full list of roles. Read-only.</span></span>
| <span data-ttu-id="acdc0-144">shareId</span><span class="sxs-lookup"><span data-stu-id="acdc0-144">shareId</span></span>             | <span data-ttu-id="acdc0-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="acdc0-145">String</span></span>                      | <span data-ttu-id="acdc0-146">Um token exclusivo que pode ser usado para acessar esse item compartilhado por meio da **[API de compartilhamentos][]**.</span><span class="sxs-lookup"><span data-stu-id="acdc0-146">A unique token that can be used to access this shared item via the **[shares API][]**.</span></span> <span data-ttu-id="acdc0-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acdc0-147">Read-only.</span></span>
| <span data-ttu-id="acdc0-148">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="acdc0-148">expirationDateTime</span></span>  | <span data-ttu-id="acdc0-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acdc0-149">DateTimeOffset</span></span>              | <span data-ttu-id="acdc0-150">Um formato de yyyy-MM-ddTHH: mm: ssZ de DateTimeOffset indica o tempo de expiração da permissão.</span><span class="sxs-lookup"><span data-stu-id="acdc0-150">A format of yyyy-MM-ddTHH:mm:ssZ of DateTimeOffset indicates the expiration time of the permission.</span></span> <span data-ttu-id="acdc0-151">DateTime. MinValue indica que não há validade configurada para essa permissão.</span><span class="sxs-lookup"><span data-stu-id="acdc0-151">DateTime.MinValue indicates there is no expiration set for this permission.</span></span> <span data-ttu-id="acdc0-152">Opcional.</span><span class="sxs-lookup"><span data-stu-id="acdc0-152">Optional.</span></span>
| <span data-ttu-id="acdc0-153">hasPassword</span><span class="sxs-lookup"><span data-stu-id="acdc0-153">hasPassword</span></span>         | <span data-ttu-id="acdc0-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="acdc0-154">Boolean</span></span>                     | <span data-ttu-id="acdc0-155">Isso indica se a senha está definida para essa permissão, ela só será mostrada em resposta.</span><span class="sxs-lookup"><span data-stu-id="acdc0-155">This indicates whether password is set for this permission, it's only showing in response.</span></span> <span data-ttu-id="acdc0-156">Opcional e somente leitura e somente para o OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="acdc0-156">Optional and Read-only and for OneDrive Personal only.</span></span>

### <a name="roles-enumeration-values"></a><span data-ttu-id="acdc0-157">Valores de enumeração de funções</span><span class="sxs-lookup"><span data-stu-id="acdc0-157">Roles enumeration values</span></span>

| <span data-ttu-id="acdc0-158">Valor</span><span class="sxs-lookup"><span data-stu-id="acdc0-158">Value</span></span>        | <span data-ttu-id="acdc0-159">Detalhes</span><span class="sxs-lookup"><span data-stu-id="acdc0-159">Details</span></span>                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | <span data-ttu-id="acdc0-160">Fornece a capacidade de ler os metadados e o conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="acdc0-160">Provides the ability to read the metadata and contents of the item.</span></span>            |
| `write`     | <span data-ttu-id="acdc0-161">Fornece a capacidade de ler e modificar os metadados e o conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="acdc0-161">Provides the ability to read and modify the metadata and contents of the item.</span></span> |
| `sp.owner`  | <span data-ttu-id="acdc0-162">Para o SharePoint e o OneDrive for Business, isso representa a função de proprietário.</span><span class="sxs-lookup"><span data-stu-id="acdc0-162">For SharePoint and OneDrive for Business this represents the owner role.</span></span>       |
| `sp.member` | <span data-ttu-id="acdc0-163">Para o SharePoint e o OneDrive for Business, isso representa a função de membro.</span><span class="sxs-lookup"><span data-stu-id="acdc0-163">For SharePoint and OneDrive for Business this represents the member role.</span></span>      |

<span data-ttu-id="acdc0-164">O recurso permission usa _facetas_ para fornecer informações sobre o tipo de permissão representado pelo recurso.</span><span class="sxs-lookup"><span data-stu-id="acdc0-164">The permission resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="acdc0-165">Os links de compartilhamento contêm um token exclusivo e necessário para acessar o item.</span><span class="sxs-lookup"><span data-stu-id="acdc0-165">Sharing links contain a unique token required to access the item.</span></span>

<span data-ttu-id="acdc0-166">Permissões com uma faceta [**invitation**][SharingInvitation] representam permissões adicionadas convidando usuários ou grupos específicos para ter acesso ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="acdc0-166">Permissions with an [**invitation**][SharingInvitation] facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

## <a name="sharing-links"></a><span data-ttu-id="acdc0-167">Links de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="acdc0-167">Sharing links</span></span>

<span data-ttu-id="acdc0-168">Permissões com uma faceta [**link**][SharingLink] representam links de compartilhamento criados no item.</span><span class="sxs-lookup"><span data-stu-id="acdc0-168">Permissions with a [**link**][SharingLink] facet represent sharing links created on the item.</span></span>
<span data-ttu-id="acdc0-169">Estes são os tipos mais comuns de permissões.</span><span class="sxs-lookup"><span data-stu-id="acdc0-169">These are the most common kinds of permissions.</span></span>
<span data-ttu-id="acdc0-170">Os links de compartilhamento fornecem uma URL exclusiva que pode ser usada para acessar um arquivo ou pasta.</span><span class="sxs-lookup"><span data-stu-id="acdc0-170">Sharing links provide a unique URL that can be used to access a file or folder.</span></span>
<span data-ttu-id="acdc0-171">Eles podem ser configurados para conceder acesso de várias maneiras.</span><span class="sxs-lookup"><span data-stu-id="acdc0-171">They can be set up to grant access in a variety of ways.</span></span>
<span data-ttu-id="acdc0-172">Por exemplo, você pode usar a API [createLink][] para criar um link que funcione para qualquer pessoa conectada à sua organização ou criar um link que funcione para qualquer pessoa, sem precisar fazer logon.</span><span class="sxs-lookup"><span data-stu-id="acdc0-172">For example, you can use the [createLink][] API to create a link that works for anyone signed into your organization, or you can create a link that works for anyone, without needing to sign in.</span></span>
<span data-ttu-id="acdc0-173">Você pode usar a API [invite][] para criar um link que funcione apenas para pessoas específicas, estejam elas na sua empresa ou não.</span><span class="sxs-lookup"><span data-stu-id="acdc0-173">You can use the [invite][] API to create a link that only works for specific people, whether they're in your company or not.</span></span>

<span data-ttu-id="acdc0-174">Aqui estão alguns exemplos de links de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="acdc0-174">Here are some examples of sharing links.</span></span>

### <a name="view-link"></a><span data-ttu-id="acdc0-175">Link de exibição</span><span class="sxs-lookup"><span data-stu-id="acdc0-175">View link</span></span>

<span data-ttu-id="acdc0-176">Este link de exibição fornece acesso somente leitura a qualquer pessoa com o link.</span><span class="sxs-lookup"><span data-stu-id="acdc0-176">This view link provides read-only access to anyone with the link.</span></span>

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

### <a name="edit-link"></a><span data-ttu-id="acdc0-177">Editar link</span><span class="sxs-lookup"><span data-stu-id="acdc0-177">Edit link</span></span>

<span data-ttu-id="acdc0-178">Este link de edição fornece acesso de leitura e gravação a qualquer pessoa na organização com o link.</span><span class="sxs-lookup"><span data-stu-id="acdc0-178">This edit link provides read and write access to anyone in the organization with the link.</span></span>

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

### <a name="existing-access-link"></a><span data-ttu-id="acdc0-179">Link de acesso existente</span><span class="sxs-lookup"><span data-stu-id="acdc0-179">Existing access link</span></span>

<span data-ttu-id="acdc0-180">Este link não concede nenhum privilégio adicional para o usuário.</span><span class="sxs-lookup"><span data-stu-id="acdc0-180">This link does not grant any additional privileges to the user.</span></span>

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

### <a name="specific-people-link"></a><span data-ttu-id="acdc0-181">Link de pessoas específicas</span><span class="sxs-lookup"><span data-stu-id="acdc0-181">Specific people link</span></span>

<span data-ttu-id="acdc0-182">Este link fornece acesso de leitura e gravação para as pessoas específicas na coleção `grantedToIdentities`.</span><span class="sxs-lookup"><span data-stu-id="acdc0-182">This link provides read and write access to the specific people in the `grantedToIdentities` collection.</span></span>

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

## <a name="sharing-invitations"></a><span data-ttu-id="acdc0-183">Compartilhar convites</span><span class="sxs-lookup"><span data-stu-id="acdc0-183">Sharing invitations</span></span>

<span data-ttu-id="acdc0-184">As permissões enviadas pelo [convite][] ou pela API de [concessão][] podem ter informações adicionais na faceta[SharingInvitation] do [convite]para endereços de email que não correspondem a uma conta conhecida.</span><span class="sxs-lookup"><span data-stu-id="acdc0-184">Permissions sent by the [invite][] or [grant][] API can have additional information in the [invitation][SharingInvitation] facet for email addresses that don't match a known account.</span></span> <span data-ttu-id="acdc0-185">Nesses casos, a propriedade **concedidoto** pode não ser definida até que o link do convite seja resgatado, que ocorre na primeira vez que o usuário clica no link e entrar.</span><span class="sxs-lookup"><span data-stu-id="acdc0-185">In such cases, the **grantedTo** property might not be set until the invitation link is redeemed, which occurs the first time the user clicks the link and signs in.</span></span>

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

<span data-ttu-id="acdc0-186">Depois que o convite de compartilhamento tiver sido resgatado por um usuário, a propriedade **grantedTo** conterá as informações sobre a conta que resgatou as permissões:</span><span class="sxs-lookup"><span data-stu-id="acdc0-186">After the sharing invitation has been redeemed by a user, the **grantedTo** property will contain the information about the account that redeemed the permissions:</span></span>

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

## <a name="methods"></a><span data-ttu-id="acdc0-187">Métodos</span><span class="sxs-lookup"><span data-stu-id="acdc0-187">Methods</span></span>

| <span data-ttu-id="acdc0-188">Método</span><span class="sxs-lookup"><span data-stu-id="acdc0-188">Method</span></span>                                                   | <span data-ttu-id="acdc0-189">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="acdc0-189">REST Path</span></span>
|:---------------------------------------------------------|:-----------------------
| [<span data-ttu-id="acdc0-190">Listar permissões</span><span class="sxs-lookup"><span data-stu-id="acdc0-190">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="acdc0-191">Obter permissão</span><span class="sxs-lookup"><span data-stu-id="acdc0-191">Get permission</span></span>](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| <span data-ttu-id="acdc0-192">[Criar link][createLink]</span><span class="sxs-lookup"><span data-stu-id="acdc0-192">[Create link][createLink]</span></span>                                | `POST /drive/items/{item-id}/createLink`
| <span data-ttu-id="acdc0-193">[Convidar pessoas][invite]</span><span class="sxs-lookup"><span data-stu-id="acdc0-193">[Invite people][invite]</span></span>                                  | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="acdc0-194">Atualizar</span><span class="sxs-lookup"><span data-stu-id="acdc0-194">Update</span></span>](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="acdc0-195">Delete</span><span class="sxs-lookup"><span data-stu-id="acdc0-195">Delete</span></span>](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="acdc0-196">Adicionar usuários ao link de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="acdc0-196">Add users to sharing link</span></span>](../api/permission-grant.md)  | `POST /shares/{encoded-sharing-url}/permission/grant`


[createLink]: ../api/driveitem-createlink.md
[conceder]: ../api/permission-grant.md
[grant]: ../api/permission-grant.md
[IdentitySet]: identityset.md
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
  "suppressions": []
}
-->
