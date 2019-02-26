---
title: Tipo de recurso deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4a2dbad17a731c8c63b6ef7705c97deab82a90da
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260988"
---
# <a name="deviceenrollmentwindowshelloforbusinessconfiguration-resource-type"></a>Tipo de recurso deviceEnrollmentWindowsHelloForBusinessConfiguration

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ainda não documentado


Herda de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceEnrollmentWindowsHelloForBusinessConfigurations](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-list.md)|Conjunto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)|Listar propriedades e relações de objetos de [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).|
|[Obter deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-get.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)|Ler propriedades e relações de objetos de [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).|
|[Criar deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-create.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)|Criar um novo objeto de [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).|
|[Excluir deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-delete.md)|Nenhum|Excluir [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).|
|[Atualizar deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-update.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)|Atualizar as propriedades de um objeto de [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|displayName|String|Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|description|Cadeia de caracteres|Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|prioridade|Int32|Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|version|Int32|Ainda não está documentado Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|pinMinimumLength|Int32|Ainda não documentado|
|pinMaximumLength|Int32|Ainda não documentado|
|pinUppercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Ainda não documentado. Os valores possíveis são: `allowed`, `required`, `disallowed`.|
|pinLowercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Ainda não documentado. Os valores possíveis são: `allowed`, `required`, `disallowed`.|
|pinSpecialCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Ainda não documentado. Os valores possíveis são: `allowed`, `required`, `disallowed`.|
|state|[habilitação](../resources/intune-onboarding-enablement.md)|Ainda não documentado. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|securityDeviceRequired|Booliano|Ainda não documentado|
|unlockWithBiometricsEnabled|Booliano|Ainda não documentado|
|remotePassportEnabled|Booliano|Ainda não documentado|
|pinPreviousBlockCount|Int32|Ainda não documentado|
|pinExpirationInDays|Int32|Ainda não documentado|
|enhancedBiometricsState|[habilitação](../resources/intune-onboarding-enablement.md)|Ainda não documentado. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|

## <a name="relationships"></a>Relacionamentos
|Relação|Tipo|Descrição|
|:---|:---|:---|
|atribuições|Conjunto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdada do [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "pinMinimumLength": 1024,
  "pinMaximumLength": 1024,
  "pinUppercaseCharactersUsage": "String",
  "pinLowercaseCharactersUsage": "String",
  "pinSpecialCharactersUsage": "String",
  "state": "String",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 1024,
  "pinExpirationInDays": 1024,
  "enhancedBiometricsState": "String"
}
```



