---
author: JeremyKelley
title: tipo de recurso de permissão
description: recurso permission representando uma permissão de compartilhamento concedida para um driveItem
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: e7eb160bf7899feec9afda49c6087072aab83c3b
ms.sourcegitcommit: 2d8b04725ea4eaf304f3da1056a6451457a4630f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/12/2021
ms.locfileid: "52335601"
---
# <a name="permission-resource-type"></a><span data-ttu-id="c06a5-103">tipo de recurso de permissão</span><span class="sxs-lookup"><span data-stu-id="c06a5-103">permission resource type</span></span>

<span data-ttu-id="c06a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c06a5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c06a5-105">O **recurso de** permissão fornece informações sobre uma permissão de compartilhamento concedida para um recurso [driveItem.](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="c06a5-105">The **permission** resource provides information about a sharing permission granted for a [driveItem](driveitem.md) resource.</span></span>

<span data-ttu-id="c06a5-106">As permissões de compartilhamento têm várias formas diferentes.</span><span class="sxs-lookup"><span data-stu-id="c06a5-106">Sharing permissions have a number of different forms.</span></span>
<span data-ttu-id="c06a5-107">O **recurso de** permissão representa esses diferentes formulários por meio de facetas no recurso.</span><span class="sxs-lookup"><span data-stu-id="c06a5-107">The **permission** resource represents these different forms through facets on the resource.</span></span>

><span data-ttu-id="c06a5-108">**Observação:** OneDrive for Business e SharePoint de documentos não retornam a **propriedade inheritedFrom.**</span><span class="sxs-lookup"><span data-stu-id="c06a5-108">**Note:** OneDrive for Business and SharePoint document libraries do not return the **inheritedFrom** property.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c06a5-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c06a5-109">JSON representation</span></span>

<span data-ttu-id="c06a5-110">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c06a5-110">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="c06a5-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c06a5-111">Properties</span></span>

| <span data-ttu-id="c06a5-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c06a5-112">Property</span></span>            | <span data-ttu-id="c06a5-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="c06a5-113">Type</span></span>                        | <span data-ttu-id="c06a5-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="c06a5-114">Description</span></span>
|:--------------------|:----------------------------|:-------------------------
| <span data-ttu-id="c06a5-115">id</span><span class="sxs-lookup"><span data-stu-id="c06a5-115">id</span></span>                  | <span data-ttu-id="c06a5-116">String</span><span class="sxs-lookup"><span data-stu-id="c06a5-116">String</span></span>                      | <span data-ttu-id="c06a5-p102">O identificador exclusivo da permissão entre todas as permissões no item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c06a5-p102">The unique identifier of the permission among all permissions on the item. Read-only.</span></span>
| <span data-ttu-id="c06a5-119">grantedTo</span><span class="sxs-lookup"><span data-stu-id="c06a5-119">grantedTo</span></span>           | <span data-ttu-id="c06a5-120">[IdentitySet][]</span><span class="sxs-lookup"><span data-stu-id="c06a5-120">[IdentitySet][]</span></span>             | <span data-ttu-id="c06a5-p103">Para permissões de tipo de usuário, os detalhes de usuários e aplicativos para esta permissão. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c06a5-p103">For user type permissions, the details of the users & applications for this permission. Read-only.</span></span>
| <span data-ttu-id="c06a5-123">grantedToIdentities</span><span class="sxs-lookup"><span data-stu-id="c06a5-123">grantedToIdentities</span></span> | <span data-ttu-id="c06a5-124">Coleção([IdentitySet][])</span><span class="sxs-lookup"><span data-stu-id="c06a5-124">Collection([IdentitySet][])</span></span> | <span data-ttu-id="c06a5-125">Para permissões de tipo de link, os detalhes dos usuários aos quais a permissão foi concedida.</span><span class="sxs-lookup"><span data-stu-id="c06a5-125">For link type permissions, the details of the users to whom permission was granted.</span></span> <span data-ttu-id="c06a5-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c06a5-126">Read-only.</span></span>
| <span data-ttu-id="c06a5-127">invitation</span><span class="sxs-lookup"><span data-stu-id="c06a5-127">invitation</span></span>          | <span data-ttu-id="c06a5-128">[SharingInvitation][]</span><span class="sxs-lookup"><span data-stu-id="c06a5-128">[SharingInvitation][]</span></span>       | <span data-ttu-id="c06a5-p105">Detalhes de um convite de compartilhamento associado para esta permissão. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c06a5-p105">Details of any associated sharing invitation for this permission. Read-only.</span></span>
| <span data-ttu-id="c06a5-131">inheritedFrom</span><span class="sxs-lookup"><span data-stu-id="c06a5-131">inheritedFrom</span></span>       | <span data-ttu-id="c06a5-132">[ItemReference][]</span><span class="sxs-lookup"><span data-stu-id="c06a5-132">[ItemReference][]</span></span>           | <span data-ttu-id="c06a5-p106">Fornece uma referência para o ancestral da permissão atual, se ela for herdada de um ancestral. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c06a5-p106">Provides a reference to the ancestor of the current permission, if it is inherited from an ancestor. Read-only.</span></span>
| <span data-ttu-id="c06a5-135">vínculo</span><span class="sxs-lookup"><span data-stu-id="c06a5-135">link</span></span>                | <span data-ttu-id="c06a5-136">[SharingLink][]</span><span class="sxs-lookup"><span data-stu-id="c06a5-136">[SharingLink][]</span></span>             | <span data-ttu-id="c06a5-p107">Fornece os detalhes do link de permissão atual, caso se trate de permissões de tipo de link. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c06a5-p107">Provides the link details of the current permission, if it is a link type permissions. Read-only.</span></span>
| <span data-ttu-id="c06a5-139">funções</span><span class="sxs-lookup"><span data-stu-id="c06a5-139">roles</span></span>               | <span data-ttu-id="c06a5-140">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="c06a5-140">Collection(String)</span></span>          | <span data-ttu-id="c06a5-p108">O tipo de permissão, por exemplo, `read`. Veja abaixo a lista completa de funções. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c06a5-p108">The type of permission, e.g. `read`. See below for the full list of roles. Read-only.</span></span>
| <span data-ttu-id="c06a5-144">shareId</span><span class="sxs-lookup"><span data-stu-id="c06a5-144">shareId</span></span>             | <span data-ttu-id="c06a5-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c06a5-145">String</span></span>                      | <span data-ttu-id="c06a5-146">Um token exclusivo que pode ser usado para acessar esse item compartilhado por meio da **[API de compartilhamentos][]**.</span><span class="sxs-lookup"><span data-stu-id="c06a5-146">A unique token that can be used to access this shared item via the **[shares API][]**.</span></span> <span data-ttu-id="c06a5-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c06a5-147">Read-only.</span></span>
| <span data-ttu-id="c06a5-148">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c06a5-148">expirationDateTime</span></span>  | <span data-ttu-id="c06a5-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c06a5-149">DateTimeOffset</span></span>              | <span data-ttu-id="c06a5-150">Um formato yyyy-MM-ddTHH:mm:ssZ de DateTimeOffset indica o tempo de expiração da permissão.</span><span class="sxs-lookup"><span data-stu-id="c06a5-150">A format of yyyy-MM-ddTHH:mm:ssZ of DateTimeOffset indicates the expiration time of the permission.</span></span> <span data-ttu-id="c06a5-151">DateTime.MinValue indica que não há expiração definida para esta permissão.</span><span class="sxs-lookup"><span data-stu-id="c06a5-151">DateTime.MinValue indicates there is no expiration set for this permission.</span></span> <span data-ttu-id="c06a5-152">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c06a5-152">Optional.</span></span>
| <span data-ttu-id="c06a5-153">hasPassword</span><span class="sxs-lookup"><span data-stu-id="c06a5-153">hasPassword</span></span>         | <span data-ttu-id="c06a5-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="c06a5-154">Boolean</span></span>                     | <span data-ttu-id="c06a5-155">Isso indica se a senha está configurada para esta permissão, está sendo exibida apenas em resposta.</span><span class="sxs-lookup"><span data-stu-id="c06a5-155">This indicates whether password is set for this permission, it's only showing in response.</span></span> <span data-ttu-id="c06a5-156">Opcional e Somente leitura e somente para o OneDrive Personal.</span><span class="sxs-lookup"><span data-stu-id="c06a5-156">Optional and Read-only and for OneDrive Personal only.</span></span>

### <a name="roles-property-values"></a><span data-ttu-id="c06a5-157">Valores de propriedades Roles</span><span class="sxs-lookup"><span data-stu-id="c06a5-157">Roles property values</span></span>

| <span data-ttu-id="c06a5-158">Valor</span><span class="sxs-lookup"><span data-stu-id="c06a5-158">Value</span></span>              | <span data-ttu-id="c06a5-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="c06a5-159">Description</span></span>                                                                        |
|:------------------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="c06a5-160">leitura</span><span class="sxs-lookup"><span data-stu-id="c06a5-160">read</span></span>            | <span data-ttu-id="c06a5-161">Oferece a capacidade de ler os metadados e o conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="c06a5-161">Provides the ability to read the metadata and contents of the item.</span></span>            |
| <span data-ttu-id="c06a5-162">gravação</span><span class="sxs-lookup"><span data-stu-id="c06a5-162">write</span></span>           | <span data-ttu-id="c06a5-163">Oferece a capacidade de ler e modificar os metadados e o conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="c06a5-163">Provides the ability to read and modify the metadata and contents of the item.</span></span> |
| <span data-ttu-id="c06a5-164">owner</span><span class="sxs-lookup"><span data-stu-id="c06a5-164">owner</span></span>           | <span data-ttu-id="c06a5-165">Para o SharePoint e o OneDrive for Business, isso representa a função de proprietário.</span><span class="sxs-lookup"><span data-stu-id="c06a5-165">For SharePoint and OneDrive for Business this represents the owner role.</span></span>       |

<span data-ttu-id="c06a5-166">O recurso permission usa _facetas_ para fornecer informações sobre o tipo de permissão representado pelo recurso.</span><span class="sxs-lookup"><span data-stu-id="c06a5-166">The permission resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="c06a5-167">Os links de compartilhamento contêm um token exclusivo e necessário para acessar o item.</span><span class="sxs-lookup"><span data-stu-id="c06a5-167">Sharing links contain a unique token required to access the item.</span></span>

<span data-ttu-id="c06a5-168">Permissões com uma faceta [**invitation**][SharingInvitation] representam permissões adicionadas convidando usuários ou grupos específicos para ter acesso ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="c06a5-168">Permissions with an [**invitation**][SharingInvitation] facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

## <a name="sharing-links"></a><span data-ttu-id="c06a5-169">Links de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="c06a5-169">Sharing links</span></span>

<span data-ttu-id="c06a5-170">Permissões com uma faceta [**link**][SharingLink] representam links de compartilhamento criados no item.</span><span class="sxs-lookup"><span data-stu-id="c06a5-170">Permissions with a [**link**][SharingLink] facet represent sharing links created on the item.</span></span>
<span data-ttu-id="c06a5-171">Estes são os tipos mais comuns de permissões.</span><span class="sxs-lookup"><span data-stu-id="c06a5-171">These are the most common kinds of permissions.</span></span>
<span data-ttu-id="c06a5-172">Os links de compartilhamento fornecem uma URL exclusiva que pode ser usada para acessar um arquivo ou pasta.</span><span class="sxs-lookup"><span data-stu-id="c06a5-172">Sharing links provide a unique URL that can be used to access a file or folder.</span></span>
<span data-ttu-id="c06a5-173">Eles podem ser configurados para conceder acesso de várias maneiras.</span><span class="sxs-lookup"><span data-stu-id="c06a5-173">They can be set up to grant access in a variety of ways.</span></span>
<span data-ttu-id="c06a5-174">Por exemplo, você pode usar a API [createLink][] para criar um link que funcione para qualquer pessoa conectada à sua organização ou criar um link que funcione para qualquer pessoa, sem precisar fazer logon.</span><span class="sxs-lookup"><span data-stu-id="c06a5-174">For example, you can use the [createLink][] API to create a link that works for anyone signed into your organization, or you can create a link that works for anyone, without needing to sign in.</span></span>
<span data-ttu-id="c06a5-175">Você pode usar a API [invite][] para criar um link que funcione apenas para pessoas específicas, estejam elas na sua empresa ou não.</span><span class="sxs-lookup"><span data-stu-id="c06a5-175">You can use the [invite][] API to create a link that only works for specific people, whether they're in your company or not.</span></span>

<span data-ttu-id="c06a5-176">Aqui estão alguns exemplos de links de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="c06a5-176">Here are some examples of sharing links.</span></span>

### <a name="view-link"></a><span data-ttu-id="c06a5-177">Link Exibir</span><span class="sxs-lookup"><span data-stu-id="c06a5-177">View link</span></span>

<span data-ttu-id="c06a5-178">Este link de exibição fornece acesso somente leitura a qualquer pessoa com o link.</span><span class="sxs-lookup"><span data-stu-id="c06a5-178">This view link provides read-only access to anyone with the link.</span></span>

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

### <a name="edit-link"></a><span data-ttu-id="c06a5-179">Editar link</span><span class="sxs-lookup"><span data-stu-id="c06a5-179">Edit link</span></span>

<span data-ttu-id="c06a5-180">Este link de edição fornece acesso de leitura e gravação a qualquer pessoa na organização com o link.</span><span class="sxs-lookup"><span data-stu-id="c06a5-180">This edit link provides read and write access to anyone in the organization with the link.</span></span>

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

### <a name="existing-access-link"></a><span data-ttu-id="c06a5-181">Link de acesso existente</span><span class="sxs-lookup"><span data-stu-id="c06a5-181">Existing access link</span></span>

<span data-ttu-id="c06a5-182">Este link não concede privilégios adicionais ao usuário.</span><span class="sxs-lookup"><span data-stu-id="c06a5-182">This link does not grant any additional privileges to the user.</span></span>

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

### <a name="specific-people-link"></a><span data-ttu-id="c06a5-183">Link de pessoas específicas</span><span class="sxs-lookup"><span data-stu-id="c06a5-183">Specific people link</span></span>

<span data-ttu-id="c06a5-184">Este link fornece acesso de leitura e gravação para as pessoas específicas na coleção `grantedToIdentities`.</span><span class="sxs-lookup"><span data-stu-id="c06a5-184">This link provides read and write access to the specific people in the `grantedToIdentities` collection.</span></span>

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

## <a name="sharing-invitations"></a><span data-ttu-id="c06a5-185">Compartilhamento de convites</span><span class="sxs-lookup"><span data-stu-id="c06a5-185">Sharing invitations</span></span>

<span data-ttu-id="c06a5-186">Permissões enviadas pela [API][] [de][] convite ou concessão podem ter informações adicionais na faceta [][convite SharingInvitation] para endereços de email que não corresponderem a uma conta conhecida.</span><span class="sxs-lookup"><span data-stu-id="c06a5-186">Permissions sent by the [invite][] or [grant][] API can have additional information in the [invitation][SharingInvitation] facet for email addresses that don't match a known account.</span></span> <span data-ttu-id="c06a5-187">Nesses casos, a propriedade **grantedTo** pode não ser definida até que o link de convite seja resgatado, o que ocorre na primeira vez que o usuário clica no link e faz logona.</span><span class="sxs-lookup"><span data-stu-id="c06a5-187">In such cases, the **grantedTo** property might not be set until the invitation link is redeemed, which occurs the first time the user clicks the link and signs in.</span></span>

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

<span data-ttu-id="c06a5-188">Depois que o convite de compartilhamento tiver sido resgatado por um usuário, a propriedade **grantedTo** conterá as informações sobre a conta que resgatou as permissões:</span><span class="sxs-lookup"><span data-stu-id="c06a5-188">After the sharing invitation has been redeemed by a user, the **grantedTo** property will contain the information about the account that redeemed the permissions:</span></span>

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

## <a name="methods"></a><span data-ttu-id="c06a5-189">Métodos</span><span class="sxs-lookup"><span data-stu-id="c06a5-189">Methods</span></span>

| <span data-ttu-id="c06a5-190">Método</span><span class="sxs-lookup"><span data-stu-id="c06a5-190">Method</span></span>                                                   | <span data-ttu-id="c06a5-191">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="c06a5-191">REST Path</span></span>
|:---------------------------------------------------------|:-----------------------
| [<span data-ttu-id="c06a5-192">Listar permissões</span><span class="sxs-lookup"><span data-stu-id="c06a5-192">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="c06a5-193">Obter permissão</span><span class="sxs-lookup"><span data-stu-id="c06a5-193">Get permission</span></span>](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| <span data-ttu-id="c06a5-194">[Criar link][createLink]</span><span class="sxs-lookup"><span data-stu-id="c06a5-194">[Create link][createLink]</span></span>                                | `POST /drive/items/{item-id}/createLink`
| <span data-ttu-id="c06a5-195">[Convidar pessoas][invite]</span><span class="sxs-lookup"><span data-stu-id="c06a5-195">[Invite people][invite]</span></span>                                  | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="c06a5-196">Atualizar</span><span class="sxs-lookup"><span data-stu-id="c06a5-196">Update</span></span>](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="c06a5-197">Delete</span><span class="sxs-lookup"><span data-stu-id="c06a5-197">Delete</span></span>](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="c06a5-198">Adicionar usuários ao link de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="c06a5-198">Add users to sharing link</span></span>](../api/permission-grant.md)  | `POST /shares/{encoded-sharing-url}/permission/grant`
| [<span data-ttu-id="c06a5-199">Revogar concessões</span><span class="sxs-lookup"><span data-stu-id="c06a5-199">Revoke grants</span></span>](../api/permission-revokegrants.md)   | `POST /drive/items/{item-id}/permissions/{id}/revokeGrants`

[createLink]: ../api/driveitem-createlink.md
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
