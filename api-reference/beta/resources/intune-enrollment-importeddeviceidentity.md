---
title: tipo de recurso importedDeviceIdentity
description: O recurso importedDeviceIdentity representa uma identidade de hardware exclusiva de um dispositivo que foi pré-configurado para configuração de pré-registro.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 197f4d9fd3377e6359d93a75ac36c8c15be3e0f5
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941524"
---
# <a name="importeddeviceidentity-resource-type"></a>tipo de recurso importedDeviceIdentity

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso importedDeviceIdentity representa uma identidade de hardware exclusiva de um dispositivo que foi pré-configurado para configuração de pré-registro.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar importedDeviceIdentities](../api/intune-enrollment-importeddeviceidentity-list.md)|coleção [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Listar Propriedades e relações dos objetos [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .|
|[Obter importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-get.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Leia as propriedades e as relações do objeto [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .|
|[Criar importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-create.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Criar um novo objeto [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .|
|[Excluir importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-delete.md)|Nenhum|Exclui [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).|
|[Atualizar importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-update.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Atualiza as propriedades de um objeto [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .|
|[Ação importDeviceIdentityList](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|coleção [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|Ainda não documentado|
|[Ação searchExistingIdentities](../api/intune-enrollment-importeddeviceidentity-searchexistingidentities.md)|coleção [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID da identidade do dispositivo importado|
|importedDeviceIdentifier|Cadeia de caracteres|Identificador de dispositivo importado|
|importedDeviceIdentityType|[importedDeviceIdentityType](../resources/intune-enrollment-importeddeviceidentitytype.md)|Tipo de identidade de dispositivo importada. Os valores possíveis são: `unknown`, `imei`, `serialNumber`.|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação da descrição|
|createdDateTime|DateTimeOffset|Data e hora de criação do dispositivo|
|lastContactedDateTime|DateTimeOffset|Data e hora do último contato do dispositivo|
|description|String|A descrição do dispositivo|
|enrollmentid|[enrollmentid](../resources/intune-enrollment-enrollmentstate.md)|O estado do dispositivo no Intune. Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
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




