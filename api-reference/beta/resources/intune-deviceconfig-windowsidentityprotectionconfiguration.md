---
title: tipo de recurso de windowsIdentityProtectionConfiguration
description: Esta entidade fornece descrições dos declarado métodos, propriedades e os relacionamentos expostos pelo Windows Olá for Business.
localization_priority: Normal
ms.openlocfilehash: c83a87737db6deacf7a08cc0fb4a73aff6d4f781
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823398"
---
# <a name="windowsidentityprotectionconfiguration-resource-type"></a>tipo de recurso de windowsIdentityProtectionConfiguration

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Esta entidade fornece descrições dos declarado métodos, propriedades e os relacionamentos expostos pelo Windows Olá for Business.

Herda de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista windowsIdentityProtectionConfigurations](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-list.md)|coleção [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|Lista as propriedades e os relacionamentos dos objetos [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .|
|[Obter windowsIdentityProtectionConfiguration](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-get.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|Leia as propriedades e os relacionamentos do objeto [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .|
|[Criar windowsIdentityProtectionConfiguration](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-create.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|Crie um novo objeto de [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .|
|[Excluir windowsIdentityProtectionConfiguration](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-delete.md)|Nenhum|Exclui um [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md).|
|[Atualizar windowsIdentityProtectionConfiguration](../api/intune-deviceconfig-windowsidentityprotectionconfiguration-update.md)|[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)|Atualize as propriedades de um objeto [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|String collection|Lista de escopo marcas para essa instância da entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Booliano|Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo. Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure. Esta propriedade é somente leitura. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|enhancedAntiSpoofingForFacialFeaturesEnabled|Booliano|Valor booleano usado para habilitar avançada antifalsificação para reconhecimento de recurso faciais na autenticação do Windows Olá face padrão.|
|pinMinimumLength|Int32|Valor inteiro que define o número mínimo de caracteres necessários para o Windows Olá PIN de negócios. Os valores válidos são de 4 a 127 inclusive e menor ou igual ao valor definido para o PIN máximo. Valores válidos 4 a 127|
|pinMaximumLength|Int32|Valor inteiro que define o número máximo de caracteres permitido para o trabalho PIN. Valores válidos são de 4 a 127 inclusive e maior ou igual ao valor definido para o PIN mínimo. Valores válidos 4 a 127|
|pinUppercaseCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Esse valor configura o uso de caracteres maiusculos no Windows Olá PIN de negócios. Os valores possíveis são: `blocked`, `required`, `allowed`.|
|pinLowercaseCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Esse valor configura o uso de caracteres minúsculos no Windows Olá PIN de negócios. Os valores possíveis são: `blocked`, `required`, `allowed`.|
|pinSpecialCharactersUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Controla a capacidade de usar caracteres especiais no Windows Olá PIN de negócios. Os valores possíveis são: `blocked`, `required`, `allowed`.|
|pinExpirationInDays|Int32|Valor inteiro Especifica o período (em dias) que um PIN pode ser usado antes que o sistema exige que o usuário alterá-la. Valores válidos são 0 para 730 inclusive. Valores válidos de 0 a 730|
|pinPreviousBlockCount|Int32|Controla a capacidade de impedir que os usuários utilizem antigas PINs. Isso deve ser definido entre 0 e 50, inclusive, e o PIN atual do usuário está incluído nessa contagem. Se definido como 0, anterior PINs não são armazenadas. Histórico PIN não é preservado por meio de um PIN redefinir. Valores válidos de 0 a 50|
|pinRecoveryEnabled|Booliano|Valor booleano que permite que um usuário alterar seus PINs usando o Windows Hello para o serviço de recuperação de PIN de negócios.|
|securityDeviceRequired|Booliano|Controla se será exigido um Trusted Platform Module (TPM) para provisionamento Windows Olá for Business. Um TPM fornece um benefício de segurança adicionais em que os dados armazenados nela não podem ser usados em outros dispositivos. Se definido como False, todos os dispositivos podem provisionar Windows Olá for Business, mesmo se não houver um TPM utilizável.|
|unlockWithBiometricsEnabled|Booliano|Controla o uso de gestos biométricos, como nominal e a impressão digital, como uma alternativa para o Windows Olá PIN de negócios.  Se definido como False, biométricos gestos não é permitido. Os usuários ainda devem configurar um PIN como um backup em caso de falhas.|
|useCertificatesForOnPremisesAuthEnabled|Booliano|Valor Boolean que permite Windows Olá for Business usar certificados para autenticar os recursos no local.|
|windowsHelloForBusinessBlocked|Booliano|Valor Boolean que bloqueia Windows Olá para negócios como um método para fazer o login no Windows.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status de instalação da configuração do dispositivo por dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status de instalação da configuração de dispositivo por usuário. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status dos dispositivos na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status dos usuários na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Resumo de dispositivo de estado de configuração do dispositivo Herdada do [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsIdentityProtectionConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
  "pinMinimumLength": 1024,
  "pinMaximumLength": 1024,
  "pinUppercaseCharactersUsage": "String",
  "pinLowercaseCharactersUsage": "String",
  "pinSpecialCharactersUsage": "String",
  "pinExpirationInDays": 1024,
  "pinPreviousBlockCount": 1024,
  "pinRecoveryEnabled": true,
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "useCertificatesForOnPremisesAuthEnabled": true,
  "windowsHelloForBusinessBlocked": true
}
```





