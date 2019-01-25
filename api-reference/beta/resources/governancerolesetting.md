---
title: tipo de recurso de governanceRoleSetting
description: " regra e assim por diante."
localization_priority: Normal
ms.openlocfilehash: a52769d4714608df11bdde826ca37907d7942e4e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508164"
---
# <a name="governancerolesetting-resource-type"></a>tipo de recurso de governanceRoleSetting

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um conjunto de configurações em cada definição de função que precisa ser avaliada quando as atribuições de função são criadas ou modificadas. Por exemplo, configurações de função podem incluir "Duração máxima de atribuição" regra, a regra "MFA necessários na ativação" e assim por diante.

## <a name="methods"></a>Métodos

| Método          | Tipo de retorno |Descrição|
|:---------------|:--------|:--------|
|[List](../api/governancerolesetting-list.md) | coleção [governanceRoleSetting](../resources/governancerolesetting.md)|Uma coleção de definições de função em um recurso de lista.|
|[Get](../api/governancerolesetting-get.md) |  [governanceRoleSetting](../resources/governancerolesetting.md) |Leia as propriedades e os relacionamentos de uma configuração de função.|
|[Update](../api/governancerolesetting-update.md) | [governanceRoleSetting](../resources/governancerolesetting.md)  |Atualize um objeto de configuração de função. |

## <a name="properties"></a>Propriedades
|Propriedade               |Tipo                                      |Descrição|
|:--------------------|:---------------------------------------|:----------|
|id                   |String                                  |A identificação do roleSetting.|
|resourceId           |Cadeia de caracteres                                  |Obrigatório. A identificação do recurso que a configuração da função está associada.|
|roleDefinitionId     |String                                  |Obrigatório. A id da definição de função que a configuração da função está associada.|
|isDefault            |Booliano                                 |Somente leitura. Indique se o roleSetting é um roleSetting padrão|
|lastUpdatedDateTime  |DateTimeOffset                          |Somente leitura. A hora em que a configuração de funções foi atualizada pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|lastUpdatedBy        |String                                  |Somente leitura. O nome de exibição do administrador que atualizada pela última vez o roleSetting.|
|adminEligibleSettings|coleção [governanceRuleSetting](../resources/governancerulesetting.md)|As definições de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função elegíveis.|
|adminMemberSettings  |coleção [governanceRuleSetting](../resources/governancerulesetting.md)|As definições de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função de membro direto.|
|userEligibleSettings |coleção [governanceRuleSetting](../resources/governancerulesetting.md)|As definições de regra que são avaliadas quando um usuário tentar adicionar uma atribuição de função elegíveis. A configuração não é suportada por enquanto.|
|userMemberSettings   |coleção [governanceRuleSetting](../resources/governancerulesetting.md)|As definições de regra que são avaliadas quando um usuário tentar ativar sua atribuição de função.|

## <a name="relationships"></a>Relacionamento
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|recurso|[governanceResource](../resources/governanceresource.md)|Somente leitura. O recurso associado para esta definição de função.|
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Somente leitura. A definição de função que é imposta com essa definição de função. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
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
  "suppressions": [
    "Error: /api-reference/beta/resources/governancerolesetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
