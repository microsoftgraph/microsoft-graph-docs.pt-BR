---
title: tipo de recurso importedAppleDeviceIdentity
description: O recurso importedAppleDeviceIdentity representa a identidade do dispositivo importado de um dispositivo Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f6b6addd7ee52793eb5bc6f1cb2888aa2f28417b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694953"
---
# <a name="importedappledeviceidentity-resource-type"></a>tipo de recurso importedAppleDeviceIdentity

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso importedAppleDeviceIdentity representa a identidade do dispositivo importado de um dispositivo Apple.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar importedAppleDeviceIdentities](../api/intune-enrollment-importedappledeviceidentity-list.md)|coleção [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Listar Propriedades e relações dos objetos [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .|
|[Obter importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-get.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Leia as propriedades e as relações do objeto [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .|
|[Criar importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-create.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Criar um novo objeto [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .|
|[Excluir importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-delete.md)|Nenhum|Exclui [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).|
|[Atualizar importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-update.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Atualiza as propriedades de um objeto [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .|
|[Ação importAppleDeviceIdentityList](../api/intune-enrollment-importedappledeviceidentity-importappledeviceidentitylist.md)|coleção [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|serialNumber|String|Número de série do dispositivo|
|requestedEnrollmentProfileId|String|ID do perfil de registro o administrador pretende aplicar ao dispositivo durante o próximo registro|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|O perfil de registro de tempo foi atribuído ao dispositivo|
|isSupervised|Boolean|Indica se o dispositivo Apple é supervisionado. Mais informações em: https://support.apple.com/HT202837|
|discoverySource|[discoverySource](../resources/intune-enrollment-discoverysource.md)|Fonte de descoberta de dispositivos Apple. Os valores possíveis são: `unknown`, `adminImport`, `deviceEnrollmentProgram`.|
|isDeleted|Boolean|Indica se o dispositivo é excluído do Apple Business Manager|
|createdDateTime|DateTimeOffset|Data e hora de criação do dispositivo|
|lastContactedDateTime|DateTimeOffset|Data e hora do último contato do dispositivo|
|description|String|A descrição do dispositivo|
|enrollmentid|[enrollmentid](../resources/intune-shared-enrollmentstate.md)|O estado do dispositivo no Intune. Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|plataforma|[plataforma](../resources/intune-enrollment-platform.md)|A plataforma do dispositivo. Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|

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





