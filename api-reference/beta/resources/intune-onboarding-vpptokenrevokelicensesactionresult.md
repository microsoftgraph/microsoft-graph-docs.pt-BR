---
title: Tipo de recurso vppTokenRevokeLicensesActionResult
description: O status da ação revogar licenças realizada no token do Programa de Compra de Volume da Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bd08741b48e81afa4a3775fdb3cd4ed160e0e6b9
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58790616"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a>Tipo de recurso vppTokenRevokeLicensesActionResult

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O status da ação revogar licenças realizada no token do Programa de Compra de Volume da Apple.


Herda de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|actionName|Cadeia de caracteres|Nome da ação Herdado [de vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|Estado da ação Herdada de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md). Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|startDateTime|DateTimeOffset|Hora em que a ação foi iniciada Herdada de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)|
|lastUpdatedDateTime|DateTimeOffset|Hora em que o estado da ação foi atualizado pela última vez Herdado de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)|
|totalLicensesCount|Int32|Uma contagem do número de licenças que foram tentadas revogar.|
|failedLicensesCount|Int32|Uma contagem do número de licenças que não foram revogadas.|
|actionFailureReason|[vppTokenActionFailureReason](../resources/intune-shared-vpptokenactionfailurereason.md)|O motivo da falha na ação revogar licenças. Os valores possíveis são: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.|

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



