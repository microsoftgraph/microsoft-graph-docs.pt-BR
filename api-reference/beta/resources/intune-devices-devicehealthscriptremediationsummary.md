---
title: Tipo de recurso deviceHealthScriptRemediationSummary
description: O número de scripts de saúde do dispositivo implantados e o número de dispositivos que os scripts remediaram.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2eb1177b80f95572599e6205cfdd00499e65b0f3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59144311"
---
# <a name="devicehealthscriptremediationsummary-resource-type"></a>Tipo de recurso deviceHealthScriptRemediationSummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O número de scripts de saúde do dispositivo implantados e o número de dispositivos que os scripts remediaram.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|scriptCount|Int32|O número de scripts de saúde do dispositivo implantados.|
|remediatedDeviceCount|Int32|O número de dispositivos remediados por scripts de saúde do dispositivo.|

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



