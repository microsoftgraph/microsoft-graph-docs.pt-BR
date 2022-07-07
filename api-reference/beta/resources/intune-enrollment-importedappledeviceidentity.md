---
title: Tipo de recurso importedAppleDeviceIdentity
description: O recurso importedAppleDeviceIdentity representa a identidade do dispositivo importado de um dispositivo Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5355f273e2e6535eb877d72efc7e1718fe04e87e
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66669060"
---
# <a name="importedappledeviceidentity-resource-type"></a>Tipo de recurso importedAppleDeviceIdentity

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso importedAppleDeviceIdentity representa a identidade do dispositivo importado de um dispositivo Apple.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar importedAppleDeviceIdentities](../api/intune-enrollment-importedappledeviceidentity-list.md)|[Coleção importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Listar propriedades e relações dos [objetos importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .|
|[Obter importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-get.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Ler propriedades e relações do [objeto importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .|
|[Criar importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-create.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Crie um novo [objeto importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .|
|[Excluir importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-delete.md)|Nenhum|Exclui um [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).|
|[Atualizar importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-update.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Atualize as propriedades de [um objeto importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .|
|[Ação importAppleDeviceIdentityList](../api/intune-enrollment-importedappledeviceidentity-importappledeviceidentitylist.md)|[Coleção importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|serialNumber|String|Número de série do dispositivo|
|requestedEnrollmentProfileId|Cadeia de caracteres|O administrador da ID do perfil de registro pretende aplicar ao dispositivo durante o próximo registro|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|O perfil de registro de tempo foi atribuído ao dispositivo|
|isSupervised|Boolean|Indica se o dispositivo Apple é supervisionado. Mais informações estão em: https://support.apple.com/en-us/HT202837|
|discoverySource|[discoverySource](../resources/intune-enrollment-discoverysource.md)|Origem da descoberta de dispositivos da Apple. Os valores possíveis são: `unknown`, `adminImport`, `deviceEnrollmentProgram`.|
|isDeleted|Booleano|Indica se o dispositivo foi excluído do Apple Business Manager|
|createdDateTime|DateTimeOffset|Data e hora de criação do dispositivo|
|lastContactedDateTime|DateTimeOffset|Hora da Data do Último Contato do dispositivo|
|descrição|Cadeia de caracteres|A descrição do dispositivo|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|O estado do dispositivo em Intune. Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|plataforma|[Plataforma](../resources/intune-enrollment-platform.md)|A plataforma do dispositivo. Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedAppleDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
  "id": "String (identifier)",
  "serialNumber": "String",
  "requestedEnrollmentProfileId": "String",
  "requestedEnrollmentProfileAssignmentDateTime": "String (timestamp)",
  "isSupervised": true,
  "discoverySource": "String",
  "isDeleted": true,
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String"
}
```




