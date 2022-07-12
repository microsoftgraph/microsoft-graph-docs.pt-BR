---
title: Tipo de recurso deviceEnrollmentPlatformRestrictionsConfiguration
description: Configuração de Registro de Dispositivo que restringe os tipos de dispositivos que um usuário pode registrar
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f82847f8e224b2c50a966dd04763fdd35b91ae52
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730572"
---
# <a name="deviceenrollmentplatformrestrictionsconfiguration-resource-type"></a>Tipo de recurso deviceEnrollmentPlatformRestrictionsConfiguration

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Configuração de Registro de Dispositivo que restringe os tipos de dispositivos que um usuário pode registrar


Herda de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceEnrollmentPlatformRestrictionsConfigurations](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-list.md)|Conjunto [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|Listar propriedades e relações de objeto de [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).|
|[Obter deviceEnrollmentPlatformRestrictionsConfiguration](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-get.md)|[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|Ler propriedades e relações de objetos de [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).|
|[Criar deviceEnrollmentPlatformRestrictionsConfiguration](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-create.md)|[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|Criar um novo objeto de [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).|
|[Excluir deviceEnrollmentPlatformRestrictionsConfiguration](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-delete.md)|Nenhum|Excluir [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).|
|[Atualizar deviceEnrollmentPlatformRestrictionsConfiguration](../api/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration-update.md)|[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)|Atualizar as propriedades de um objeto de [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para a conta Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|displayName|String|O nome de exibição da configuração de registro do dispositivo Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|description|String|A descrição da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|prioridade|Int32|A prioridade é usada quando um usuário existe em vários grupos que recebem a configuração de registro. Os usuários estão sujeitos apenas à configuração com o valor de prioridade mais baixa. Herdada do [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|Data e hora de criação em UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação em UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|versão|Int32|A versão da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|iosRestriction|[deviceEnrollmentPlatformRestriction](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|Restrições de E/S com base na plataforma, na versão do sistema operacional da plataforma e na propriedade do dispositivo|
|windowsRestriction|[deviceEnrollmentPlatformRestriction](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|Restrições do Windows com base na plataforma, na versão do sistema operacional da plataforma e na propriedade do dispositivo|
|windowsMobileRestriction|[deviceEnrollmentPlatformRestriction](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|Restrições móveis do Windows com base na plataforma, na versão do sistema operacional da plataforma e na propriedade do dispositivo|
|androidRestriction|[deviceEnrollmentPlatformRestriction](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|Restrições do Android com base na plataforma, na versão do sistema operacional da plataforma e na propriedade do dispositivo|
|macOSRestriction|[deviceEnrollmentPlatformRestriction](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|Restrições do Mac com base na plataforma, na versão do sistema operacional da plataforma e na propriedade do dispositivo|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|atribuições|Conjunto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String"
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String"
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String"
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String"
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "String",
    "osMaximumVersion": "String"
  }
}
```





