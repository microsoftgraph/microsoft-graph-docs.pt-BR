---
title: Tipo de recurso importedDeviceIdentity
description: O recurso importedDeviceIdentity representa uma identidade de hardware exclusiva de um dispositivo que foi pré-em estágios para configuração de pré-registro.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c18a744e9a0a3aa7597c4d3d017e39b975be7693
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033487"
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
|[Excluir importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-delete.md)|Nenhum|Exclui um [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).|
|[Atualizar importedDeviceIdentity](../api/intune-enrollment-importeddeviceidentity-update.md)|[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Atualize as propriedades de [um objeto importedDeviceIdentity.](../resources/intune-enrollment-importeddeviceidentity.md)|
|[Ação importDeviceIdentityList](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|[Coleção importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)|Ainda não documentado|
|[Ação searchExistingIdentities](../api/intune-enrollment-importeddeviceidentity-searchexistingidentities.md)|[Coleção importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID da identidade do dispositivo importado|
|importedDeviceIdentifier|Cadeia de Caracteres|Identificador de Dispositivo Importado|
|importedDeviceIdentityType|[importedDeviceIdentityType](../resources/intune-enrollment-importeddeviceidentitytype.md)|Tipo de Identidade de Dispositivo Importado. Os valores possíveis são: `unknown`, `imei`, `serialNumber`.|
|lastModifiedDateTime|DateTimeOffset|Last Modified DateTime of the description|
|createdDateTime|DateTimeOffset|Data de criação hora do dispositivo|
|lastContactedDateTime|DateTimeOffset|Hora da Última Data Contata do dispositivo|
|description|String|A descrição do dispositivo|
|enrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|O estado do dispositivo no Intune. Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|plataforma|[platform](../resources/intune-enrollment-platform.md)|A plataforma do Dispositivo. Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|

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



