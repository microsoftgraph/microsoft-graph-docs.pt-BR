---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Permissão
localization_priority: Priority
description: O recurso Permission fornece informações sobre uma permissão de compartilhamento concedida a um recurso DriveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2fa13c414d45561110d1fa1310cfc913efec6118
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534062"
---
# <a name="permission-resource-type"></a>Tipo de recurso permission

Namespace: microsoft.graph

O recurso **Permission** fornece informações sobre uma permissão de compartilhamento concedida a um recurso [DriveItem](driveitem.md).

As permissões de compartilhamento têm várias formas diferentes.
O recurso **Permission** representa estes diferentes formulários por meio de facetas do recurso.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

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

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo                                      | Descrição
|:--------------|:------------------------------------------|:-----------------
| id            | String                                    | O identificador exclusivo da permissão entre todas as permissões no item. Somente leitura.
| grantedTo     | [IdentitySet](identityset.md)             | Para permissões de tipo de usuário, os detalhes de usuários e aplicativos para esta permissão. Somente leitura.
| invitation    | [SharingInvitation][]                     | Detalhes de um convite de compartilhamento associado para esta permissão. Somente leitura.
| inheritedFrom | [ItemReference](itemreference.md)         | Fornece uma referência para o ancestral da permissão atual, se ela for herdada de um ancestral. Somente leitura.
| vínculo          | [SharingLink][]                           | Fornece os detalhes do link de permissão atual, caso se trate de permissões de tipo de link. Somente leitura.
| funções         | Coleção de Cadeias de Caracteres                      | O tipo de permissão, por exemplo, `read`. Veja abaixo a lista completa de funções. Somente leitura.
| shareId       | Cadeia de caracteres                                    | Um token exclusivo que pode ser usado para acessar esse item compartilhado por meio da [**API** Shares](../api/shares-get.md). Somente leitura.

O recurso permission usa _facetas_ para fornecer informações sobre o tipo de permissão representado pelo recurso.

Permissões com uma faceta [**link**][SharingLink] representam links de compartilhamento criados no item. Os links de compartilhamento contêm um token exclusivo que fornece acesso ao item para qualquer pessoa com o link.

Permissões com uma faceta [**invitation**][SharingInvitation] representam permissões adicionadas convidando usuários ou grupos específicos para ter acesso ao arquivo.

[SharingInvitation]: sharinginvitation.md
[SharingLink]: sharinglink.md

## <a name="roles-enumeration"></a>Enumeração de funções

| Função        | Detalhes                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | Fornece a capacidade de ler os metadados e o conteúdo do item.            |
| `write`     | Fornece a capacidade de ler e modificar os metadados e o conteúdo do item. |
| `sp.owner`  | Para o SharePoint e o OneDrive for Business, isso representa a função de proprietário.       |
| `sp.member` | Para o SharePoint e o OneDrive for Business, isso representa a função de membro.      |

## <a name="sharing-links"></a>Links de compartilhamento
O tipo mais comum de permissões são os links de compartilhamento. Esses links fornecem uma URL exclusiva que inclui o recurso que está sendo compartilhado e um token de autenticação que fornece acesso ao recurso. Os usuários não precisam entrar para acessar o conteúdo compartilhado com um link de compartilhamento. Os usuários podem compartilhar um link que concede acesso somente leitura ou acesso de gravação ao conteúdo.

### <a name="view-link"></a>Link de exibição
Um link de exibição oferece acesso somente leitura a um item.

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

### <a name="edit-link"></a>Link de edição
Um link de edição fornece acesso de leitura e gravação a um item.

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

### <a name="sharing-invitation"></a>Convite de compartilhamento
Além de criar links de compartilhamento, um usuário pode ser convidado pelo endereço de email. Nesse cenário, a permissão cria um convite que é enviado ao email do usuário.

#### <a name="invitation-to-an-email-address"></a>Convite para um endereço de email
Se a permissão for enviada por meio do endereço de email para um destinatário que não tem uma conta correspondente, a propriedade **grantedTo** não poderá ser definida até que o convite seja resgatado, o que ocorre na primeira vez que um usuário clica no link e entra na sessão.

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

Depois que o convite de compartilhamento tiver sido resgatado por um usuário, a propriedade **grantedTo** conterá as informações sobre a conta que resgatou as permissões:

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

## <a name="methods"></a>Métodos

| Método                                                   | Caminho REST
|:---------------------------------------------------------|:-----------------------
| [Listar permissões](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [Obter permissão](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| [Adicionar](../api/driveitem-invite.md)                        | `POST /drive/items/{item-id}/invite`
| [Update](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [Delete](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`


## <a name="remarks"></a>Comentários

O OneDrive for Business e as bibliotecas de documentos do SharePoint não retornam a propriedade **inheritedFrom**.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The permission object provides information about permissions and roles and sharing information.",
  "keywords": "sharing,permissions,read,write,acl",
  "section": "documentation",
  "tocPath": "Resources/Permission"
} -->
