---
title: Tipo de recurso deviceComplianceDeviceOverview
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 607b85e9cbfbc5ee8d9be792a7f6f29bf6f6ace1
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58819203"
---
# <a name="devicecompliancedeviceoverview-resource-type"></a>Tipo de recurso deviceComplianceDeviceOverview

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceComplianceDeviceOverview](../api/intune-deviceconfig-devicecompliancedeviceoverview-get.md)|[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|Ler propriedades e relações de objetos de [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).|
|[Atualizar deviceComplianceDeviceOverview](../api/intune-deviceconfig-devicecompliancedeviceoverview-update.md)|[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|Atualizar as propriedades de um objeto de [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|pendingCount|Int32|Número de dispositivos pendentes|
|notApplicableCount|Int32|Número de dispositivos não aplicáveis|
|notApplicablePlatformCount|Int32|Número de dispositivos não aplicáveis devido à plataforma e à política de incompatibilidade|
|successCount|Int32|Número de dispositivos com êxito|
|errorCount|Int32|Número de dispositivos com erro|
|failedCount|Int32|Número de dispositivos com falha|
|conflictCount|Int32|Número de dispositivos em conflito|
|lastUpdateDateTime|DateTimeOffset|Hora da última atualização|
|configurationVersion|Int32|Versão da política para essa visão geral|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "notApplicablePlatformCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "conflictCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```



