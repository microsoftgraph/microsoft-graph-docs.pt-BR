---
title: tipo de recurso directoryRole
description: Representa uma função de diretório do Windows Azure AD. Funções de diretório do Windows Azure AD também são conhecidos como *funções de administrador*. Para obter mais informações sobre as funções de diretório (administrador), consulte a atribuição de funções de administrador no Azure AD. Com o Microsoft Graph, você pode atribuir usuários a funções de diretório para conceder as permissões da função de destino. Para ler uma função de diretório ou atualizar seus membros, ele deve primeiro ser ativado no inquilino. Por padrão, apenas a função do diretório de administradores de empresa é ativada. Para ativar a outras funções de diretório disponíveis que você enviar uma solicitação POST com a ID do directoryRoleTemplate na qual a função de diretório se baseia. Herda de directoryObject.
localization_priority: Priority
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4b3379bbbecd86612043dcc3cb8455f5c43ba9cf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939543"
---
# <a name="directoryrole-resource-type"></a>tipo de recurso directoryRole

Representa uma função de diretório do Windows Azure AD. Funções de diretório do Windows Azure AD também são conhecidos como *funções de administrador*. Para obter mais informações sobre as funções de diretório (administrador), consulte [Atribuindo funções de administrador no Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/). Com o Microsoft Graph, você pode atribuir usuários a funções de diretório para conceder as permissões da função de destino. Para ler uma função de diretório ou atualizar seus membros, ele deve primeiro ser ativado no inquilino. Por padrão, apenas a função do diretório de administradores de empresa é ativada. Para ativar a outras funções de diretório disponíveis que você enviar uma solicitação POST com a ID de [directoryRoleTemplate](directoryroletemplate.md) na qual a função de diretório se baseia. Herda de [directoryObject](directoryobject.md).
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
|[delta](../api/directoryrole-delta.md)|Coleção directoryRole| Obtenha as alterações incrementais para funções de diretório. |

## <a name="properties"></a>Propriedades
| Propriedade   | Tipo | Descrição |
|:---------------|:--------|:----------|
|description|String|A descrição da função de diretório. Somente leitura. |
|displayName|String|O nome de exibição da função de diretório. Somente leitura. |
|id|String|O identificador exclusivo da função de diretório. Herdado de [directoryObject](directoryobject.md). Chave, Não Anulável, Somente Leitura.|
|roleTemplateId|String| A **id** do [directoryRoleTemplate](directoryroletemplate.md) em que esta função se baseia. A propriedade deve ser especificada ao ativar uma função de diretório em um locatário com uma operação POST. Depois que a função directory tiver sido ativada, a propriedade será somente leitura. |

## <a name="relationships"></a>Relações
| Relação | Tipo |Descrição|
|:---------------|:--------|:----------|
|membros|Coleção [directoryObject](directoryobject.md)|Usuários que são membros desta função de diretório. Métodos HTTP: GET, POST, DELETE. Somente leitura. Anulável.|

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
