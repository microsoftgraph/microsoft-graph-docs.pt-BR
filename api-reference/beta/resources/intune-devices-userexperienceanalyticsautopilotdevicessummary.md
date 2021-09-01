---
title: tipo de recurso userExperienceAnalyticsAutopilotDevicesSummary
description: O resumo de análise de experiência do usuário de Dispositivos que não estão prontos para o windows autopilot.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 95d93e809d72df3e2e224c77d6691f5c801e376f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58806107"
---
# <a name="userexperienceanalyticsautopilotdevicessummary-resource-type"></a>tipo de recurso userExperienceAnalyticsAutopilotDevicesSummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O resumo de análise de experiência do usuário de Dispositivos que não estão prontos para o windows autopilot.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|devicesNotAutopilotRegistered|Int32|A contagem de dispositivos do intune que não estão no piloto automático registrado.|
|devicesWithoutAutopilotProfileAssigned|Int32|A contagem de dispositivos do intune não atribuídos ao perfil de piloto automático.|
|totalWindows10DevicesWithoutTenantAttached|Int32|A contagem de dispositivos windows 10 que são Intune e Comanaged.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsAutopilotDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAutopilotDevicesSummary",
  "devicesNotAutopilotRegistered": 1024,
  "devicesWithoutAutopilotProfileAssigned": 1024,
  "totalWindows10DevicesWithoutTenantAttached": 1024
}
```



