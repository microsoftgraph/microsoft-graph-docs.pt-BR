---
title: Tipo de recurso restrictedAppsViolation
description: Violação do perfil de configuração de aplicativos restritos por dispositivo por usuário
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a328938975b67ebce005f3cee05fb753f051ad49
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665508"
---
# <a name="restrictedappsviolation-resource-type"></a>Tipo de recurso restrictedAppsViolation

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Violação do perfil de configuração de aplicativos restritos por dispositivo por usuário

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar restrictedAppsViolations](../api/intune-deviceconfig-restrictedappsviolation-list.md)|[Coleção restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Listar propriedades e relações dos objetos [restrictedAppsViolation.](../resources/intune-deviceconfig-restrictedappsviolation.md)|
|[Obter restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-get.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Leia propriedades e relações do objeto [restrictedAppsViolation.](../resources/intune-deviceconfig-restrictedappsviolation.md)|
|[Criar restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-create.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Crie um novo [objeto restrictedAppsViolation.](../resources/intune-deviceconfig-restrictedappsviolation.md)|
|[Excluir restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-delete.md)|Nenhuma|Exclui um [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).|
|[Atualizar restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-update.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Atualize as propriedades de [um objeto restrictedAppsViolation.](../resources/intune-deviceconfig-restrictedappsviolation.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo do objeto. Composto por accountId, deviceId, policyId e userId|
|userId|Cadeia de caracteres|Identificador exclusivo do usuário, deve ser Guid|
|userName|Cadeia de caracteres|Nome de usuário|
|managedDeviceId|String|Identificador exclusivo do dispositivo gerenciado, deve ser Guid|
|deviceName|String|Nome do dispositivo|
|deviceConfigurationId|String|Identificador exclusivo do perfil de configuração do dispositivo, deve ser Guid|
|deviceConfigurationName|String|Nome do perfil de configuração do dispositivo|
|platformType|[policyPlatformType](../resources/intune-shared-policyplatformtype.md)|Tipo de plataforma. Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `androidAOSP`, `all`.|
|restrictedAppsState|[restrictedAppsState](../resources/intune-deviceconfig-restrictedappsstate.md)|Estado de aplicativos restritos. Os valores possíveis são: `prohibitedApps` e `notApprovedApps`.|
|restrictedApps|[Coleção managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)|Lista de aplicativos restritos violados|

## <a name="relationships"></a>Relações
Nenhuma

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




