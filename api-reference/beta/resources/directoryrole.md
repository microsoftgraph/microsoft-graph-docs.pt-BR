---
title: tipo de recurso directoryRole
description: Representa uma função do diretório do Azure AD. As funções de diretório do AD do Azure também são conhecidas como *funções de administrador*. Para obter mais informações sobre funções de diretório (administrador), confira Atribuindo funções de administrador no Azure AD. Com o Microsoft Graph, você pode atribuir usuários a funções de diretório para conceder a eles as permissões da função de destino. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Apenas a função de diretório Administradores de Empresa é ativada por padrão. Para ativar outras funções de diretório disponíveis, você envia uma solicitação POST com a ID do directoryRoleTemplate no qual a função directory se baseia. Herda de directoryObject.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 30b22313da70c33bffc0b759f9b474f4deac2ac1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521247"
---
# <a name="directoryrole-resource-type"></a>tipo de recurso directoryRole

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma função do diretório do Azure AD. As funções de diretório do AD do Azure também são conhecidas como *funções de administrador*. Para obter mais informações sobre funções de diretório (administrador), confira [Atribuindo funções de administrador no Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/). Com o Microsoft Graph, você pode atribuir usuários a funções de diretório para conceder a eles as permissões da função de destino. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Apenas a função de diretório Administradores de Empresa é ativada por padrão. Para ativar outras funções de diretório disponíveis, você envia uma solicitação POST com a ID do [directoryRoleTemplate](directoryroletemplate.md) no qual a função directory se baseia. Herda de [directoryObject](directoryobject.md).

Por padrão, as funções de diretório limitam-se para ser todo o inquilino.  No entanto, funções de diretório (atualmente somente o *administrador da conta de usuário* e *Administração de assistência técnica*) podem também ser escopo [unidades administrativas](administrativeunit.md).

Esse recurso permite:

- Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/directoryrole-delta.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter directoryRole](../api/directoryrole-get.md) | [directoryRole](directoryrole.md) |Leia as propriedades e os relacionamentos do objeto directoryRole.|
|[Listar directoryRoles](../api/directoryrole-list.md) | Coleção [directoryRole](directoryrole.md) | Lista as funções de diretório ativadas no locatário. |
|[Adicionar membro](../api/directoryrole-post-members.md) |[directoryObject](directoryobject.md)| Adicione um usuário à função de diretório postando na propriedade de navegação de membros.|
|[Listar membros](../api/directoryrole-list-members.md) |Coleção [directoryObject](directoryobject.md)| Obtenha os usuários que são membros da função directory da propriedade de navegação members.|
|[Remover um membro](../api/directoryrole-delete-member.md) |[directoryObject](directoryobject.md)| Remova um usuário da função de diretório.|
|[Membros da função com escopo de lista](../api/directoryrole-list-members.md) |coleção [scopedRoleMembership](scopedrolemembership.md)| Lista os membros dessa função directory que têm como escopo para [unidades administrativas](administrativeunit.md), toda a coleção de recursos scopedRoleMembership.|
|[delta](../api/directoryrole-delta.md)|Coleção directoryRole| Obtenha as alterações incrementais para funções de diretório. |

## <a name="properties"></a>Propriedades
| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|description|Cadeia de caracteres|A descrição da função de diretório. Somente leitura. |
|displayName|String|O nome de exibição da função de diretório. Somente leitura. |
|id|String|O identificador exclusivo da função de diretório. Herdado de [directoryObject](directoryobject.md). Chave, Não Anulável, Somente Leitura.|
|roleTemplateId|String| A **id** do [directoryRoleTemplate](directoryroletemplate.md) em que esta função se baseia. A propriedade deve ser especificada ao ativar uma função de diretório em um locatário com uma operação POST. Depois que a função directory tiver sido ativada, a propriedade será somente leitura. |

## <a name="relationships"></a>Relações
| Relação | Tipo |Descrição|
|:---------------|:--------|:----------|
|membros|Coleção [directoryObject](directoryobject.md)|Usuários que são membros desta função de diretório. Métodos HTTP: GET, POST, DELETE. Somente leitura. Anulável.|
|scopedMembers|coleção [scopedRoleMembership](scopedrolemembership.md)| Membros da função diretório que têm o escopo para [unidades administrativas](administrativeunit.md). Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryRole"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "roleTemplateId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryrole.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
