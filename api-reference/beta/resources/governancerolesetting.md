---
title: Tipo de recurso governanceRoleSetting
description: Representa um conjunto de configurações em cada definição de função que precisa ser avaliada quando as atribuições de função são criadas ou modificadas.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: carolinetempleton
ms.openlocfilehash: af49836d52659b6f75727008599aea1ca16d5206
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688167"
---
# <a name="governancerolesetting-resource-type"></a>Tipo de recurso governanceRoleSetting

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v1resourceroles-deprecation](../../includes/pim-v1resourceroles-deprecation.md)]

Representa um conjunto de configurações em cada definição de função que precisa ser avaliada quando as atribuições de função são criadas ou modificadas. Por exemplo, as configurações de função podem incluir a regra "duração máxima da atribuição", a regra "MFA necessária na ativação" e assim por diante.

## <a name="methods"></a>Methods

| Método          | Tipo de retorno |Descrição|
|:---------------|:--------|:--------|
|[List](../api/governancerolesetting-list.md) | [Coleção governanceRoleSetting](../resources/governancerolesetting.md)|Listar uma coleção de configurações de função em um recurso.|
|[Obter](../api/governancerolesetting-get.md) |  [governanceRoleSetting](../resources/governancerolesetting.md) |Ler propriedades e relações de uma configuração de função.|
|[Atualizar](../api/governancerolesetting-update.md) | [governanceRoleSetting](../resources/governancerolesetting.md)  |Atualizar um objeto de configuração de função. |

## <a name="properties"></a>Propriedades
|Propriedade               |Tipo                                      |Descrição|
|:--------------------|:---------------------------------------|:----------|
|id                   |String                                  |A id da roleSetting.|
|resourceId           |String                                  |Obrigatório. A id do recurso ao que a configuração de função está associada.|
|roleDefinitionId     |String                                  |Obrigatório. A id da definição de função à que a configuração de função está associada.|
|isDefault            |Booliano                                 |Somente leitura. Indicar se roleSetting é uma roleSetting padrão|
|lastUpdatedDateTime  |DateTimeOffset                          |Somente leitura. A hora em que a configuração de função foi atualizada pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|lastUpdatedBy        |String                                  |Somente leitura. O nome de exibição do administrador que atualizou pela última vez a funçãoSetting.|
|adminEligibleSettings|[Coleção governanceRuleSetting](../resources/governancerulesetting.md)|As configurações de regra avaliadas quando um administrador tenta adicionar uma atribuição de função qualificada.|
|adminMemberSettings  |[Coleção governanceRuleSetting](../resources/governancerulesetting.md)|As configurações de regra avaliadas quando um administrador tenta adicionar uma atribuição de função de membro direto.|
|userEligibleSettings |[Coleção governanceRuleSetting](../resources/governancerulesetting.md)|As configurações de regra avaliadas quando um usuário tenta adicionar uma atribuição de função qualificada. A configuração não tem suporte por enquanto.|
|userMemberSettings   |[Coleção governanceRuleSetting](../resources/governancerulesetting.md)|As configurações de regra avaliadas quando um usuário tenta ativar sua atribuição de função.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|recurso|[governanceResource](../resources/governanceresource.md)|Somente leitura. O recurso associado para essa configuração de função.|
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Apenas leitura. A definição de função que é imposta com essa configuração de função. |

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


