---
title: Tipo de recurso importedDeviceIdentityResult
description: O recurso importedDeviceIdentityResult representa o resultado da tentativa de importar uma identidade de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cfa16effcc05b979a6d7c4110ed0b3fd65d8da2ac33d51d4442f1d1727b155fb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54122387"
---
# <a name="importeddeviceidentityresult-resource-type"></a>Tipo de recurso importedDeviceIdentityResult

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso importedDeviceIdentityResult representa o resultado da tentativa de importar uma identidade de dispositivo.


Herda de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar importedDeviceIdentityResults](../api/intune-enrollment-importeddeviceidentityresult-list.md)|[Coleção importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|Listar propriedades e relações dos [objetos importedDeviceIdentityResult.](../resources/intune-enrollment-importeddeviceidentityresult.md)|
|[Obter importedDeviceIdentityResult](../api/intune-enrollment-importeddeviceidentityresult-get.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|Leia propriedades e relações do [objeto importedDeviceIdentityResult.](../resources/intune-enrollment-importeddeviceidentityresult.md)|
|[Criar importedDeviceIdentityResult](../api/intune-enrollment-importeddeviceidentityresult-create.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|Crie um novo [objeto importedDeviceIdentityResult.](../resources/intune-enrollment-importeddeviceidentityresult.md)|
|[Excluir importedDeviceIdentityResult](../api/intune-enrollment-importeddeviceidentityresult-delete.md)|Nenhum|Exclui um [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).|
|[Atualizar importedDeviceIdentityResult](../api/intune-enrollment-importeddeviceidentityresult-update.md)|[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|Atualize as propriedades de [um objeto importedDeviceIdentityResult.](../resources/intune-enrollment-importeddeviceidentityresult.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID da identidade do dispositivo importado Herdada de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|importedDeviceIdentifier|Cadeia de caracteres|Identificador de Dispositivo Importado Herdado [de importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|importedDeviceIdentityType|[importedDeviceIdentityType](../resources/intune-enrollment-importeddeviceidentitytype.md)|Tipo de Identidade de Dispositivo Importado Herdada [de importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md). Os valores possíveis são: `unknown`, `imei`, `serialNumber`.|
|lastModifiedDateTime|DateTimeOffset|Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|createdDateTime|DateTimeOffset|Data de criação Hora do dispositivo Herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|lastContactedDateTime|DateTimeOffset|Hora da Última Data Contada do dispositivo Herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|description|Cadeia de caracteres|A descrição do dispositivo Herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|enrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|O estado do dispositivo no Intune Herdado de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md). Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|plataforma|[platform](../resources/intune-enrollment-platform.md)|A plataforma do Dispositivo. Herdado [de importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md). Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|
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




