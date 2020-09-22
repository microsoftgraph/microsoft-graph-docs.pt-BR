---
title: tipo de recurso externalGroupMember
description: Representa um membro de um grupo externo usado para definir permissões no conteúdo externo adicionado ao Microsoft Graph.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 19b5c5094501215cc3ffd3e852ba6ca427807988
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193810"
---
# <a name="externalgroupmember-resource-type"></a>tipo de recurso externalGroupMember

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um membro de um grupo [externo](externalgroup.md) usado para definir permissões no conteúdo externo adicionado ao Microsoft Graph.

## <a name="methods"></a>Methods

| Método                                                              | Tipo de retorno         | Descrição                              |
|:--------------------------------------------------------------------|:--------------------|:-----------------------------------------|
| [Criar externalGroupMember](../api/externalgroup-post-members.md) | externalGroupMember | Criar um novo objeto **externalGroupMember** . |
| [Excluir externalGroupMember](../api/externalgroupmember-delete.md)  | Nenhum                | Excluir um objeto **externalGroupMember** .   |

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo                    | Descrição                                                          |
|:---------------|:------------------------|:---------------------------------------------------------------------|
| id             | String                  | A identificação exclusiva do membro. Seria o objectId em caso de usuários ou grupos do Active Directory do Azure e a propriedade **ID** do grupo **externo** no caso de grupos externos.                                    |
| tipo           | externalGroupMemberType | O tipo de membro adicionado ao grupo externo. Os valores possíveis são: `user` ou `group` quando **IdentityName** é `azureActiveDirectory` e apenas `group` quando **IdentityName** é `external` . |
| identificação da identidade | identitySourceType      | A origem de identidade à qual o membro pertence. Os valores possíveis são: `azureActiveDirectory`, `external`.                                                                                         |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalGroupMember",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "String (identifier)",
  "type": "String",
  "identitySource": "String"
}
```
