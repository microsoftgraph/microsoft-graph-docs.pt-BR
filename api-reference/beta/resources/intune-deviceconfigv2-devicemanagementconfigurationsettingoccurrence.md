---
title: Tipo de recurso deviceManagementConfigurationSettingOccurrence
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d339ba6fce600c578ce4aa180a509ec685ca2216
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58816911"
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



