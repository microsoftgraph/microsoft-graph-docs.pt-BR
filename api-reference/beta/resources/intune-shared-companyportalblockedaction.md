---
title: Tipo de recurso companyPortalBlockedAction
description: Ações bloqueadas no portal da empresa de acordo com tipos de propriedade de plataforma e dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0e608fee9178e3e7dedfecd99df19707901cdc3d
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266811"
---
# <a name="companyportalblockedaction-resource-type"></a>Tipo de recurso companyPortalBlockedAction

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ações bloqueadas no portal da empresa de acordo com tipos de propriedade de plataforma e dispositivo

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|plataforma|[devicePlatformType](../resources/intune-wip-deviceplatformtype.md)|Sistema operacional/plataforma do dispositivo. Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|ownerType|[ownerType](../resources/intune-shared-ownertype.md)|Tipo de propriedade do dispositivo. Os valores possíveis são: `unknown`, `company`, `personal`.|
|ação|[companyPortalAction](../resources/intune-shared-companyportalaction.md)|Ação do dispositivo. Os valores possíveis são: `unknown`, `remove`, `reset`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.companyPortalBlockedAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.companyPortalBlockedAction",
  "platform": "String",
  "ownerType": "String",
  "action": "String"
}
```




