---
title: Tipo de recurso hardwareConfigurationRunSummary
description: Contém propriedades para o resumo de execução de um script de configuração de hardware.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6debf44d50ff1f501af172de706165c22dd02642
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61345347"
---
# <a name="hardwareconfigurationrunsummary-resource-type"></a>Tipo de recurso hardwareConfigurationRunSummary

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para o resumo de execução de um script de configuração de hardware.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter hardwareConfigurationRunSummary](../api/intune-deviceconfig-hardwareconfigurationrunsummary-get.md)|[hardwareConfigurationRunSummary](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md)|Leia propriedades e relações do [objeto hardwareConfigurationRunSummary.](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md)|
|[Atualizar hardwareConfigurationRunSummary](../api/intune-deviceconfig-hardwareconfigurationrunsummary-update.md)|[hardwareConfigurationRunSummary](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md)|Atualize as propriedades de [um objeto hardwareConfigurationRunSummary.](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade resumo de execução de configuração de hardware. Essa propriedade é somente leitura.|
|successfulDeviceCount|Int32|Número de dispositivos para os quais o hardware foi configurado sem qualquer problema|
|failedDeviceCount|Int32|Número de dispositivos para os quais a configuração de hardware encontrou um problema|
|pendingDeviceCount|Int32|Número de dispositivos para os quais a configuração de hardware está em estado pendente|
|errorDeviceCount|Int32|Número de dispositivos para os quais o estado de configuração de hardware é erro|
|notApplicableDeviceCount|Int32|Número de dispositivos para os quais o estado de configuração de hardware não é aplicável|
|unknownDeviceCount|Int32|Número de dispositivos para os quais o estado de configuração de hardware é desconhecido|
|successfulUserCount|Int32|Número de usuários para os quais o hardware foi configurado sem qualquer problema|
|failedUserCount|Int32|Número de usuários para os quais a configuração de hardware encontrou um problema|
|pendingUserCount|Int32|Número de usuários para os quais a configuração de hardware está em estado pendente|
|errorUserCount|Int32|Número de usuários para os quais o estado de configuração de hardware é erro|
|notApplicableUserCount|Int32|Número de usuários para os quais o estado de configuração de hardware não é aplicável|
|unknownUserCount|Int32|Número de usuários para os quais o estado de configuração de hardware é desconhecido|
|lastRunDateTime|DateTimeOffset|Último tempo de execução para a configuração em todos os dispositivos|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.hardwareConfigurationRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwareConfigurationRunSummary",
  "id": "String (identifier)",
  "successfulDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "pendingDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "successfulUserCount": 1024,
  "failedUserCount": 1024,
  "pendingUserCount": 1024,
  "errorUserCount": 1024,
  "notApplicableUserCount": 1024,
  "unknownUserCount": 1024,
  "lastRunDateTime": "String (timestamp)"
}
```




