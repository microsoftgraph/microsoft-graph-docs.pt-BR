---
title: Criar deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Crie um novo objeto deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8e932b69a1d4a83d9f01bcf734c491556f0480e1
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34981185"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a>Criar deviceEnrollmentWindowsHelloForBusinessConfiguration

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

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
No corpo da solicitação, forneça uma representação JSON do objeto deviceEnrollmentWindowsHelloForBusinessConfiguration.

A tabela a seguir mostra as propriedades obrigatórias ao criar deviceEnrollmentWindowsHelloForBusinessConfiguration.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da conta herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|displayName|String|O nome de exibição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|descrição|String|A descrição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|prioridade|Int32|A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro. Os usuários estão sujeitos somente à configuração com o menor valor de prioridade. Herdada do [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|Data e hora de criação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação no UTC da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|versão|Int32|A versão da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|pinMinimumLength|Int32|Controla o número mínimo de caracteres necessários para o PIN do Windows Hello para empresas.  Esse valor deve estar entre 4 e 127, inclusive e menor ou igual ao valor definido para o PIN máximo.|
|pinMaximumLength|Int32|Controla o número máximo de caracteres permitido para o PIN do Windows Hello para empresas. Esse valor deve estar entre 4 e 127, inclusive. Esse valor deve ser maior ou igual ao valor definido para o PIN mínimo.|
|pinUppercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Controla a capacidade de usar letras maiúsculas no PIN do Windows Hello para empresas.  Permitido permite o uso de letras maiúsculas, enquanto que Required garante que estão presentes. Se definido como não permitido, as letras maiúsculas não serão permitidas. Os valores possíveis são: `allowed`, `required`, `disallowed`.|
|pinLowercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Controla a capacidade de usar letras minúsculas no PIN do Windows Hello para empresas.  Permitido permite o uso de letras minúsculas, enquanto que Required garante que estão presentes. Se definido como não permitido, as letras minúsculas não serão permitidas. Os valores possíveis são: `allowed`, `required`, `disallowed`.|
|pinSpecialCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Controla a capacidade de usar caracteres especiais no PIN do Windows Hello para empresas.  Permitido permite o uso de caracteres especiais, enquanto que Required garante que eles estão presentes. Se definido como não permitido, caracteres especiais não serão permitidos. Os valores possíveis são: `allowed`, `required`, `disallowed`.|
|estado|[habilitação](../resources/intune-shared-enablement.md)|Controla se é para permitir que o dispositivo seja configurado para o Windows Hello para empresas. Se for definido como desabilitado, o usuário não poderá provisionar o Windows Hello para empresas, exceto no Azure Active Directory que ingressou em telefones móveis, se for necessário. Se definido como não configurado, o Intune não substituirá os padrões do cliente. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|securityDeviceRequired|Booliano|Controla se é necessário exigir um TPM (Trusted Platform Module) para provisionar o Windows Hello para empresas. Um TPM oferece um benefício de segurança adicional nos dados armazenados nele que não podem ser usados em outros dispositivos. Se for definido como false, todos os dispositivos poderão provisionar o Windows Hello para empresas mesmo se não houver um TPM utilizável.|
|unlockWithBiometricsEnabled|Booliano|Controla o uso de gestos biométricos, como face e impressão digital, como uma alternativa para o PIN do Windows Hello para empresas.  Se for definido como false, os gestos biométricos não serão permitidos. Os usuários ainda devem configurar um PIN como um backup em caso de falhas.|
|remotePassportEnabled|Booliano|Controla o uso do Windows Hello para empresas remotos. O Windows Hello para empresas remotos permite que um dispositivo portátil e registrado possa ser usado como um complemento para autenticação de área de trabalho. A área de trabalho deve ser membro do Azure AD e o dispositivo complementar deve ter um PIN do Windows Hello para empresas.|
|pinPreviousBlockCount|Int32|Controla a capacidade de impedir que os usuários usem PINs passados. Isso deve ser definido entre 0 e 50, inclusive, e o PIN atual do usuário é incluído nessa contagem. Se for definido como 0, os PINs anteriores não serão armazenados. O histórico de PIN não é preservado por meio de uma redefinição de PIN.|
|pinExpirationInDays|Int32|Controla o período de tempo (em dias) que um PIN pode ser usado antes que o sistema exija que o usuário o altere. Isso deve ser definido entre 0 e 730, inclusive. Se definido como 0, o PIN do usuário nunca expirará|
|enhancedBiometricsState|[habilitação](../resources/intune-shared-enablement.md)|Controla a capacidade de usar os recursos antifalsificação para reconhecimento facial em dispositivos que dão suporte a ele. Se for definido como Disabled, os recursos anti-falsificação não serão permitidos. Se definido como não configurado, o usuário pode escolher se deseja usar anti-falsificação. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|securityKeyForSignIn|[habilitação](../resources/intune-shared-enablement.md)|Chave de segurança para entrar fornece a capacidade de ativar/desativar remotamente o Windows Hello sercurity Keyl não configurada honrará as configurações realizadas no clinet. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 667

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
  "enhancedBiometricsState": "enabled",
  "securityKeyForSignIn": "enabled"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 839

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
  "enhancedBiometricsState": "enabled",
  "securityKeyForSignIn": "enabled"
}
```





