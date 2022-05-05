---
title: Criar deviceComanagementAuthorityConfiguration
description: Crie um novo objeto deviceComanagementAuthorityConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cd8a36ea8b23099e83cd23abf4f062249c13defd
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206143"
---
# <a name="create-devicecomanagementauthorityconfiguration"></a>Criar deviceComanagementAuthorityConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto deviceComanagementAuthorityConfiguration.

A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComanagementAuthorityConfiguration.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo para a conta Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|displayName|Cadeia de caracteres|O nome de exibição da configuração de registro do dispositivo Herdado de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|descrição|String|A descrição da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|prioridade|Int32|A prioridade é usada quando um usuário existe em vários grupos que recebem a configuração de registro. Os usuários estão sujeitos apenas à configuração com o valor de prioridade mais baixa. Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|Data e hora de criação em UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação em UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|versão|Int32|A versão da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|roleScopeTagIds|Conjunto de cadeias de caracteres|Marcas de escopo de função opcionais para as restrições de registro. Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|deviceEnrollmentConfigurationType|[deviceEnrollmentConfigurationType](../resources/intune-onboarding-deviceenrollmentconfigurationtype.md)|Suporte para o tipo de configuração de registro herdado de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md). Os valores possíveis são: `unknown`, `limit`, `platformRestrictions`, `windowsHelloForBusiness`, `defaultLimit`, `defaultPlatformRestrictions`, `defaultWindowsHelloForBusiness`, `defaultWindows10EnrollmentCompletionPageConfiguration`, `windows10EnrollmentCompletionPageConfiguration`, `deviceComanagementAuthorityConfiguration`, `singlePlatformRestriction`, `unknownFutureValue` e `enrollmentNotificationsConfiguration`.|
|managedDeviceAuthority|Int32|Configuração da Autoridade de Gerenciamento CoManagement ManagedDeviceAuthority|
|installConfigurationManagerAgent|Booliano|Configuração da Autoridade de Gerenciamento CoManagement InstallConfigurationManagerAgent|
|configurationManagerAgentCommandLineArgument|Cadeia de Caracteres|Configuração da Autoridade de Gerenciamento CoManagement ConfigurationManagerAgentCommandLineArgument|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceComanagementAuthorityConfiguration](../resources/intune-onboarding-devicecomanagementauthorityconfiguration.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 494

{
  "@odata.type": "#microsoft.graph.deviceComanagementAuthorityConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "deviceEnrollmentConfigurationType": "limit",
  "managedDeviceAuthority": 6,
  "installConfigurationManagerAgent": true,
  "configurationManagerAgentCommandLineArgument": "Configuration Manager Agent Command Line Argument value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 666

{
  "@odata.type": "#microsoft.graph.deviceComanagementAuthorityConfiguration",
  "id": "0ba0057f-057f-0ba0-7f05-a00b7f05a00b",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "deviceEnrollmentConfigurationType": "limit",
  "managedDeviceAuthority": 6,
  "installConfigurationManagerAgent": true,
  "configurationManagerAgentCommandLineArgument": "Configuration Manager Agent Command Line Argument value"
}
```




