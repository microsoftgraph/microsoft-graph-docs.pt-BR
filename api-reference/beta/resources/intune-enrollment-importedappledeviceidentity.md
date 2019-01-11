---
title: tipo de recurso de importedAppleDeviceIdentity
description: O recurso de importedAppleDeviceIdentity representa a identidade do dispositivo importadas de um dispositivo da Apple.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b7ad629721190b67e001ea56ca732eb325358768
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887441"
---
# <a name="importedappledeviceidentity-resource-type"></a>tipo de recurso de importedAppleDeviceIdentity

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

O recurso de importedAppleDeviceIdentity representa a identidade do dispositivo importadas de um dispositivo da Apple.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista importedAppleDeviceIdentities](../api/intune-enrollment-importedappledeviceidentity-list.md)|coleção [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Lista as propriedades e os relacionamentos dos objetos [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .|
|[Obter importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-get.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Leia as propriedades e os relacionamentos do objeto [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .|
|[Criar importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-create.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Crie um novo objeto de [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .|
|[Excluir importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-delete.md)|Nenhum|Exclui um [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md).|
|[Atualizar importedAppleDeviceIdentity](../api/intune-enrollment-importedappledeviceidentity-update.md)|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|Atualize as propriedades de um objeto [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) .|
|[ação de importAppleDeviceIdentityList](../api/intune-enrollment-importedappledeviceidentity-importappledeviceidentitylist.md)|coleção [importedAppleDeviceIdentityResult](../resources/intune-enrollment-importedappledeviceidentityresult.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|serialNumber|Cadeia de caracteres|Número de série do dispositivo|
|requestedEnrollmentProfileId|Cadeia de caracteres|Administração de Id de perfil de inscrição pretende aplicáveis ao dispositivo durante o próximo registro|
|requestedEnrollmentProfileAssignmentDateTime|DateTimeOffset|O perfil de inscrição de tempo foi atribuído ao dispositivo|
|isSupervised|Booliano|Indica se o dispositivo Apple seja supervisionado. Mais informações estão em:https://support.apple.com/en-us/HT202837|
|discoverySource|[discoverySource](../resources/intune-enrollment-discoverysource.md)|Fonte de descoberta do dispositivo Apple. Os valores possíveis são: `unknown`, `adminImport`, `deviceEnrollmentProgram`.|
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
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String"
}
```





