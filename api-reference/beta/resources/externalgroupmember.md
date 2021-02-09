---
title: Tipo de recurso externalGroupMember
description: Representa um membro de um externalGroup usado para definir permissões em conteúdo externo adicionado ao Microsoft Graph.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 1e86fb275b941b7a3033999fedd4c71aa3ac1de1
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161688"
---
# <a name="externalgroupmember-resource-type"></a>Tipo de recurso externalGroupMember

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um membro de um [externalGroup](externalgroup.md) usado para definir permissões em conteúdo externo adicionado ao Microsoft Graph.

## <a name="methods"></a>Métodos

| Método                                                              | Tipo de retorno         | Descrição                              |
|:--------------------------------------------------------------------|:--------------------|:-----------------------------------------|
| [Criar externalGroupMember](../api/externalgroup-post-members.md) | externalGroupMember | Criar um novo **objeto externalGroupMember.** |
| [Excluir externalGroupMember](../api/externalgroupmember-delete.md)  | Nenhum(a)                | **Exclua um objeto externalGroupMember.**   |

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo                    | Descrição                                                          |
|:---------------|:------------------------|:---------------------------------------------------------------------|
| id             | String                  | A ID exclusiva do membro. Seria o objectId no caso de usuários ou grupos do Azure Active Directory e a propriedade **de id** do **externalGroup** no caso de grupos externos.                                    |
| type           | externalGroupMemberType | O tipo de membro adicionado ao grupo externo. Os valores `user` possíveis são: `group` ou quando **identitySource** é `azureActiveDirectory` e apenas quando `group` **identitySource** é `external` . |
| identitySource | identitySourceType      | A fonte de identidade à que o membro pertence. Os valores possíveis são: `azureActiveDirectory`, `external`.                                                                                         |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalGroupMember",
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
