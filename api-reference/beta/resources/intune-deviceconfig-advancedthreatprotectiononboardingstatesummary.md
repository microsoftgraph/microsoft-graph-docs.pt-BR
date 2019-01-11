---
title: tipo de recurso de advancedThreatProtectionOnboardingStateSummary
description: Windows defender ameaça avançada proteção inclusão resumo estado entre a conta.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b700658c6ae7b486ae52f4ea226b7a6bab7f0af6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838217"
---
# <a name="advancedthreatprotectiononboardingstatesummary-resource-type"></a>tipo de recurso de advancedThreatProtectionOnboardingStateSummary

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Windows defender ameaça avançada proteção inclusão resumo estado entre a conta.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter advancedThreatProtectionOnboardingStateSummary](../api/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary-get.md)|[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|Leia as propriedades e os relacionamentos do objeto [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) .|
|[Atualizar advancedThreatProtectionOnboardingStateSummary](../api/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary-update.md)|[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)|Atualize as propriedades de um objeto [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo|
|unknownDeviceCount|Int32|Número de dispositivos desconhecidos|
|notApplicableDeviceCount|Int32|Número de dispositivos não aplicáveis|
|compliantDeviceCount|Int32|Número de dispositivos em conformidade|
|remediatedDeviceCount|Int32|Número de dispositivos corrigidos|
|nonCompliantDeviceCount|Int32|Número de dispositivos sem conformidade|
|errorDeviceCount|Int32|Número de dispositivos com erro|
|conflictDeviceCount|Int32|Número de dispositivos em conflito|
|notAssignedDeviceCount|Int32|Número de dispositivos não atribuídos|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|advancedThreatProtectionOnboardingDeviceSettingStates|coleção [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)|Ainda não documentado|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.advancedThreatProtectionOnboardingStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingStateSummary",
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024,
  "notAssignedDeviceCount": 1024
}
```





