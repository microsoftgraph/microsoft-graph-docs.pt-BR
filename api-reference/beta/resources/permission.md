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
# <a name="permission-resource-type"></a>Tipo de recurso permission

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **Permission** fornece informações sobre uma permissão de compartilhamento concedida a um recurso [DriveItem](driveitem.md).

As permissões de compartilhamento têm várias formas diferentes.
O recurso **Permission** representa estes diferentes formatos por meio de facetas do recurso.

>**Observação:** OneDrive para negócios e SharePoint bibliotecas de documentos não retornou a propriedade **inheritedFrom** .

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
| grantedToIdentities | Coleção ([IdentitySet][]) | Para obter permissões de tipo de link, os detalhes dos usuários aos quais a permissão foi concedida. Somente leitura.
| invitation          | [SharingInvitation][]       | Detalhes de um convite de compartilhamento associado para esta permissão. Somente leitura.
| inheritedFrom       | [ItemReference][]           | Fornece uma referência para o ancestral da permissão atual, se ela for herdada de um ancestral. Somente leitura.
| vínculo                | [SharingLink][]             | Fornece os detalhes do link de permissão atual, caso se trate de permissões de tipo de link. Somente leitura.
| funções               | Collection(String)          | O tipo de permissão, por exemplo, `read`. Veja abaixo a lista completa de funções. Somente leitura.
| shareId             | String                      | Um token exclusivo que pode ser usado para acessar esse item compartilhado por meio da ** [API][] Shares**. Somente leitura.
| expirationDateTime  | DateTimeOffset              | Um formato AAAA-MM-ddTHH:mm:ssZ de DateTimeOffset indica a hora de expiração da permissão. DateTime.MinValue indica que existem é nenhum vencimento definido para esta permissão. Opcional.
| HasPassword         | Booliano                     | Isso indica que se a senha é definida para esta permissão, ele só Mostrar em resposta. Opcional e somente leitura e para OneDrive pessoal somente.

### <a name="roles-enumeration-values"></a>Valores de enumeração de funções

| Valor        | Detalhes                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | Fornece a capacidade de ler os metadados e o conteúdo do item.            |
| `write`     | Fornece a capacidade de ler e modificar os metadados e o conteúdo do item. |
| `sp.owner`  | Para o SharePoint e o OneDrive for Business, isso representa a função de proprietário.       |
| `sp.member` | Para o SharePoint e o OneDrive for Business, isso representa a função de membro.      |

O recurso permission usa _facetas_ para fornecer informações sobre o tipo de permissão representado pelo recurso.

Links de compartilhamento contêm um token exclusivo necessário para acessar o item.

Permissões com uma faceta [**invitation**][SharingInvitation] representam permissões adicionadas convidando usuários ou grupos específicos para ter acesso ao arquivo.

## <a name="sharing-links"></a>Links de compartilhamento

Permissões com um [**link**][SharingLink] faceta representam que compartilhamento links criados no item.
Esses são os tipos mais comuns de permissões.
Compartilhamento de links fornecem uma URL exclusiva que pode ser usada para acessar um arquivo ou pasta.
Eles podem ser configurados para conceder acesso de várias maneiras.
Por exemplo, você pode usar o [createLink][] API para criar um link que funciona para qualquer pessoa entrado na sua organização, ou você pode criar um link que funciona para qualquer pessoa, sem precisar entrar.
Você pode usar a [Convidar][] API para criar um link que funciona somente para pessoas específicas, se eles estiverem em sua empresa ou não.

Aqui estão alguns exemplos de links de compartilhamento.

### <a name="view-link"></a>Link de exibição

Este link Exibir fornece acesso somente leitura para qualquer pessoa com o link.

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

### <a name="edit-link"></a>Link de edição

Este link Editar fornece acesso de leitura e gravação para qualquer pessoa da organização com o link.

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

### <a name="specific-people-link"></a>Link de pessoas específicas

Este link fornece acesso de leitura e gravação para as pessoas específicas no `grantedToIdentities` conjunto.

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

## <a name="sharing-invitations"></a>Convites de compartilhamento

Permissões enviadas pela [Convidar][] API podem ter informações adicionais no aspecto de[SharingInvitation] [convite].
Se um convite foi enviado a um endereço de email que não corresponda a uma conta conhecida, a propriedade **grantedTo** não pode ser definida até que o convite for trocado, o que ocorre na primeira vez em que o usuário clica no link e entra no.

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
| [Link Criar] [createLink]                                | `POST /drive/items/{item-id}/createLink`
| [Convidar pessoas] [Convidar]                                  | `POST /drive/items/{item-id}/invite`
| [Update](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [Delete](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`



[createLink]: ../api/driveitem-createlink.md
[IdentitySet]: identityset.md
[Convidar]: ../api/driveitem-invite.md
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
  "suppressions": [
    "Error: /api-reference/beta/resources/permission.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
