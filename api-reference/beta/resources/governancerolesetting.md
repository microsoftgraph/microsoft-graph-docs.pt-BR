---
title: tipo de recurso governanceRoleSetting
description: " regra e assim por diante."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 1bd1821bbb3336386b54b62ebe7b4787c85d1ebf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006420"
---
# <a name="governancerolesetting-resource-type"></a>tipo de recurso governanceRoleSetting

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um conjunto de configurações em cada definição de função que precisam ser avaliadas quando as atribuições de função são criadas ou modificadas. Por exemplo, as configurações de função podem incluir a regra "duração da atribuição máxima", regra "MFA necessária na ativação" e assim por diante.

## <a name="methods"></a>Métodos

| Método          | Tipo de retorno |Descrição|
|:---------------|:--------|:--------|
|[List](../api/governancerolesetting-list.md) | coleção [governanceRoleSetting](../resources/governancerolesetting.md)|Lista uma coleção de configurações de função em um recurso.|
|[Get](../api/governancerolesetting-get.md) |  [governanceRoleSetting](../resources/governancerolesetting.md) |Leia as propriedades e as relações de uma configuração de função.|
|[Atualização](../api/governancerolesetting-update.md) | [governanceRoleSetting](../resources/governancerolesetting.md)  |Atualize um objeto de configuração de função. |

## <a name="properties"></a>Propriedades
|Propriedade               |Tipo                                      |Descrição|
|:--------------------|:---------------------------------------|:----------|
|id                   |String                                  |A ID do roleSetting.|
|resourceId           |String                                  |Obrigatório. A ID do recurso ao qual a configuração de função está associada.|
|roleDefinitionId     |String                                  |Obrigatório. A ID da definição de função à qual a configuração de função está associada.|
|isDefault            |Booliano                                 |Somente leitura. Indica se o roleSetting é um padrão roleSetting|
|lastUpdatedDateTime  |DateTimeOffset                          |Somente leitura. A hora em que a configuração da função foi atualizada pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|lastUpdatedBy        |String                                  |Somente leitura. O nome de exibição do administrador que atualizou pela última vez o roleSetting.|
|adminEligibleSettings|coleção [governanceRuleSetting](../resources/governancerulesetting.md)|As configurações de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função qualificada.|
|adminMemberSettings  |coleção [governanceRuleSetting](../resources/governancerulesetting.md)|As configurações de regra que são avaliadas quando um administrador tenta adicionar uma atribuição de função de membro direto.|
|userEligibleSettings |coleção [governanceRuleSetting](../resources/governancerulesetting.md)|As configurações de regra que são avaliadas quando um usuário tenta adicionar uma atribuição de função qualificada. A configuração não é suportada por enquanto.|
|userMemberSettings   |coleção [governanceRuleSetting](../resources/governancerulesetting.md)|As configurações de regra que são avaliadas quando um usuário tenta ativar sua atribuição de função.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|recurso|[Entidadegovernanceresource](../resources/governanceresource.md)|Somente leitura. O recurso associado para esta configuração de função.|
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Somente leitura. A definição de função aplicada a essa configuração de função. |

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
