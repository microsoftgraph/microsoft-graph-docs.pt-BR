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
# <a name="permission-resource-type"></a>tipo de recurso Permission

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **Permission** fornece informações sobre uma permissão de compartilhamento concedida para um recurso [driveItem](driveitem.md) .

As permissões de compartilhamento têm várias formas diferentes.
O recurso **Permission** representa esses diferentes formatos através de facetas no recurso.

>**Observação:** As bibliotecas de documentos do OneDrive for Business e do SharePoint não retornam a propriedade **inheritedFrom** .

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
| grantedToIdentities | Coleção([IdentitySet][]) | Para permissões de tipo de link, os detalhes dos usuários aos quais a permissão foi concedida. Somente leitura.
| invitation          | [SharingInvitation][]       | Detalhes de um convite de compartilhamento associado para esta permissão. Somente leitura.
| inheritedFrom       | [ItemReference][]           | Fornece uma referência para o ancestral da permissão atual, se ela for herdada de um ancestral. Somente leitura.
| vínculo                | [SharingLink][]             | Fornece os detalhes do link de permissão atual, caso se trate de permissões de tipo de link. Somente leitura.
| funções               | Collection(String)          | O tipo de permissão, por exemplo, `read`. Veja abaixo a lista completa de funções. Somente leitura.
| shareId             | Cadeia de caracteres                      | Um token exclusivo que pode ser usado para acessar esse item compartilhado por meio da **[API de compartilhamentos][]**. Somente leitura.
| expirationDateTime  | DateTimeOffset              | Um formato de yyyy-MM-ddTHH: mm: ssZ de DateTimeOffset indica o tempo de expiração da permissão. DateTime. MinValue indica que não há validade configurada para essa permissão. Opcional.
| hasPassword         | Booliano                     | Isso indica se a senha está definida para essa permissão, ela só será mostrada em resposta. Opcional e somente leitura e somente para o OneDrive Personal.

### <a name="roles-enumeration-values"></a>Valores de enumeração de funções

| Valor        | Detalhes                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | Fornece a capacidade de ler os metadados e o conteúdo do item.            |
| `write`     | Fornece a capacidade de ler e modificar os metadados e o conteúdo do item. |
| `sp.owner`  | Para o SharePoint e o OneDrive for Business, isso representa a função de proprietário.       |
| `sp.member` | Para o SharePoint e o OneDrive for Business, isso representa a função de membro.      |

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

### <a name="view-link"></a>Link de exibição

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

Este link não concede nenhum privilégio adicional para o usuário.

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

## <a name="sharing-invitations"></a>Compartilhar convites

As permissões enviadas pelo [convite][] ou pela API de [concessão][] podem ter informações adicionais na faceta[SharingInvitation] do [convite]para endereços de email que não correspondem a uma conta conhecida. Nesses casos, a propriedade **concedidoto** pode não ser definida até que o link do convite seja resgatado, que ocorre na primeira vez que o usuário clica no link e entrar.

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


[createLink]: ../api/driveitem-createlink.md
[conceder]: ../api/permission-grant.md
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
