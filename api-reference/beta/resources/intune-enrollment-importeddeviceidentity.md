---
title: tipo de recurso de importedDeviceIdentity
description: O recurso de importedDeviceIdentity representa uma identidade exclusiva de hardware de um dispositivo que tenha sido esses transferidos para configuração de inscrição prévia.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3c33069520913c7c750220ca8938459ba9bf96c2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811666"
---
# <a name="importeddeviceidentity-resource-type"></a>tipo de recurso de importedDeviceIdentity

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

O recurso de importedDeviceIdentity representa uma identidade exclusiva de hardware de um dispositivo que tenha sido esses transferidos para configuração de inscrição prévia.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista importedDeviceIdentities](../api/intune-enrollment-importeddeviceidentity-list.md)|coleção [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Lista as propriedades e os relacionamentos dos objetos [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .|
|[Obter importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-get.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Leia as propriedades e os relacionamentos do objeto [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .|
|[Criar importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-create.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Crie um novo objeto de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .|
|[Excluir importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-delete.md)|Nenhum|Exclui um [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).|
|[Atualizar importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-update.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Atualize as propriedades de um objeto [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .|
|[ação de importDeviceIdentityList](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|coleção [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID da identidade do dispositivo importada|
|importedDeviceIdentifier|Cadeia de caracteres|Identificador de dispositivo importada|
|importedDeviceIdentityType|[importedDeviceIdentityType](../resources/intune-enrollment-importeddeviceidentitytype.md)|Tipo de identidade do dispositivo importada. Os valores possíveis são: `unknown`, `imei`, `serialNumber`.|
|lastModifiedDateTime|DateTimeOffset|Última data e hora modificadas da descrição|
|createdDateTime|DateTimeOffset|Criada data hora do dispositivo|
|lastContactedDateTime|DateTimeOffset|Última contatado data hora do dispositivo|
|description|Cadeia de caracteres|A descrição do dispositivo|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|O estado do dispositivo em Intune. Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|platform|[plataforma](../resources/intune-enrollment-platform.md)|A plataforma do dispositivo. Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "id": "String (identifier)",
  "importedDeviceIdentifier": "String",
  "importedDeviceIdentityType": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String"
}
```





