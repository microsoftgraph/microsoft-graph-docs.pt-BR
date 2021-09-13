---
title: Tipo de recurso deviceHealthScriptRemediationHistoryData
description: O número de dispositivos remediados por um script de saúde do dispositivo em uma determinada data.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a7578a8455b3c74f843c090522ad5d3e491cd1b1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59144326"
---
# <a name="devicehealthscriptremediationhistorydata-resource-type"></a>Tipo de recurso deviceHealthScriptRemediationHistoryData

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O número de dispositivos remediados por um script de saúde do dispositivo em uma determinada data.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|data|Data|A data em que os dispositivos foram remediados pelo script de saúde do dispositivo.|
|remediatedDeviceCount|Int32|O número de dispositivos remediados pelo script de saúde do dispositivo.|
|noIssueDeviceCount|Int32|O número de dispositivos que foram encontrados sem problemas pelo script de saúde do dispositivo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRemediationHistoryData"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRemediationHistoryData",
  "date": "String (Date)",
  "remediatedDeviceCount": 1024,
  "noIssueDeviceCount": 1024
}
```



