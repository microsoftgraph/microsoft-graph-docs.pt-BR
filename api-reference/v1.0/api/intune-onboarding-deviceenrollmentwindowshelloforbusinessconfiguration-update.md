---
title: Atualizar deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Atualize as propriedades de um objeto deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 042a3a0b7ee43e0720f7124059563253e1bc3bcb
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66733504"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a>Atualizar deviceEnrollmentWindowsHelloForBusinessConfiguration

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de um objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).

A tabela a seguir mostra as propriedades obrigatórias ao criar [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para a conta Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|displayName|String|O nome de exibição da configuração de registro do dispositivo Herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|description|String|A descrição da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|prioridade|Int32|A prioridade é usada quando um usuário existe em vários grupos que recebem a configuração de registro. Os usuários estão sujeitos apenas à configuração com o valor de prioridade mais baixa. Herdada do [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|Data e hora de criação em UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação em UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|versão|Int32|A versão da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|pinMinimumLength|Int32|Controla o número mínimo de caracteres necessários para a Windows Hello para Empresas PIN.  Esse valor deve estar entre 4 e 127, inclusive, e menor ou igual ao valor definido para o PIN máximo.|
|pinMaximumLength|Int32|Controla o número máximo de caracteres permitidos para o PIN Windows Hello para Empresas dados. Esse valor deve estar entre 4 e 127, inclusive. Esse valor deve ser maior ou igual ao valor definido para o PIN mínimo.|
|pinUppercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Controla a capacidade de usar letras maiúsculas no WINDOWS HELLO PARA EMPRESAS PIN.  Permitido permite o uso de letras maiúsculas, enquanto Obrigatório garante que elas estejam presentes. Se definido como Não Permitido, letras maiúsculas não serão permitidas. Os valores possíveis são: `allowed`, `required`, `disallowed`.|
|pinLowercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Controla a capacidade de usar letras minúsculas no WINDOWS HELLO PARA EMPRESAS PIN.  Permitido permite o uso de letras minúsculas, enquanto Obrigatório garante que elas estejam presentes. Se definido como Não Permitido, letras minúsculas não serão permitidas. Os valores possíveis são: `allowed`, `required`, `disallowed`.|
|pinSpecialCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Controla a capacidade de usar caracteres especiais na Windows Hello para Empresas PIN.  Permitido permite o uso de caracteres especiais, enquanto Obrigatório garante que eles estejam presentes. Se definido como Não Permitido, caracteres especiais não serão permitidos. Os valores possíveis são: `allowed`, `required`, `disallowed`.|
|state|[Capacitação](../resources/intune-onboarding-enablement.md)|Controla se o dispositivo deve ser configurado para Windows Hello para Empresas. Se definido como desabilitado, o usuário não poderá provisionar Windows Hello para Empresas exceto em telefones móveis ingressados no Azure Active Directory, se necessário. Se definido como Não Configurado, o Intune substituirá os padrões do cliente. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|securityDeviceRequired|Booliano|Controla se é necessário um TPM (Trusted Platform Module) para provisionamento Windows Hello para Empresas. Um TPM fornece um benefício de segurança adicional em que os dados armazenados nele não podem ser usados em outros dispositivos. Se definido como False, todos os dispositivos poderão provisionar Windows Hello para Empresas mesmo que não haja um TPM utilizável.|
|unlockWithBiometricsEnabled|Booliano|Controla o uso de gestos biométricos, como rosto e impressão digital, como uma alternativa ao PIN Windows Hello para Empresas dados.  Se definido como False, gestos biométricos não serão permitidos. Os usuários ainda devem configurar um PIN como um backup em caso de falhas.|
|remotePassportEnabled|Booliano|Controla o uso de controles Windows Hello para Empresas. O Windows Hello para Empresas remoto fornece a capacidade de um dispositivo portátil e registrado ser utilizável como um complemento para autenticação da área de trabalho. A área de trabalho deve Azure AD ingressada e o dispositivo complementar deve ter Windows Hello para Empresas PIN.|
|pinPreviousBlockCount|Int32|Controla a capacidade de impedir que os usuários usem PINs anteriores. Isso deve ser definido entre 0 e 50, inclusive, e o PIN atual do usuário está incluído nessa contagem. Se definido como 0, os PINs anteriores não serão armazenados. O histórico de PIN não é preservado por meio de uma redefinição de PIN.|
|pinExpirationInDays|Int32|Controla o período de tempo (em dias) que um PIN pode ser usado antes que o sistema exija que o usuário o altere. Isso deve ser definido entre 0 e 730, inclusive. Se definido como 0, o PIN do usuário nunca expirará|
|enhancedBiometricsState|[Capacitação](../resources/intune-onboarding-enablement.md)|Controla a capacidade de usar os recursos antifalsificação para reconhecimento facial em dispositivos que dão suporte a ele. Se definido como desabilitado, os recursos antifalsificação não serão permitidos. Se definido como Não Configurado, o usuário poderá escolher se deseja usar antifalsificação. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 629

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 801

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "id": "3068e0cd-e0cd-3068-cde0-6830cde06830",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled"
}
```





