---
title: tipo de recurso importedDeviceIdentityResult
description: O recurso importedDeviceIdentityResult representa o resultado da tentativa de importar uma identidade de dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b1a5fbaac297a85595827f23cafd93035188bc4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156277"
---
# <a name="importeddeviceidentityresult-resource-type"></a>tipo de recurso importedDeviceIdentityResult

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso importedDeviceIdentityResult representa o resultado da tentativa de importar uma identidade de dispositivo.


Herda de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar importedDeviceIdentityResults](../api/intune-enrollment-importeddeviceidentityresult-list.md)|coleção [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|Listar Propriedades e relações dos objetos [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) .|
|[Obter importedDeviceIdentityResult](../api/intune-enrollment-importeddeviceidentityresult-get.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|Leia as propriedades e as relações do objeto [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) .|
|[Criar importedDeviceIdentityResult](../api/intune-enrollment-importeddeviceidentityresult-create.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|Criar um novo objeto [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) .|
|[Excluir importedDeviceIdentityResult](../api/intune-enrollment-importeddeviceidentityresult-delete.md)|Nenhum|Exclui [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).|
|[Atualizar importedDeviceIdentityResult](../api/intune-enrollment-importeddeviceidentityresult-update.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|Atualiza as propriedades de um objeto [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|ID da identidade de dispositivo importada herdada de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|importedDeviceIdentifier|String|Identificador de dispositivo imPortado herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|importedDeviceIdentityType|[importedDeviceIdentityType](../resources/intune-enrollment-importeddeviceidentitytype.md)|Tipo de identidade de dispositivo imPortado herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md). Os valores possíveis são: `unknown`, `imei`, `serialNumber`.|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação da descrição herdadas de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|createdDateTime|DateTimeOffset|Data e hora de criação do dispositivo herdadas de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|lastContactedDateTime|DateTimeOffset|Data e hora do último contato do dispositivo herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|description|Cadeia de caracteres|A descrição do dispositivo herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|enrollmentid|[enrollmentid](../resources/intune-enrollment-enrollmentstate.md)|O estado do dispositivo no Intune herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md). Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|platform|[plataforma](../resources/intune-enrollment-platform.md)|A plataforma do dispositivo. Herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md). Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|
|status|Boolean|Status da identidade do dispositivo importado|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedDeviceIdentityResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "id": "String (identifier)",
  "importedDeviceIdentifier": "String",
  "importedDeviceIdentityType": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String",
  "status": true
}
```




