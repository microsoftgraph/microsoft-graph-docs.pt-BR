---
title: tipo de recurso directoryRole
description: Representa uma função do diretório do Azure AD. As funções de diretório do AD do Azure também são conhecidas como *funções de administrador*.
ms.localizationpriority: high
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 051278a83d0d45a87ec397ca3c7fdf2fb80b1a24
ms.sourcegitcommit: bfd1ab7e015ef04cb2ca3fb85d308ba2ce830a89
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/19/2022
ms.locfileid: "62072660"
---
# <a name="directoryrole-resource-type"></a>tipo de recurso directoryRole

Namespace: microsoft.graph

Representa uma função de diretório do Azure AD. As funções de diretório do Azure AD também são conhecidas como *funções de administrador*. Para obter mais informações sobre as funções de diretório (administrador), consulte [Atribuir funções de administrador no Azure AD](/azure/active-directory/users-groups-roles/directory-assign-admin-roles). Com o Microsoft Graph, você pode atribuir usuários a funções de diretório para conceder a eles as permissões da função de destino. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Apenas a função do diretório Administradores da empresa é ativada por padrão. Para ativar outras funções de diretório disponíveis, você envia uma solicitação POST com a ID do [directoryRoleTemplate](directoryroletemplate.md) no qual a função de diretório é baseada. [Liste modelos de função de diretório](../api/directoryroletemplate-list.md) para obter todos os outros diretórios disponíveis. Herda de [directoryObject](directoryobject.md).

Esse recurso permite:

- Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/directoryrole-delta.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter directoryRole](../api/directoryrole-get.md) | [directoryRole](directoryrole.md) | Leia as propriedades e os relacionamentos do objeto directoryRole. |
|[Listar directoryRoles](../api/directoryrole-list.md) | Coleção [directoryRole](directoryrole.md) | Lista as funções de diretório ativadas no locatário. |
|[Adicionar membro](../api/directoryrole-post-members.md) |[directoryObject](directoryobject.md)| Adicione um usuário à função de diretório postando na propriedade de navegação de membros.|
|[Listar membros](../api/directoryrole-list-members.md) |Coleção [directoryObject](directoryobject.md)| Obtenha os usuários que são membros da função directory da propriedade de navegação members.|
|[Remover um membro](../api/directoryrole-delete-member.md) |[directoryObject](directoryobject.md)| Remova um usuário da função de diretório.|
|[Ativar directoryRole](../api/directoryrole-post-directoryroles.md) |[directoryRole](directoryrole.md) | Ative uma função de diretório.|
|[Lista de scopedMembers](../api/directoryrole-list-scopedmembers.md) |Coleção [scopedRoleMembership](scopedrolemembership.md)| Liste os membros desta função de diretório que têm como escopo as [unidades administrativas](administrativeunit.md), por meio da coleção de recursos scopedRoleMembership.|
|[delta](../api/directoryrole-delta.md)|Coleção directoryRole| Obtenha alterações incrementais para as funções de diretório. |

## <a name="properties"></a>Propriedades
| Propriedade   | Tipo | Descrição |
|:---------------|:--------|:----------|
|description|Cadeia de caracteres|A descrição da função de diretório. Somente leitura. Suporta `$filter` (`eq`), `$search`, `$select`. |
|displayName|Cadeia de caracteres|O nome de exibição da função de diretório. Somente leitura. Suporta `$filter` (`eq`), `$search`, `$select`. |
|id|Cadeia de caracteres|O identificador exclusivo da função de diretório. Herdado de [directoryObject](directoryobject.md). Chave, Não Anulável, Somente Leitura. Suporta `$filter` (`eq`), `$select`.|
|roleTemplateId|String| A **id** do [directoryRoleTemplate](directoryroletemplate.md) em que esta função se baseia. A propriedade deve ser especificada ao ativar uma função de diretório em um locatário com uma operação POST. Depois que a função directory tiver sido ativada, a propriedade será somente leitura. Suporta `$filter` (`eq`), `$select`. |

## <a name="relationships"></a>Relações
| Relação | Tipo |Descrição|
|:---------------|:--------|:----------|
|membros|Coleção [directoryObject](directoryobject.md)|Usuários que são membros desta função de diretório. Métodos HTTP: GET, POST, DELETE. Somente leitura. Anulável. Suporta o `$expand`.|
|scopedMembers|Coleção [scopedRoleMembership](scopedrolemembership.md)| Membros dessa função de diretório que têm como escopo [unidades administrativas](administrativeunit.md). Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.directoryRole",
  "@odata.annotations": [
    {
      "capabilities": {
        "toppable": false
      }
    }
  ]
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
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
