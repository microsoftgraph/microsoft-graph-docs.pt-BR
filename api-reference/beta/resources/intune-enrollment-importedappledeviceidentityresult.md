---
title: Tipo de recurso importedAppleDeviceIdentityResult
description: O recurso importedAppleDeviceIdentityResult representa o resultado da tentativa de importar identidades de dispositivos Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ac4cf24a6b6ec28add8345a080aa9c701a95e499f330b1e67bde3912ccd185c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54197951"
---
# <a name="importedappledeviceidentityresult-resource-type"></a>Tipo de recurso importedAppleDeviceIdentityResult

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso importedAppleDeviceIdentityResult representa o resultado da tentativa de importar identidades de dispositivos Apple.


Herda de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar importedAppleDeviceIdentityResults](../api/intune-enrollment-importedappledeviceidentityresult-list.md)|[Coleção importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)|Listar propriedades e relações dos [objetos importedAppleDeviceIdentityResult.](../resources/intune-enrollment-importedappledeviceidentityresult.md)|
|[Obter importedAppleDeviceIdentityResult](../api/intune-enrollment-importedappledeviceidentityresult-get.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)|Leia propriedades e relações do [objeto importedAppleDeviceIdentityResult.](../resources/intune-enrollment-importedappledeviceidentityresult.md)|
|[Criar importedAppleDeviceIdentityResult](../api/intune-enrollment-importedappledeviceidentityresult-create.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)|Crie um novo [objeto importedAppleDeviceIdentityResult.](../resources/intune-enrollment-importedappledeviceidentityresult.md)|
|[Excluir importedAppleDeviceIdentityResult](../api/intune-enrollment-importedappledeviceidentityresult-delete.md)|Nenhum|Exclui um [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md).|
|[Atualizar importedAppleDeviceIdentityResult](../api/intune-enrollment-importedappledeviceidentityresult-update.md)|[importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)|Atualize as propriedades de [um objeto importedAppleDeviceIdentityResult.](../resources/intune-enrollment-importedappledeviceidentityresult.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado [de importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|serialNumber|String|Número de série do dispositivo Herdado [de importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|requestedEnrollmentProfileId|Cadeia de caracteres|O administrador de ID do perfil de registro pretende aplicar-se ao dispositivo durante o próximo registro Herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|O perfil de registro de hora foi atribuído ao dispositivo Herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|isSupervised|Boolean|Indica se o dispositivo Apple é supervisionado. Mais informações estão em: https://support.apple.com/en-us/HT202837 Herdada de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|discoverySource|[discoverySource](../resources/intune-enrollment-discoverysource.md)|Fonte de descoberta de dispositivo Apple. Herdado [de importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md). Os valores possíveis são: `unknown`, `adminImport`, `deviceEnrollmentProgram`.|
|isDeleted|Boolean|Indica se o dispositivo é excluído do Apple Business Manager Herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|createdDateTime|DateTimeOffset|Data de criação Hora do dispositivo Herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|lastContactedDateTime|DateTimeOffset|Última Data contatada Hora do dispositivo Herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|description|Cadeia de caracteres|A descrição do dispositivo Herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|
|enrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|O estado do dispositivo no Intune Herdado de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md). Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|plataforma|[platform](../resources/intune-enrollment-platform.md)|A plataforma do Dispositivo. Herdado [de importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md). Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|
|status|Boolean|Status da identidade do dispositivo importado|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedAppleDeviceIdentityResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
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
  "platform": "String",
  "status": true
}
```




