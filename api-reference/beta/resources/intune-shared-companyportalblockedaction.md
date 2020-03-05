---
title: tipo de recurso companyPortalBlockedAction
description: Ações bloqueadas no portal da empresa de acordo com os tipos de propriedade de plataforma e dispositivo
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 15460de0c53b1b7b383095b7bee50af0192b3462
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527481"
---
# <a name="companyportalblockedaction-resource-type"></a>tipo de recurso companyPortalBlockedAction

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ações bloqueadas no portal da empresa de acordo com os tipos de propriedade de plataforma e dispositivo

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|platform|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)|Sistema operacional/plataforma do dispositivo. Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|ownerType|[ownerType](../resources/intune-shared-ownertype.md)|Tipo de propriedade de dispositivo. Os valores possíveis são: `unknown`, `company`, `personal`.|
|ação|[companyPortalAction](../resources/intune-shared-companyportalaction.md)|Ação de dispositivo. Os valores possíveis são: `unknown`, `remove`, `reset`.|

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



