---
title: Tipo de recurso deviceComanagementAuthorityConfiguration
description: configuração Windows 10 Co-Management página autoridade de segurança
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ae2f690a1e1ee10c606eeb7c880be2152cd45951
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210231"
---
# <a name="devicecomanagementauthorityconfiguration-resource-type"></a>Tipo de recurso deviceComanagementAuthorityConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

configuração Windows 10 Co-Management página autoridade de segurança


Herda de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceComanagementAuthorityConfigurations](../api/intune-onboarding-devicecomanagementauthorityconfiguration-list.md)|[Coleção deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)|Listar propriedades e relações dos [objetos deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) .|
|[Obter deviceComanagementAuthorityConfiguration](../api/intune-onboarding-devicecomanagementauthorityconfiguration-get.md)|[deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)|Ler propriedades e relações do objeto [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) .|
|[Criar deviceComanagementAuthorityConfiguration](../api/intune-onboarding-devicecomanagementauthorityconfiguration-create.md)|[deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)|Crie um novo [objeto deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) .|
|[Excluir deviceComanagementAuthorityConfiguration](../api/intune-onboarding-devicecomanagementauthorityconfiguration-delete.md)|Nenhuma|Exclui um [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md).|
|[Atualizar deviceComanagementAuthorityConfiguration](../api/intune-onboarding-devicecomanagementauthorityconfiguration-update.md)|[deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md)|Atualize as propriedades de [um objeto deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo para a conta Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|displayName|String|O nome de exibição da configuração de registro do dispositivo Herdado de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|descrição|Cadeia de caracteres|A descrição da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|prioridade|Int32|A prioridade é usada quando um usuário existe em vários grupos que recebem a configuração de registro. Os usuários estão sujeitos apenas à configuração com o valor de prioridade mais baixa. Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|Data e hora de criação em UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação em UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|versão|Int32|A versão da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|roleScopeTagIds|Conjunto de cadeias de caracteres|Marcas de escopo de função opcionais para as restrições de registro. Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|deviceEnrollmentConfigurationType|[deviceEnrollmentConfigurationType](../resources/intune-onboarding-deviceenrollmentconfigurationtype.md)|Suporte para o tipo de configuração de registro herdado de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md). Os valores possíveis são: `unknown`, `limit`, `platformRestrictions`, `windowsHelloForBusiness`, `defaultLimit`, `defaultPlatformRestrictions`, `defaultWindowsHelloForBusiness`, `defaultWindows10EnrollmentCompletionPageConfiguration`, `windows10EnrollmentCompletionPageConfiguration`, `deviceComanagementAuthorityConfiguration`, `singlePlatformRestriction`, `unknownFutureValue` e `enrollmentNotificationsConfiguration`.|
|managedDeviceAuthority|Int32|Configuração da Autoridade de Gerenciamento CoManagement ManagedDeviceAuthority|
|installConfigurationManagerAgent|Booliano|Configuração da Autoridade de Gerenciamento CoManagement InstallConfigurationManagerAgent|
|configurationManagerAgentCommandLineArgument|Cadeia de Caracteres|Configuração da Autoridade de Gerenciamento CoManagement ConfigurationManagerAgentCommandLineArgument|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|atribuições|Conjunto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo Herdado de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComanagementAuthorityConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComanagementAuthorityConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "roleScopeTagIds": [
    "String"
  ],
  "deviceEnrollmentConfigurationType": "String",
  "managedDeviceAuthority": 1024,
  "installConfigurationManagerAgent": true,
  "configurationManagerAgentCommandLineArgument": "String"
}
```




