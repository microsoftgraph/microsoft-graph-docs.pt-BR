---
title: Tipo de recurso deviceHealthScriptRemediationSummary
description: O número de scripts de saúde do dispositivo implantados e o número de dispositivos que os scripts remediaram.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ac9e06cdbc8aa5ba754528459e52142b7e4f3679
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58820685"
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



