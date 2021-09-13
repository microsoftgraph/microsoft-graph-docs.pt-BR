---
title: Tipo de recurso conditionalAccessConditionSet
description: Representa o tipo de condições que regem quando a política se aplica.
ms.localizationpriority: medium
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 97a4f3079ccdf5f81cad16a15d31591e379b152b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109238"
---
# <a name="conditionalaccessconditionset-resource-type"></a>Tipo de recurso conditionalAccessConditionSet

Namespace: microsoft.graph

Representa o tipo de condições que regem quando a política se aplica.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|applications|[conditionalAccessApplications](conditionalaccessapplications.md)| Aplicativos e ações do usuário incluídas e excluídas da política. Obrigatório. |
|usuários|[conditionalAccessUsers](conditionalaccessusers.md)| Usuários, grupos e funções incluídos e excluídos da política. Obrigatório. |
|clientAppTypes|coleção conditionalAccessClientApp| Tipos de aplicativo cliente incluídos na política. Os possíveis valores são: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`. Obrigatório.|
|locations|[conditionalAccessLocations](conditionalaccesslocations.md)| Locais incluídos e excluídos da política. |
|plataformas|[conditionalAccessPlatforms](conditionalaccessplatforms.md)| Plataformas incluídas e excluídas da política. |
|signInRiskLevels|Coleção riskLevel| Níveis de risco de login incluídos na política. Os possíveis valores são: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`. Obrigatório.|
|userRiskLevels|Coleção riskLevel| Níveis de risco de usuário incluídos na política. Os possíveis valores são: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`. Obrigatório.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "clientAppTypes",
    "locations",
    "platforms",
    "signInRiskLevels",
    "userRiskLevels"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessConditionSet",
  "baseType": null
}-->

```json
{
  "applications": {"@odata.type": "microsoft.graph.conditionalAccessApplications"},
  "users": {"@odata.type": "microsoft.graph.conditionalAccessUsers"},
  "clientAppTypes": ["String"],
  "locations": {"@odata.type": "microsoft.graph.conditionalAccessLocations"},
  "platforms": {"@odata.type": "microsoft.graph.conditionalAccessPlatforms"},
  "signInRiskLevels": ["String"],
  "userRiskLevels": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessConditionSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

