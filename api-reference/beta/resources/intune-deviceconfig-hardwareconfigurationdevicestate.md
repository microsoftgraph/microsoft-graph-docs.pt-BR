---
title: Tipo de recurso hardwareConfigurationDeviceState
description: Contém propriedades para o estado de execução do dispositivo da configuração de hardware
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 70a5fdd114afd1ad4de4e6317282146f481e0288
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63368270"
---
# <a name="hardwareconfigurationdevicestate-resource-type"></a>Tipo de recurso hardwareConfigurationDeviceState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para o estado de execução do dispositivo da configuração de hardware

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar hardwareConfigurationDeviceStates](../api/intune-deviceconfig-hardwareconfigurationdevicestate-list.md)|[Coleção hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)|Listar propriedades e relações dos [objetos hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md) .|
|[Obter hardwareConfigurationDeviceState](../api/intune-deviceconfig-hardwareconfigurationdevicestate-get.md)|[hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)|Ler propriedades e relações do [objeto hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md) .|
|[Criar hardwareConfigurationDeviceState](../api/intune-deviceconfig-hardwareconfigurationdevicestate-create.md)|[hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)|Crie um novo [objeto hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md) .|
|[Excluir hardwareConfigurationDeviceState](../api/intune-deviceconfig-hardwareconfigurationdevicestate-delete.md)|Nenhum|Exclui [um hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md).|
|[Atualizar hardwareConfigurationDeviceState](../api/intune-deviceconfig-hardwareconfigurationdevicestate-update.md)|[hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md)|Atualize as propriedades de [um objeto hardwareConfigurationDeviceState](../resources/intune-deviceconfig-hardwareconfigurationdevicestate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade de estado do dispositivo de script de configuração de hardware. Essa propriedade é somente leitura.|
|deviceName|String|O nome do dispositivo|
|osVersion|String|Versão do sistema operacional do dispositivo (por exemplo, 10.0.19042.1165, 10.0.19042.1288 etc.)|
|upn|Cadeia de caracteres|Nome principal do usuário (UPN).|
|internalVersion|Int32|A versão interna da Política|
|lastStateUpdateDateTime|DateTimeOffset|O último período de data/hora de quando a configuração de hardware foi executada|
|configurationState|[runState](../resources/intune-deviceconfig-runstate.md)|Estado de configuração da última execução de configuração de hardware. Os possíveis valores são: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|configurationOutput|String|Saída da execução da configuração de hardware|
|configurationError|String|Erro da execução da configuração de hardware|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.hardwareConfigurationDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwareConfigurationDeviceState",
  "id": "String (identifier)",
  "deviceName": "String",
  "osVersion": "String",
  "upn": "String",
  "internalVersion": 1024,
  "lastStateUpdateDateTime": "String (timestamp)",
  "configurationState": "String",
  "configurationOutput": "String",
  "configurationError": "String"
}
```




