---
title: Tipo de recurso customUpdateTimeWindow
description: Janela de tempo de atualização personalizada
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4653237f56ef0f00d7c22e2e2c09bfb694cd8cca
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59146699"
---
# <a name="customupdatetimewindow-resource-type"></a>Tipo de recurso customUpdateTimeWindow

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Janela de tempo de atualização personalizada

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|startDay|[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)|Dia de início da janela de tempo. Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|endDay|[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)|Fim do dia da janela de tempo. Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|startTime|TimeOfDay|Hora de início da janela de tempo|
|endTime|TimeOfDay|Hora de término da janela de tempo|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customUpdateTimeWindow"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customUpdateTimeWindow",
  "startDay": "String",
  "endDay": "String",
  "startTime": "String (time of day)",
  "endTime": "String (time of day)"
}
```



