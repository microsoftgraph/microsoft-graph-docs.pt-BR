---
title: tipo de recurso de revokeAppleVppLicensesActionResult
description: Revogar o resultado de ação do Apple Vpp licenças
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2cd77bee330e919ab51927af0773d913099cea6e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419223"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a>tipo de recurso de revokeAppleVppLicensesActionResult

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Revogar o resultado de ação do Apple Vpp licenças


Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|actionName|Cadeia de caracteres|Nome da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|Estado da ação Inherited de [deviceActionResult](../resources/intune-devices-deviceactionresult.md). Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|startDateTime|DateTimeOffset|Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|
|lastUpdatedDateTime|DateTimeOffset|Hora em que o estado da ação foi atualizado pela última vez, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|
|totalLicensesCount|Int32|Número total de licenças do Apple Vpp associados|
|failedLicensesCount|Int32|Número total de licenças Apple Vpp com falha para revogar|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.revokeAppleVppLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.revokeAppleVppLicensesActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024
}
```




