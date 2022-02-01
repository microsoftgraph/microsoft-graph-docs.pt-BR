---
title: tipo de recurso userExperienceAnalyticsWorkFromAnywhereModelPerformance
description: A análise de experiência do usuário funciona a partir do desempenho do modelo em qualquer lugar.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0c6a21965c5f1f947b2f3d66dafcfb03cb777fc9
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2022
ms.locfileid: "62292257"
---
# <a name="userexperienceanalyticsworkfromanywheremodelperformance-resource-type"></a>tipo de recurso userExperienceAnalyticsWorkFromAnywhereModelPerformance

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A análise de experiência do usuário funciona a partir do desempenho do modelo em qualquer lugar.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsWorkFromAnywhereModelPerformances](../api/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance-list.md)|[coleção userExperienceAnalyticsWorkFromAnywhereModelPerformance](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsWorkFromAnywhereModelPerformance](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md) .|
|[Obter userExperienceAnalyticsWorkFromAnywhereModelPerformance](../api/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance-get.md)|[userExperienceAnalyticsWorkFromAnywhereModelPerformance](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md)|Ler propriedades e relações do [objeto userExperienceAnalyticsWorkFromAnywhereModelPerformance](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md) .|
|[Criar userExperienceAnalyticsWorkFromAnywhereModelPerformance](../api/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance-create.md)|[userExperienceAnalyticsWorkFromAnywhereModelPerformance](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md)|Crie um novo [objeto userExperienceAnalyticsWorkFromAnywhereModelPerformance](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md) .|
|[Excluir userExperienceAnalyticsWorkFromAnywhereModelPerformance](../api/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance-delete.md)|Nenhuma|Exclui um [userExperienceAnalyticsWorkFromAnywhereModelPerformance](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md).|
|[Atualizar userExperienceAnalyticsWorkFromAnywhereModelPerformance](../api/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance-update.md)|[userExperienceAnalyticsWorkFromAnywhereModelPerformance](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsWorkFromAnywhereModelPerformance](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do objeto de desempenho do modelo de análise de experiência do usuário.|
|modelo|String|A experiência do usuário funciona a partir do nome do modelo dos dispositivos em qualquer lugar.|
|fabricante|String|A experiência do usuário funciona a partir do nome do fabricante dos dispositivos em qualquer lugar.|
|modelDeviceCount|Int32|A experiência do usuário funciona a partir da contagem de dispositivos de qualquer lugar para o modelo. Valores válidos -2147483648 para 2147483647|
|workFromAnywhereScore|Duplo|A experiência do usuário funciona em qualquer lugar da pontuação geral do modelo. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|windowsScore|Duplo|A experiência do usuário funciona de qualquer lugar que o Windows pontua para o modelo. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|cloudManagementScore|Duplo|A experiência do usuário funciona a partir da pontuação de gerenciamento de nuvem em qualquer lugar para o modelo. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|cloudIdentityScore|Duplo|A experiência do usuário funciona a partir da pontuação de identidade na nuvem do modelo. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|cloudProvisioningScore|Duplo|A experiência do usuário funciona a partir da pontuação de provisionamento de nuvem de qualquer lugar para o modelo. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|O estado de saúde da análise de experiência do usuário funciona de qualquer modelo. Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsWorkFromAnywhereModelPerformance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereModelPerformance",
  "id": "String (identifier)",
  "model": "String",
  "manufacturer": "String",
  "modelDeviceCount": 1024,
  "workFromAnywhereScore": "4.2",
  "windowsScore": "4.2",
  "cloudManagementScore": "4.2",
  "cloudIdentityScore": "4.2",
  "cloudProvisioningScore": "4.2",
  "healthStatus": "String"
}
```




