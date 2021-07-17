---
title: Tipo de recurso externalGroupMember
description: Representa um membro de um externalGroup usado para definir permissões no conteúdo externo adicionado à Microsoft Graph.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e3626c718360982bf79cb9757a13e4b4c01669cd
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467568"
---
# <a name="externalgroupmember-resource-type"></a>Tipo de recurso externalGroupMember

Namespace: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um membro de [um externalGroup](externalconnectors-externalgroup.md) usado para definir permissões no conteúdo externo adicionado à Microsoft Graph.

## <a name="methods"></a>Métodos

| Método                                                              | Tipo de retorno         | Descrição                              |
|:--------------------------------------------------------------------|:--------------------|:-----------------------------------------|
| [Criar externalGroupMember](../api/externalconnectors-externalgroup-post-members.md) | [externalGroupMember](../resources/externalconnectors-externalgroupmember.md) | Crie um novo **objeto externalGroupMember.** |
| [Excluir externalGroupMember](../api/externalconnectors-externalgroupmember-delete.md)  | Nenhum                | **Exclua um objeto externalGroupMember.**   |

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo                    | Descrição                                                          |
|:---------------|:------------------------|:---------------------------------------------------------------------|
| id             | String                  | A ID exclusiva do membro. Seria objectId no caso de Azure Active Directory ou grupos e a propriedade **id** do **externalGroup** no caso de grupos externos.                                    |
| tipo           | microsoft.graph.externalConnectors.externalGroupMemberType | O tipo de membro adicionado ao grupo externo. Os valores possíveis são: `user` `group` ou quando **identitySource** é `azureActiveDirectory` e apenas quando `group` **identitySource** é `external` . |
| identitySource | microsoft.graph.externalConnectors.identitySourceType      | A fonte de identidade à que o membro pertence. Os valores possíveis são: `azureActiveDirectory`, `external`.                                                                                         |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.externalGroupMember",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "type": "String",
  "identitySource": "String"
}
```
