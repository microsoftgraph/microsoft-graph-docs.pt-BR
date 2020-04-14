---
title: tipo de recurso deviceHealthScriptRemediationSummary
description: O número de scripts de integridade do dispositivo implantados e o número de dispositivos nos quais os scripts foram corrigidos.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5ca477131c3051161b17ed3f3e90aaf172662dfc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43388444"
---
# <a name="devicehealthscriptremediationsummary-resource-type"></a>tipo de recurso deviceHealthScriptRemediationSummary

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O número de scripts de integridade do dispositivo implantados e o número de dispositivos nos quais os scripts foram corrigidos.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|scriptCount|Int32|O número de scripts de integridade do dispositivo implantados.|
|remediatedDeviceCount|Int32|O número de dispositivos corrigidos por scripts de integridade de dispositivo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRemediationSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRemediationSummary",
  "scriptCount": 1024,
  "remediatedDeviceCount": 1024
}
```



