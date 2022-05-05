---
title: Tipo de recurso deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Windows Hello para Empresas configurações permitem que os usuários acessem seus dispositivos usando um gesto, como autenticação biométrica ou um PIN. Defina as configurações para Windows 10, Windows 10 Mobile e posterior.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 79213079fb72a151994f65aed178f85b85d27c67
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209881"
---
# <a name="deviceenrollmentwindowshelloforbusinessconfiguration-resource-type"></a>Tipo de recurso deviceEnrollmentWindowsHelloForBusinessConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Windows Hello para Empresas configurações permitem que os usuários acessem seus dispositivos usando um gesto, como autenticação biométrica ou um PIN. Defina as configurações para Windows 10, Windows 10 Mobile e posterior.


Herda de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)

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
|id|Cadeia de caracteres|Identificador exclusivo para a conta Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|displayName|Cadeia de caracteres|O nome de exibição da configuração de registro do dispositivo Herdado de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|descrição|Cadeia de caracteres|A descrição da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|prioridade|Int32|A prioridade é usada quando um usuário existe em vários grupos que recebem a configuração de registro. Os usuários estão sujeitos apenas à configuração com o valor de prioridade mais baixa. Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|Data e hora de criação em UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação em UTC da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|versão|Int32|A versão da configuração de registro de dispositivo Herdada de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|roleScopeTagIds|Conjunto de cadeias de caracteres|Marcas de escopo de função opcionais para as restrições de registro. Herdada do [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|deviceEnrollmentConfigurationType|[deviceEnrollmentConfigurationType](../resources/intune-onboarding-deviceenrollmentconfigurationtype.md)|Suporte para o tipo de configuração de registro herdado de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md). Os valores possíveis são: `unknown`, `limit`, `platformRestrictions`, `windowsHelloForBusiness`, `defaultLimit`, `defaultPlatformRestrictions`, `defaultWindowsHelloForBusiness`, `defaultWindows10EnrollmentCompletionPageConfiguration`, `windows10EnrollmentCompletionPageConfiguration`, `deviceComanagementAuthorityConfiguration`, `singlePlatformRestriction`, `unknownFutureValue` e `enrollmentNotificationsConfiguration`.|
|pinMinimumLength|Int32|Controla o número mínimo de caracteres necessários para a Windows Hello para Empresas PIN.  Esse valor deve estar entre 4 e 127, inclusive, e menor ou igual ao valor definido para o PIN máximo.|
|pinMaximumLength|Int32|Controla o número máximo de caracteres permitidos para o PIN Windows Hello para Empresas dados. Esse valor deve estar entre 4 e 127, inclusive. Esse valor deve ser maior ou igual ao valor definido para o PIN mínimo.|
|pinUppercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Controla a capacidade de usar letras maiúsculas no WINDOWS HELLO PARA EMPRESAS PIN.  Permitido permite o uso de letras maiúsculas, enquanto Obrigatório garante que elas estejam presentes. Se definido como Não Permitido, letras maiúsculas não serão permitidas. Os valores possíveis são: `allowed`, `required`, `disallowed`.|
|pinLowercaseCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Controla a capacidade de usar letras minúsculas no WINDOWS HELLO PARA EMPRESAS PIN.  Permitido permite o uso de letras minúsculas, enquanto Obrigatório garante que elas estejam presentes. Se definido como Não Permitido, letras minúsculas não serão permitidas. Os valores possíveis são: `allowed`, `required`, `disallowed`.|
|pinSpecialCharactersUsage|[windowsHelloForBusinessPinUsage](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Controla a capacidade de usar caracteres especiais na Windows Hello para Empresas PIN.  Permitido permite o uso de caracteres especiais, enquanto Obrigatório garante que eles estejam presentes. Se definido como Não Permitido, caracteres especiais não serão permitidos. Os valores possíveis são: `allowed`, `required`, `disallowed`.|
|estado|[Capacitação](../resources/intune-shared-enablement.md)|Controla se o dispositivo deve ser configurado para Windows Hello para Empresas. Se definido como desabilitado, o usuário não poderá provisionar Windows Hello para Empresas exceto em Azure Active Directory celulares ingressados, se necessário. Se definido como Não Configurado, o Intune substituirá os padrões do cliente. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|securityDeviceRequired|Booliano|Controla se é necessário um TPM (Trusted Platform Module) para provisionamento Windows Hello para Empresas. Um TPM fornece um benefício de segurança adicional em que os dados armazenados nele não podem ser usados em outros dispositivos. Se definido como False, todos os dispositivos poderão provisionar Windows Hello para Empresas mesmo que não haja um TPM utilizável.|
|unlockWithBiometricsEnabled|Booliano|Controla o uso de gestos biométricos, como rosto e impressão digital, como uma alternativa ao PIN Windows Hello para Empresas dados.  Se definido como False, gestos biométricos não serão permitidos. Os usuários ainda devem configurar um PIN como um backup em caso de falhas.|
|remotePassportEnabled|Booliano|Controla o uso de controles Windows Hello para Empresas. O Windows Hello para Empresas remoto fornece a capacidade de um dispositivo portátil e registrado ser utilizável como um complemento para autenticação da área de trabalho. A área de trabalho deve Azure AD ingressada e o dispositivo complementar deve ter Windows Hello para Empresas PIN.|
|pinPreviousBlockCount|Int32|Controla a capacidade de impedir que os usuários usem PINs anteriores. Isso deve ser definido entre 0 e 50, inclusive, e o PIN atual do usuário está incluído nessa contagem. Se definido como 0, os PINs anteriores não serão armazenados. O histórico de PIN não é preservado por meio de uma redefinição de PIN.|
|pinExpirationInDays|Int32|Controla o período de tempo (em dias) que um PIN pode ser usado antes que o sistema exija que o usuário o altere. Isso deve ser definido entre 0 e 730, inclusive. Se definido como 0, o PIN do usuário nunca expirará|
|enhancedBiometricsState|[Capacitação](../resources/intune-shared-enablement.md)|Controla a capacidade de usar os recursos antifalsificação para reconhecimento facial em dispositivos que dão suporte a ele. Se definido como desabilitado, os recursos antifalsificação não serão permitidos. Se definido como Não Configurado, o usuário poderá escolher se deseja usar antifalsificação. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|securityKeyForSignIn|[Capacitação](../resources/intune-shared-enablement.md)|A chave de segurança para Entrar fornece a capacidade de ativar/desativar remotamente Windows Hello keyl de sercurity não configurado respeitará as configurações feitas no clinet. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|atribuições|Conjunto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo Herdado de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|

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
  "roleScopeTagIds": [
    "String"
  ],
  "deviceEnrollmentConfigurationType": "String",
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
  "enhancedBiometricsState": "String",
  "securityKeyForSignIn": "String"
}
```




