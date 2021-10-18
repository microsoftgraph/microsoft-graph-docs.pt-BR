---
title: Criar deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Crie um novo objeto deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a2b7cb4dd160e282a19a9a32b0798ef3c7653ede
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60457432"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a>Criar deviceEnrollmentWindowsHelloForBusinessConfiguration

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementServiceConfig.ReadWrite.All|

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
|id|Cadeia de caracteres|Identificador exclusivo da conta Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|displayName|String|O nome de exibição da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|description|Cadeia de caracteres|A descrição da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|prioridade|Int32|A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro. Os usuários estão sujeitos apenas à configuração com o valor de prioridade mais baixo. Herdada do [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|Hora de data criada em UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Última data de modificação no UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|versão|Int32|A versão da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|pinMinimumLength|Int32|Controla o número mínimo de caracteres necessário para o pin Windows Hello para Empresas.  Esse valor deve estar entre 4 e 127, inclusive, e menor ou igual ao valor definido para o PIN máximo.|
|pinMaximumLength|Int32|Controla o número máximo de caracteres permitidos para o PIN Windows Hello para Empresas. Esse valor deve estar entre 4 e 127, inclusive. Esse valor deve ser maior ou igual ao valor definido para o PIN mínimo.|
|pinUppercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Controla a capacidade de usar letras maiúsculas no pin Windows Hello para Empresas.  Permitido permite o uso de letras maiúsculas, enquanto Required garante que elas estão presentes. Se definido como Não Permitido, as letras maiúsculas não serão permitidas. Os valores possíveis são: `allowed`, `required`, `disallowed`.|
|pinLowercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Controla a capacidade de usar letras minúsculas no pin Windows Hello para Empresas.  Permitido permite o uso de letras minúsculas, enquanto Required garante que elas estão presentes. Se definido como Não Permitido, as letras minúsculas não serão permitidas. Os valores possíveis são: `allowed`, `required`, `disallowed`.|
|pinSpecialCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Controla a capacidade de usar caracteres especiais no pin Windows Hello para Empresas.  Permitido permite o uso de caracteres especiais, enquanto Obrigatório garante que eles estão presentes. Se definido como Não Permitido, caracteres especiais não serão permitidos. Os valores possíveis são: `allowed`, `required`, `disallowed`.|
|state|[enablement](../resources/intune-onboarding-enablement.md)|Controla se o dispositivo deve ser configurado para Windows Hello para Empresas. Se estiver definido como desabilitado, o usuário não poderá provisionar Windows Hello para Empresas, exceto em Azure Active Directory celulares ingressados, se necessário. Se definido como Não Configurado, o Intune não substituirá os padrões do cliente. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|securityDeviceRequired|Booliano|Controla se é necessário um TPM (Trusted Platform Module) para provisionamento Windows Hello para Empresas. Um TPM fornece um benefício adicional de segurança, já que os dados armazenados nele não podem ser usados em outros dispositivos. Se definido como False, todos os dispositivos podem provisionar Windows Hello para Empresas, mesmo que não haja um TPM usável.|
|unlockWithBiometricsEnabled|Booliano|Controla o uso de gestos biométricos, como face e impressão digital, como uma alternativa ao PIN Windows Hello para Empresas.  Se definido como False, gestos biométricos não são permitidos. Os usuários ainda devem configurar um PIN como backup em caso de falhas.|
|remotePassportEnabled|Booliano|Controla o uso de controle remoto Windows Hello para Empresas. O Windows Hello remoto para Empresas fornece a capacidade de um dispositivo portátil e registrado ser usável como um parceiro para autenticação da área de trabalho. A área de trabalho deve ser ingressada no Azure AD e o dispositivo de suporte deve ter um pin Windows Hello para Empresas.|
|pinPreviousBlockCount|Int32|Controla a capacidade de impedir que os usuários usem PINs anteriores. Isso deve ser definido entre 0 e 50, inclusive, e o PIN atual do usuário está incluído nessa contagem. Se definido como 0, os PINs anteriores não serão armazenados. O histórico de PIN não é preservado por meio de uma redefinição de PIN.|
|pinExpirationInDays|Int32|Controla o período de tempo (em dias) que um PIN pode ser usado antes que o sistema exija que o usuário o altere. Isso deve ser definido entre 0 e 730, inclusive. Se definido como 0, o PIN do usuário nunca expirará|
|enhancedBiometricsState|[enablement](../resources/intune-onboarding-enablement.md)|Controla a capacidade de usar os recursos anti-spoofing para reconhecimento facial em dispositivos que o suportam. Se definido como desabilitado, os recursos anti-spoofing não são permitidos. Se definido como Não Configurado, o usuário poderá escolher se deseja usar anti-spoofing. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
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
HTTP/1.1 201 Created
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



