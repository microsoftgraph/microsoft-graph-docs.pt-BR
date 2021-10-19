---
author: JeremyKelley
title: tipo de recurso de permissão
description: recurso permission representando uma permissão de compartilhamento concedida para um driveItem
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f2b58acc06b1a7478c2728f8e371fee67e917d3e
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/19/2021
ms.locfileid: "60493470"
---
# <a name="permission-resource-type"></a>tipo de recurso de permissão

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O **recurso de** permissão fornece informações sobre uma permissão de compartilhamento concedida para um recurso [driveItem.](driveitem.md)

As permissões de compartilhamento têm várias formas diferentes.
O **recurso de** permissão representa esses diferentes formulários por meio de facetas no recurso.

>**Observação:** OneDrive for Business e SharePoint de documentos não retornam a **propriedade inheritedFrom.**

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

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

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo                        | Descrição
|:--------------------|:----------------------------|:-------------------------
| id                  | String                      | O identificador exclusivo da permissão entre todas as permissões no item. Somente leitura.
| grantedTo           | [IdentitySet][]             | Para permissões de tipo de usuário, os detalhes de usuários e aplicativos para esta permissão. Somente leitura.
| grantedToIdentities | Coleção([IdentitySet][]) | Para permissões de tipo de link, os detalhes dos usuários a quem a permissão foi concedida. Somente leitura.
| invitation          | [SharingInvitation][]       | Detalhes de um convite de compartilhamento associado para esta permissão. Somente leitura.
| inheritedFrom       | [ItemReference][]           | Fornece uma referência para o ancestral da permissão atual, se ela for herdada de um ancestral. Somente leitura.
| vínculo                | [SharingLink][]             | Fornece os detalhes do link de permissão atual, caso se trate de permissões de tipo de link. Somente leitura.
| funções               | Collection(String)          | O tipo de permissão, por exemplo, `read`. Veja abaixo a lista completa de funções. Somente leitura.
| shareId             | Cadeia de caracteres                      | Um token exclusivo que pode ser usado para acessar este item compartilhado por meio da **[API de compartilhamentos][]**. Somente leitura.
| expirationDateTime  | DateTimeOffset              | Um formato yyyy-MM-ddTHH:mm:ssZ de DateTimeOffset indica o tempo de expiração da permissão. DateTime.MinValue indica que não há expiração definida para esta permissão. Opcional.
| hasPassword         | Boolean                     | Isso indica se a senha está configurada para esta permissão, está sendo exibida apenas em resposta. Opcional e Somente leitura e somente para o OneDrive Personal.

### <a name="roles-property-values"></a>Valores de propriedades Roles

| Valor              | Descrição                                                                        |
|:------------------|:-------------------------------------------------------------------------------|
| leitura            | Oferece a capacidade de ler os metadados e o conteúdo do item.            |
| gravação           | Oferece a capacidade de ler e modificar os metadados e o conteúdo do item. |
| proprietário           | Para o Microsoft Office SharePoint Online e o OneDrive for Business, este representa o papel do proprietário.       |

O recurso permission usa _facetas_ para fornecer informações sobre o tipo de permissão representado pelo recurso.

Os links de compartilhamento contêm um token exclusivo e necessário para acessar o item.

Permissões com uma faceta [**invitation**][SharingInvitation] representam permissões adicionadas convidando usuários ou grupos específicos para ter acesso ao arquivo.

## <a name="sharing-links"></a>Links de compartilhamento

Permissões com uma faceta [**link**][SharingLink] representam links de compartilhamento criados no item.
Estes são os tipos mais comuns de permissões.
Os links de compartilhamento fornecem uma URL exclusiva que pode ser usada para acessar um arquivo ou pasta.
Eles podem ser configurados para conceder acesso de várias maneiras.
Por exemplo, você pode usar a API [createLink][] para criar um link que funcione para qualquer pessoa conectada à sua organização ou criar um link que funcione para qualquer pessoa, sem precisar fazer logon.
Você pode usar a API [invite][] para criar um link que funcione apenas para pessoas específicas, estejam elas na sua empresa ou não.

Aqui estão alguns exemplos de links de compartilhamento.

### <a name="view-link"></a>Link Exibir

Este link de exibição fornece acesso somente leitura a qualquer pessoa com o link.

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

### <a name="edit-link"></a>Editar link

Este link de edição fornece acesso de leitura e gravação a qualquer pessoa na organização com o link.

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

### <a name="existing-access-link"></a>Link de acesso existente

Este link não concede privilégios adicionais ao usuário.

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

### <a name="specific-people-link"></a>Link de pessoas específicas

Este link fornece acesso de leitura e gravação para as pessoas específicas na coleção `grantedToIdentities`.

<!-- {"blockType": "example", truncated: true, "@odata.type": "microsoft.graph.permission", "name": "permission-people-link" } -->

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

## <a name="sharing-invitations"></a>Compartilhamento de convites

Permissões enviadas pela [API][] [de][] convite ou concessão podem ter informações adicionais na faceta [][convite SharingInvitation] para endereços de email que não corresponderem a uma conta conhecida. Nesses casos, a propriedade **grantedTo** pode não ser definida até que o link de convite seja resgatado, o que ocorre na primeira vez que o usuário clica no link e faz logona.

<!-- {"blockType": "example", truncated: true, "@odata.type": "microsoft.graph.permission", "name": "permission-invite-email" } -->

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

Depois que o convite de compartilhamento tiver sido resgatado por um usuário, a propriedade **grantedTo** conterá as informações sobre a conta que resgatou as permissões:

<!-- {"blockType": "example", truncated: true,"@odata.type": "microsoft.graph.permission", "name": "permission-invite-redeemed" } -->

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

## <a name="methods"></a>Métodos

| Método                                                   | Caminho REST
|:---------------------------------------------------------|:-----------------------
| [Listar permissões](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [Obter permissão](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| [Criar link][createLink]                                | `POST /drive/items/{item-id}/createLink`
| [Convidar pessoas][invite]                                  | `POST /drive/items/{item-id}/invite`
| [Atualizar](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [Delete](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`
| [Adicionar usuários ao link de compartilhamento](../api/permission-grant.md)  | `POST /shares/{encoded-sharing-url}/permission/grant`
| [Revogar concessões](../api/permission-revokegrants.md)   | `POST /drive/items/{item-id}/permissions/{id}/revokeGrants`

[createLink]: ../api/driveitem-createlink.md
[grant]: ../api/permission-grant.md
[IdentitySet]: identityset.md
[invite]: ../api/driveitem-invite.md
[ItemReference]: itemreference.md
[API de compartilhamentos]: ../api/shares-get.md
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
