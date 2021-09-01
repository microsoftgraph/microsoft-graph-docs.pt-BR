---
title: Tipo de recurso deviceHealthScriptRemediationHistoryData
description: O número de dispositivos remediados por um script de saúde do dispositivo em uma determinada data.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c6c456b3edc591c0394446bbb23b6975781da4d4
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58793807"
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



