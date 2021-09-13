---
title: tipo de recurso userExperienceAnalyticsAutopilotDevicesSummary
description: O resumo de análise de experiência do usuário de Dispositivos que não estão prontos para o windows autopilot.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3ec2b055c67a03f65acdd306f0f1f49b30f27663
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59040047"
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



