---
title: Tipo de recurso deviceScopeActionResult
description: O resultado da ação de escopo do dispositivo disparada.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c3f991b685f2982a4b913325f409cff34ba8a985
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66670320"
---
# <a name="devicescopeactionresult-resource-type"></a>Tipo de recurso deviceScopeActionResult

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O resultado da ação de escopo do dispositivo disparada.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|deviceScopeAction|[deviceScopeAction](../resources/intune-devices-devicescopeaction.md)|O nome da ação disparada. Os valores possíveis são: .|
|deviceScopeId|Cadeia de Caracteres|O identificador exclusivo do escopo do dispositivo no qual a ação foi disparada.|
|status|[deviceScopeActionStatus](../resources/intune-devices-devicescopeactionstatus.md)|Indica o status da ação de escopo do dispositivo de tentativa. Quando bem-sucedida, a ação foi disparada com êxito. Quando falhou, a ação falhou ao disparar. Os valores possíveis são: `failed`, `succeeded`, `unknownFutureValue`.|
|failedMessage|Cadeia de Caracteres|A mensagem indica o motivo pelo qual a ação de escopo do dispositivo falhou ao disparar.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceScopeActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceScopeActionResult",
  "deviceScopeAction": "String",
  "deviceScopeId": "String",
  "status": "String",
  "failedMessage": "String"
}
```




