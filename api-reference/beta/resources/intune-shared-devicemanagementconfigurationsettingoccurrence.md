---
title: Tipo de recurso deviceManagementConfigurationSettingOccurrence
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9b8a93c75f011dba9816ee84a9ef8bf5cd05d275
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671429"
---
# <a name="devicemanagementconfigurationsettingoccurrence-resource-type"></a>Tipo de recurso deviceManagementConfigurationSettingOccurrence

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|minDeviceOccurrence|Int32|A configuração de horários mínimos pode ser definida no dispositivo. Uma MinDeviceOccurrence de 0 significa que a configuração é opcional|
|maxDeviceOccurrence|Int32|A configuração de horas máximas pode ser definida no dispositivo. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingOccurrence"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingOccurrence",
  "minDeviceOccurrence": 1024,
  "maxDeviceOccurrence": 1024
}
```




