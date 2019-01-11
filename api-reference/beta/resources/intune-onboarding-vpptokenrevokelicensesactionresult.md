---
title: tipo de recurso de vppTokenRevokeLicensesActionResult
description: O status da ação licenças revoke executada no token do programa de compra de Volume do Apple.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d7df9472be177bb52eba22ebf54f24e75c9a3539
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866490"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a>tipo de recurso de vppTokenRevokeLicensesActionResult

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

O status da ação licenças revoke executada no token do programa de compra de Volume do Apple.

Herda de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|actionName|Cadeia de caracteres|Nome da ação Inherited de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|Estado da ação Inherited de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md). Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|startDateTime|DateTimeOffset|Hora a ação foi iniciada herdado de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)|
|lastUpdatedDateTime|DateTimeOffset|Tempo que o estado de ação foi o último atualizado Inherited de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)|
|totalLicensesCount|Int32|Uma contagem do número de licenças que foram tentados a serem revogados.|
|failedLicensesCount|Int32|Uma contagem do número de licenças que falharam a serem revogados.|
|actionFailureReason|[vppTokenActionFailureReason](../resources/intune-shared-vpptokenactionfailurereason.md)|O motivo da falha de ação de licenças revoke. Os valores possíveis são: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenRevokeLicensesActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024,
  "actionFailureReason": "String"
}
```





