---
title: Tipo de recurso deviceHealthScriptRemediationHistoryData
description: O número de dispositivos remediados por um script de saúde do dispositivo em uma determinada data.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2f88d54cf9e2643c9dab4ef4c1c60e7b0fe7569f242612264dae201aa094375b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54206386"
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




