---
title: tipo de recurso deviceHealthScriptRemediationSummary
description: O número de scripts de integridade do dispositivo implantados e o número de dispositivos nos quais os scripts foram corrigidos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 06e48973305dbbdf7ae276e4d14d3307da74c36e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060284"
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






