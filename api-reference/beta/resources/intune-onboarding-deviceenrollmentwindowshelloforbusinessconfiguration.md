---
title: Tipo de recurso deviceEnrollmentWindowsHelloForBusinessConfiguration
description: As configurações do Windows Hello para empresas permitem que os usuários acessem seus dispositivos usando um gesto, como a autenticação biométrica ou um PIN. Definir configurações para o Windows 10, Windows 10 Mobile e posterior registrados.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f98f590f049f1941ddcc0a721d66e27b6c56f373
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940404"
---
# <a name="deviceenrollmentwindowshelloforbusinessconfiguration-resource-type"></a>Tipo de recurso deviceEnrollmentWindowsHelloForBusinessConfiguration

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

As configurações do Windows Hello para empresas permitem que os usuários acessem seus dispositivos usando um gesto, como a autenticação biométrica ou um PIN. Definir configurações para o Windows 10, Windows 10 Mobile e posterior registrados.


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
|id|Cadeia de caracteres|Identificador exclusivo da conta herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|displayName|String|O nome de exibição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
|description|String|A descrição da configuração de registro do dispositivo herdada de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|
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

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|atribuições|Conjunto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo herdado de [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|

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




