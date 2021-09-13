---
title: tipo de recurso userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric
description: A entidade de preparação de hardware de análise de experiência do usuário contém informações de nível de conta sobre bloqueadores de hardware para atualização do Windows.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a9716cee7e1ba03253b040c52d49e0df404b9c48
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59046866"
---
# <a name="userexperienceanalyticsworkfromanywherehardwarereadinessmetric-resource-type"></a>tipo de recurso userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de preparação de hardware de análise de experiência do usuário contém informações de nível de conta sobre bloqueadores de hardware para atualização do Windows.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric](../api/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric-get.md)|[userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric.md)|Leia propriedades e relações do [objeto userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric.](../resources/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric.md)|
|[Atualizar userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric](../api/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric-update.md)|[userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric.](../resources/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do objeto métrico de preparação de hardware de análise de experiência do usuário.|
|totalDeviceCount|Int32|A contagem do total de dispositivos em uma organização. Valores válidos -2147483648 para 2147483647|
|upgradeEligibleDeviceCount|Int32|A contagem de dispositivos em uma organização qualificada para atualização do Windows. Valores válidos -2147483648 para 2147483647|
|ramCheckFailedPercentage|Duplo|A porcentagem de dispositivos para os quais a verificação de hardware ram falhou. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|storageCheckFailedPercentage|Duplo|A porcentagem de dispositivos para os quais a verificação de hardware de armazenamento falhou. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|processorCoreCountCheckFailedPercentage|Duplo|A porcentagem de dispositivos para os quais a contagem de núcleos de hardware do processador falhou. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|processorSpeedCheckFailedPercentage|Duplo|A porcentagem de dispositivos para os quais a verificação de velocidade de hardware do processador falhou. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|tpmCheckFailedPercentage|Duplo|A porcentagem de dispositivos para os quais a verificação de hardware TPM (Trusted Platform Module) falhou. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|secureBootCheckFailedPercentage|Duplo|A porcentagem de dispositivos para os quais a verificação de hardware de inicialização segura falhou. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|processorFamilyCheckFailedPercentage|Duplo|A porcentagem de dispositivos para os quais a família de hardware do processador falhou. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|processor64BitCheckFailedPercentage|Duplo|A porcentagem de dispositivos para os quais a verificação da arquitetura de hardware de 64 bits do processador falhou. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|osCheckFailedPercentage|Duplo|A porcentagem de dispositivos para os quais a verificação do sistema operacional falhou. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric",
  "id": "String (identifier)",
  "totalDeviceCount": 1024,
  "upgradeEligibleDeviceCount": 1024,
  "ramCheckFailedPercentage": "4.2",
  "storageCheckFailedPercentage": "4.2",
  "processorCoreCountCheckFailedPercentage": "4.2",
  "processorSpeedCheckFailedPercentage": "4.2",
  "tpmCheckFailedPercentage": "4.2",
  "secureBootCheckFailedPercentage": "4.2",
  "processorFamilyCheckFailedPercentage": "4.2",
  "processor64BitCheckFailedPercentage": "4.2",
  "osCheckFailedPercentage": "4.2"
}
```



