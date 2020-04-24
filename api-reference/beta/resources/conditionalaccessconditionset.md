---
title: tipo de recurso conditionalAccessConditionSet
description: Representa o tipo de condições que controlam quando a política se aplica.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f5db4c6367834733a4a5fbbb6c7a8d6b08393160
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805676"
---
# <a name="conditionalaccessconditionset-resource-type"></a>tipo de recurso conditionalAccessConditionSet

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o tipo de condições que controlam quando a política se aplica.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|Emprego|[conditionalAccessApplications](conditionalaccessapplications.md)| Aplicativos e ações do usuário incluídos no e excluídos da política. Obrigatório. |
|usuários|[conditionalAccessUsers](conditionalaccessusers.md)| Usuários, grupos e funções incluídos no e excluídos da política. Obrigatório. |
|clientAppTypes|Coleção de cadeias de caracteres| Tipos de aplicativo cliente incluídos na política. Os valores possíveis são: `browser`, `modern`, `easSupported`, `easUnsupported`, `other`.|
|deviceStates|[conditionalAccessDeviceStates](conditionalaccessdevicestates.md)| Estados do dispositivo na política. |
|dispositivos|[conditionalAccessDevices](conditionalaccessdevices.md)| Dispositivos na política. |
|locations|[conditionalAccessLocations](conditionalaccesslocations.md)| Locais incluídos no e excluídos da política. |
|plataformas|[conditionalAccessPlatforms](conditionalaccessplatforms.md)| Plataformas incluídas e excluídas da política. |
|signInRiskLevels|Coleção de cadeias de caracteres| Níveis de risco incluídos na política. Os valores possíveis são: `low`, `medium`, `high`, `none`.|

>**Observação:** Estamos preterindo a condição **deviceStates** e ela poderá ser removida no futuro. Em frente, use a condição **dispositivos** .

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "clientAppTypes",
    "deviceStates",
    "devices",
    "locations",
    "platforms",
    "signInRiskLevels"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessConditionSet",
  "baseType": null
}-->

```json
{
  "applications": {"@odata.type": "microsoft.graph.conditionalAccessApplications"},
  "users": {"@odata.type": "microsoft.graph.conditionalAccessUsers"},
  "clientAppTypes": ["String"],
  "deviceStates": {"@odata.type": "microsoft.graph.conditionalAccessDeviceStates"},
  "devices": {"@odata.type": "microsoft.graph.conditionalAccessDevices"},
  "locations": {"@odata.type": "microsoft.graph.conditionalAccessLocations"},
  "platforms": {"@odata.type": "microsoft.graph.conditionalAccessPlatforms"},
  "signInRiskLevels": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessConditionset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
