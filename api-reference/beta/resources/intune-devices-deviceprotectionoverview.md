---
title: Tipo de recurso deviceProtectionOverview
description: Informações de hardware de um determinado dispositivo.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 310d7e8623dad1baac2d77b6b8e23e527e4e4709
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59125859"
---
# <a name="deviceprotectionoverview-resource-type"></a>Tipo de recurso deviceProtectionOverview

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Informações de hardware de um determinado dispositivo.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|totalReportedDeviceCount|Int32|Contagem total de dispositivos.|
|inactiveThreatAgentDeviceCount|Int32|Dispositivo com contagem de agentes de ameaças inativos|
|unknownStateThreatAgentDeviceCount|Int32|Dispositivo com estado de agente de ameaça como contagem desconhecida.|
|pendingSignatureUpdateDeviceCount|Int32|Dispositivo com contagem de assinatura antiga.|
|cleanDeviceCount|Int32|Contagem de dispositivos limpos.|
|pendingFullScanDeviceCount|Int32|Pendente contagem de dispositivos de verificação completa.|
|pendingRestartDeviceCount|Int32|Contagem pendente do dispositivo de reinicialização.|
|pendingManualStepsDeviceCount|Int32|Contagem de dispositivos de etapas manuais pendentes.|
|pendingOfflineScanDeviceCount|Int32|Contagem pendente do dispositivo de verificação offline.|
|criticalFailuresDeviceCount|Int32|Contagem de dispositivos de falhas críticas.|
|pendingQuickScanDeviceCount|Int32|Contagem pendente do dispositivo de verificação rápida. Valores válidos -2147483648 para 2147483647|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceProtectionOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceProtectionOverview",
  "totalReportedDeviceCount": 1024,
  "inactiveThreatAgentDeviceCount": 1024,
  "unknownStateThreatAgentDeviceCount": 1024,
  "pendingSignatureUpdateDeviceCount": 1024,
  "cleanDeviceCount": 1024,
  "pendingFullScanDeviceCount": 1024,
  "pendingRestartDeviceCount": 1024,
  "pendingManualStepsDeviceCount": 1024,
  "pendingOfflineScanDeviceCount": 1024,
  "criticalFailuresDeviceCount": 1024,
  "pendingQuickScanDeviceCount": 1024
}
```



