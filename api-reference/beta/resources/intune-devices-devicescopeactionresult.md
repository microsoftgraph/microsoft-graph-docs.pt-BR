---
title: Tipo de recurso deviceScopeActionResult
description: O resultado da ação de escopo do dispositivo disparada.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6938869b658edb1d0fddc4dfa753e45cb1fb8eb5
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858485"
---
# <a name="devicescopeactionresult-resource-type"></a>Tipo de recurso deviceScopeActionResult

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O resultado da ação de escopo do dispositivo disparada.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|deviceScopeAction|[deviceScopeAction](../resources/intune-devices-devicescopeaction.md)|O nome da ação disparada. Os valores possíveis são: .|
|deviceScopeId|String|O identificador exclusivo do escopo do dispositivo no qual a ação foi disparada.|
|status|[deviceScopeActionStatus](../resources/intune-devices-devicescopeactionstatus.md)|Indica o status da ação de escopo do dispositivo de tentativa. Quando bem-sucedida, a ação foi disparada com êxito. Quando falhou, a ação falhou ao disparar. Os valores possíveis são: `failed`, `succeeded`, `unknownFutureValue`.|
|failedMessage|String|A mensagem indica o motivo pelo qual a ação de escopo do dispositivo falhou ao disparar.|

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
  "@odata.type": "microsoft.graph.deviceScopeActionResult",
  "deviceScopeAction": "String",
  "deviceScopeId": "String",
  "status": "String",
  "failedMessage": "String"
}
```




