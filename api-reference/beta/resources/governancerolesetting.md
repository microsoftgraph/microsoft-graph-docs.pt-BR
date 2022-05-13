---
title: Tipo de recurso governanceRoleSetting
description: Representa um conjunto de configurações em cada definição de função que precisa ser avaliada quando as atribuições de função são criadas ou modificadas.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: d5e441b35cd4b6ccdb52710508bd8afe5955d860
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2022
ms.locfileid: "65399465"
---
# <a name="governancerolesetting-resource-type"></a>Tipo de recurso governanceRoleSetting

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

Representa um conjunto de configurações em cada definição de função que precisa ser avaliada quando as atribuições de função são criadas ou modificadas. Por exemplo, as configurações de função podem incluir a regra "duração máxima da atribuição", a regra "MFA necessária na ativação" e assim por diante.

## <a name="methods"></a>Métodos

| Método          | Tipo de retorno |Descrição|
|:---------------|:--------|:--------|
|[Listar](../api/governancerolesetting-list.md) | [coleção governanceRoleSetting](../resources/governancerolesetting.md)|Listar uma coleção de configurações de função em um recurso.|
|[Get](../api/governancerolesetting-get.md) |  [governanceRoleSetting](../resources/governancerolesetting.md) |Ler propriedades e relações de uma configuração de função.|
|[Atualizar](../api/governancerolesetting-update.md) | [governanceRoleSetting](../resources/governancerolesetting.md)  |Atualizar um objeto de configuração de função. |

## <a name="properties"></a>Propriedades
|Propriedade               |Tipo                                      |Descrição|
|:--------------------|:---------------------------------------|:----------|
|id                   |Cadeia de caracteres                                  |A ID da roleSetting.|
|resourceId           |Cadeia de caracteres                                  |Obrigatório. A ID do recurso ao qual a configuração de função está associada.|
|roleDefinitionId     |Cadeia de caracteres                                  |Obrigatório. A ID da definição de função à qual a configuração de função está associada.|
|isDefault            |Booliano                                 |Somente leitura. Indicar se roleSetting é um roleSetting padrão|
|lastUpdatedDateTime  |DateTimeOffset                          |Somente leitura. A hora em que a configuração de função foi atualizada pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|lastUpdatedBy        |String                                  |Somente leitura. O nome de exibição do administrador que atualizou a roleSetting pela última vez.|
|adminEligibleSettings|[coleção governanceRuleSetting](../resources/governancerulesetting.md)|As configurações de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função qualificada.|
|adminMemberSettings  |[coleção governanceRuleSetting](../resources/governancerulesetting.md)|As configurações de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função de membro direto.|
|userEligibleSettings |[coleção governanceRuleSetting](../resources/governancerulesetting.md)|As configurações de regra que são avaliadas quando um usuário tenta adicionar uma atribuição de função qualificada. Por enquanto, não há suporte para a configuração.|
|userMemberSettings   |[coleção governanceRuleSetting](../resources/governancerulesetting.md)|As configurações de regra que são avaliadas quando um usuário tenta ativar sua atribuição de função.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|recurso|[governanceResource](../resources/governanceresource.md)|Somente leitura. O recurso associado para essa configuração de função.|
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Somente leitura. A definição de função que é imposta com essa configuração de função. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleSetting"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "isDefault": true,
  "lastUpdatedDateTime": "String (timestamp)",
  "lastUpdatedBy": "String",
  "adminEligibleSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "adminMemberSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "userEligibleSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}],
  "userMemberSettings": [{"@odata.type": "microsoft.graph.governanceRuleSetting"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


