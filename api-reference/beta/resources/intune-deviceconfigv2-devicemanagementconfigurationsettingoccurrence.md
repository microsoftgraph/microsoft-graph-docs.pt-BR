---
title: Tipo de recurso deviceManagementConfigurationSettingOccurrence
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 21ff7940e6e657d965b27823f0480b8247bae013767b51eaabb737a6d21ed844
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54244831"
---
# <a name="devicemanagementconfigurationsettingoccurrence-resource-type"></a>Tipo de recurso deviceManagementConfigurationSettingOccurrence

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|minDeviceOccurrence|Int32|A configuração de horários mínimos pode ser definida no dispositivo. Uma minDeviceOccurrence de 0 significa que a configuração é opcional|
|maxDeviceOccurrence|Int32|A configuração de horários máximos pode ser definida no dispositivo. |

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




