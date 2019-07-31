---
title: tipo de recurso restrictedAppsViolation
description: Violação de perfil de configuração de aplicativos restritos por dispositivo por usuário
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 34c52c7d9d013563378ffbed4cb5af656c7c0502
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969727"
---
# <a name="restrictedappsviolation-resource-type"></a>tipo de recurso restrictedAppsViolation

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Violação de perfil de configuração de aplicativos restritos por dispositivo por usuário

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar restrictedAppsViolations](../api/intune-deviceconfig-restrictedappsviolation-list.md)|coleção [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Listar Propriedades e relações dos objetos [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .|
|[Obter restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-get.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Leia as propriedades e as relações do objeto [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .|
|[Criar restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-create.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Criar um novo objeto [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .|
|[Excluir restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-delete.md)|Nenhum|Exclui [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).|
|[Atualizar restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-update.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Atualiza as propriedades de um objeto [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo do objeto. Composto de AccountId, DeviceID, PolicyId e userId|
|userId|Cadeia de caracteres|O identificador exclusivo do usuário deve ser GUID|
|userName|Cadeia de caracteres|Nome de usuário|
|managedDeviceId|String|O identificador exclusivo do dispositivo gerenciado deve ser GUID|
|deviceName|String|Nome do dispositivo|
|deviceConfigurationId|String|O identificador exclusivo do perfil de configuração do dispositivo deve ser GUID|
|deviceConfigurationName|String|Nome do perfil de configuração do dispositivo|
|platformType|[policyPlatformType](../resources/intune-deviceconfig-policyplatformtype.md)|Tipo de plataforma. Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|restrictedAppsState|[restrictedAppsState](../resources/intune-deviceconfig-restrictedappsstate.md)|Estado de aplicativos restritos. Os valores possíveis são: `prohibitedApps` e `notApprovedApps`.|
|restrictedApps|coleção [managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)|Lista de aplicativos restritos violados|

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





