---
title: Tipo de recurso importedDeviceIdentity
description: O recurso importedDeviceIdentity representa uma identidade de hardware exclusiva de um dispositivo que foi pré-em estágios para configuração de pré-registro.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f1dbcb41d30bec09335316503fbc8f93f6264c34
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58803487"
---
# <a name="importeddeviceidentity-resource-type"></a>Tipo de recurso importedDeviceIdentity

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso importedDeviceIdentity representa uma identidade de hardware exclusiva de um dispositivo que foi pré-em estágios para configuração de pré-registro.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar importedDeviceIdentities](../api/intune-enrollment-importeddeviceidentity-list.md)|[Coleção importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Listar propriedades e relações dos [objetos importedDeviceIdentity.](../resources/intune-enrollment-importeddeviceidentity.md)|
|[Obter importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-get.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Leia propriedades e relações do [objeto importedDeviceIdentity.](../resources/intune-enrollment-importeddeviceidentity.md)|
|[Criar importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-create.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Crie um novo [objeto importedDeviceIdentity.](../resources/intune-enrollment-importeddeviceidentity.md)|
|[Excluir importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-delete.md)|Nenhum(a)|Exclui um [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).|
|[Atualizar importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-update.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Atualize as propriedades de [um objeto importedDeviceIdentity.](../resources/intune-enrollment-importeddeviceidentity.md)|
|[Ação importDeviceIdentityList](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|[Coleção importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|Ainda não documentado|
|[Ação searchExistingIdentities](../api/intune-enrollment-importeddeviceidentity-searchexistingidentities.md)|[Coleção importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID da identidade do dispositivo importado|
|importedDeviceIdentifier|Cadeia de caracteres|Identificador de Dispositivo Importado|
|importedDeviceIdentityType|[importedDeviceIdentityType](../resources/intune-enrollment-importeddeviceidentitytype.md)|Tipo de Identidade de Dispositivo Importado. Os valores possíveis são: `unknown`, `imei`, `serialNumber`.|
|lastModifiedDateTime|DateTimeOffset|Last Modified DateTime of the description|
|createdDateTime|DateTimeOffset|Data de criação hora do dispositivo|
|lastContactedDateTime|DateTimeOffset|Hora da Última Data Contata do dispositivo|
|descrição|Cadeia de caracteres|A descrição do dispositivo|
|enrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|O estado do dispositivo no Intune. Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|plataforma|[plataforma](../resources/intune-enrollment-platform.md)|A plataforma do Dispositivo. Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|

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



