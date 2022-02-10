---
title: Tipo de recurso conditionalAccessConditionSet
description: Representa o tipo de condições que regem quando a política se aplica.
ms.localizationpriority: medium
author: davidspooner
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3dbd7a5a1a436709deed0bf342718ea81a282798
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519443"
---
# <a name="conditionalaccessconditionset-resource-type"></a>Tipo de recurso conditionalAccessConditionSet

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o tipo de condições que regem quando a política se aplica.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|applications|[conditionalAccessApplications](conditionalaccessapplications.md)| Aplicativos e ações do usuário incluídas e excluídas da política. Obrigatório. |
|usuários|[conditionalAccessUsers](conditionalaccessusers.md)| Usuários, grupos e funções incluídos e excluídos da política. Os **usuários** ou **clientApplications** são necessários. |
|clientApplications|[conditionalAccessClientApplications](../resources/conditionalaccessclientapplications.md)|Aplicativos cliente (entidades de serviço e identidades de carga de trabalho) incluídos e excluídos da política. Os **usuários** ou **clientApplications** são necessários. |
|clientAppTypes|coleção conditionalAccessClientApp| Tipos de aplicativo cliente incluídos na política. Os possíveis valores são: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`. Obrigatório.|
|deviceStates|[conditionalAccessDeviceStates](conditionalaccessdevicestates.md)| Estados do dispositivo na política. |
|dispositivos|[conditionalAccessDevices](conditionalaccessdevices.md)| Dispositivos na política. |
|locations|[conditionalAccessLocations](conditionalaccesslocations.md)| Locais incluídos e excluídos da política. |
|plataformas|[conditionalAccessPlatforms](conditionalaccessplatforms.md)| Plataformas incluídas e excluídas da política. |
|servicePrincipalRiskLevels|Coleção riskLevel| Níveis de risco da entidade de serviço incluídos na política. Os valores possíveis são: `low`, `medium`, `high`, `none`, `unknownFutureValue`.|
|signInRiskLevels|Coleção riskLevel| Níveis de risco de login incluídos na política. Os possíveis valores são: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`. Obrigatório.|
|userRiskLevels|Coleção riskLevel| Níveis de risco de usuário incluídos na política. Os possíveis valores são: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`. Obrigatório.|

>**Observação:**
>* **clientAppType** `modern` será preterido e substituído por `mobileAppsAndDesktopClients`. <br>
>* **clientAppType** `easUnsupported` será preterido `exchangeActiveSync` em favor do que inclui plataformas com suporte e sem suporte do EAS. <br>
>* Estamos preterindo a condição **deviceStates** e ela pode ser removida no futuro. Em frente, use a **condição de** dispositivos.

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
  "@odata.type": "#microsoft.graph.conditionalAccessConditionSet",
  "applications": {"@odata.type": "microsoft.graph.conditionalAccessApplications"},
  "users": {"@odata.type": "microsoft.graph.conditionalAccessUsers"},
  "clientApplications": {"@odata.type": "microsoft.graph.conditionalAccessClientApplications"},
  "clientAppTypes": ["String"],
  "deviceStates": {"@odata.type": "microsoft.graph.conditionalAccessDeviceStates"},
  "devices": {"@odata.type": "microsoft.graph.conditionalAccessDevices"},
  "locations": {"@odata.type": "microsoft.graph.conditionalAccessLocations"},
  "platforms": {"@odata.type": "microsoft.graph.conditionalAccessPlatforms"},
  "servicePrincipalRiskLevels": ["String"],
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


