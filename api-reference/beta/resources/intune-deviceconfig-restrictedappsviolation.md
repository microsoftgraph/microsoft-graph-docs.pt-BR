---
title: tipo de recurso de restrictedAppsViolation
description: Violação de perfil de configuração de aplicativos restritos por dispositivo por usuário
ms.openlocfilehash: 6d7f6cb8b52671c311c39c3306a329ad37194b85
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039345"
---
# <a name="restrictedappsviolation-resource-type"></a>tipo de recurso de restrictedAppsViolation

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Violação de perfil de configuração de aplicativos restritos por dispositivo por usuário
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista restrictedAppsViolations](../api/intune-deviceconfig-restrictedappsviolation-list.md)|coleção [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Lista as propriedades e os relacionamentos dos objetos [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .|
|[Obter restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-get.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Leia as propriedades e os relacionamentos do objeto [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .|
|[Criar restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-create.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Crie um novo objeto de [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .|
|[Excluir restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-delete.md)|Nenhum|Exclui um [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).|
|[Atualizar restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-update.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Atualize as propriedades de um objeto [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para o objeto. Composto de accountId, deviceId, policyId e userId|
|userId|String|Identificador exclusivo do usuário, deve ser um Guid|
|userName|Cadeia de caracteres|Nome de usuário|
|managedDeviceId|String|Identificador exclusivo do dispositivo gerenciado, deve ser um Guid|
|deviceName|String|Nome do dispositivo|
|deviceConfigurationId|String|Identificador exclusivo do perfil do configuração de dispositivo, deve ser um Guid|
|deviceConfigurationName|String|Nome do perfil de configuração de dispositivo|
|platformType|[policyPlatformType](../resources/intune-deviceconfig-policyplatformtype.md)|Tipo de plataforma. Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|restrictedAppsState|[restrictedAppsState](../resources/intune-deviceconfig-restrictedappsstate.md)|Estado restrito de aplicativos. Os valores possíveis são: `prohibitedApps` e `notApprovedApps`.|
|restrictedApps|coleção [managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)|Lista de aplicativos restritos violadas|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.restrictedAppsViolation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.restrictedAppsViolation",
  "id": "String (identifier)",
  "userId": "String",
  "userName": "String",
  "managedDeviceId": "String",
  "deviceName": "String",
  "deviceConfigurationId": "String",
  "deviceConfigurationName": "String",
  "platformType": "String",
  "restrictedAppsState": "String",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.managedDeviceReportedApp",
      "appId": "String"
    }
  ]
}
```





