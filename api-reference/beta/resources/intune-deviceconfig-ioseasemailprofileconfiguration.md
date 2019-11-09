---
title: tipo de recurso iosEasEmailProfileConfiguration
description: Ao fornecer configurações neste perfil, você pode instruir o cliente de email nativo em dispositivos iOS para se comunicar com um servidor Exchange e obter email, contatos, calendário, lembretes e anotações. Além disso, você também pode especificar o volume de emails a ser sincronizado e a frequência em que o dispositivo deve ser sincronizado.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 17f56ac8860b93b046381a017a91894eea07e21c
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38078299"
---
# <a name="ioseasemailprofileconfiguration-resource-type"></a>tipo de recurso iosEasEmailProfileConfiguration

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ao fornecer configurações neste perfil, você pode instruir o cliente de email nativo em dispositivos iOS para se comunicar com um servidor Exchange e obter email, contatos, calendário, lembretes e anotações. Além disso, você também pode especificar o volume de emails a ser sincronizado e a frequência em que o dispositivo deve ser sincronizado.


Herda de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar iosEasEmailProfileConfigurations](../api/intune-deviceconfig-ioseasemailprofileconfiguration-list.md)|coleção [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)|Listar Propriedades e relações dos objetos [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .|
|[Obter iosEasEmailProfileConfiguration](../api/intune-deviceconfig-ioseasemailprofileconfiguration-get.md)|[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)|Leia as propriedades e as relações do objeto [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .|
|[Criar iosEasEmailProfileConfiguration](../api/intune-deviceconfig-ioseasemailprofileconfiguration-create.md)|[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)|Criar um novo objeto [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .|
|[Excluir iosEasEmailProfileConfiguration](../api/intune-deviceconfig-ioseasemailprofileconfiguration-delete.md)|Nenhum|Exclui [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).|
|[Atualizar iosEasEmailProfileConfiguration](../api/intune-deviceconfig-ioseasemailprofileconfiguration-update.md)|[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)|Atualiza as propriedades de um objeto [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|Coleção String|Lista de marcas de escopo para esta instância de entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Booliano|Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para essa política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para essa política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|descrição|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|usernameSource|[UserEmail](../resources/intune-deviceconfig-useremailsource.md)|Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo. Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md). Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.|
|usernameAADSource|[usernameSource](../resources/intune-deviceconfig-usernamesource.md)|Nome do campo AAD, que será usado para recuperar o nome de usuário para o perfil de email. Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md). Os valores possíveis são: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.|
|userDomainNameSource|[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)|Atributo UserDomainName que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo. Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md). Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.|
|customDomainName|String|Valor de nome de domínio personalizado usado durante a geração de um perfil de email antes da instalação no dispositivo. Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)|
|accountName|String|Nome da conta.|
|authenticationMethod|[easAuthenticationMethod](../resources/intune-deviceconfig-easauthenticationmethod.md)|Método de autenticação para este perfil de email. Os valores possíveis são: `usernameAndPassword`, `certificate`, `derivedCredential`.|
|blockMovingMessagesToOtherEmailAccounts|Booliano|Indica se as mensagens de movimentação devem ou não ser bloqueadas para outras contas de email.|
|blockSendingEmailFromThirdPartyApps|Booliano|Indica se o envio de emails de aplicativos de terceiros deve ou não ser bloqueado.|
|blockSyncingRecentlyUsedEmailAddresses|Booliano|Indica se a sincronização de endereços de email usados recentemente deve ou não ser bloqueada, por exemplo, ao compor novos emails.|
|durationOfEmailToSync|[emailSyncDuration](../resources/intune-deviceconfig-emailsyncduration.md)|Duração de tempo que o email deve ser sincronizado de volta para o. . Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.|
|emailAddresse|[UserEmail](../resources/intune-deviceconfig-useremailsource.md)|Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo. Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.|
|easServices|[easServices](../resources/intune-deviceconfig-easservices.md)|Trocar dados a serem sincronizados. Os valores possíveis são `none`: `calendars`, `contacts`, `email`, `notes`, `reminders`,.|
|easServicesUserOverrideEnabled|Booliano|Permitir que os usuários alterem as configurações de sincronização.|
|hostName|Cadeia de caracteres|Local do Exchange que (URL) ao qual o aplicativo de email nativo se conecta.|
|requireSmime|Booliano|Indica se o certificado S/MIME deve ou não ser usado.|
|smimeEnablePerMessageSwitch|Booliano|Indica se os emails não criptografados devem ou não ser permitidos.|
|smimeEncryptByDefaultEnabled|Booliano|Se definido como true a criptografia S/MIME estiver habilitada por padrão.|
|smimeSigningEnabled|Booliano|Se definido como true a assinatura S/MIME estiver habilitada para essa conta|
|smimeSigningUserOverrideEnabled|Booliano|Se definido como true, o usuário pode ativar ou desativar a assinatura S/MIME.|
|smimeEncryptByDefaultUserOverrideEnabled|Booliano|Se definido como true, o usuário pode ativar a opção criptografia por padrão.|
|smimeSigningCertificateUserOverrideEnabled|Booliano|Se definido como true, o usuário pode selecionar a identidade de assinatura.|
|smimeEncryptionCertificateUserOverrideEnabled|Booliano|Se definido como true, o usuário pode selecionar a identidade de criptografia S/MIME. |
|requireSsl|Booliano|Indica se o SSL deve ou não ser usado.|
|useOAuth|Booliano|Especifica se a conexão deve usar o OAuth para autenticação.|
|signingCertificateType|[emailCertificateType](../resources/intune-deviceconfig-emailcertificatetype.md)|Assinatura tipo de certificado para este perfil de email. Os valores possíveis são: `none`, `certificate`, `derivedCredential`.|
|encryptionCertificateType|[emailCertificateType](../resources/intune-deviceconfig-emailcertificatetype.md)|Tipo de certificado de criptografia para este perfil de email. Os valores possíveis são: `none`, `certificate`, `derivedCredential`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status da instalação da configuração de dispositivo por dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status de instalação da configuração do dispositivo por usuário. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status de dispositivos para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status de usuários para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Visão geral de dispositivos de configuração para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|identityCertificate|[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)|Certificado de identidade.|
|smimeSigningCertificate|[iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md)|Certificado de assinatura S/MIME.|
|smimeEncryptionCertificate|[iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md)|Certificado de criptografia S/MIME.|
|derivedCredentialSettings|[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|Configurações de nível de locatário para as credenciais derivadas a serem usadas para autenticação.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosEasEmailProfileConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosEasEmailProfileConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "usernameSource": "String",
  "usernameAADSource": "String",
  "userDomainNameSource": "String",
  "customDomainName": "String",
  "accountName": "String",
  "authenticationMethod": "String",
  "blockMovingMessagesToOtherEmailAccounts": true,
  "blockSendingEmailFromThirdPartyApps": true,
  "blockSyncingRecentlyUsedEmailAddresses": true,
  "durationOfEmailToSync": "String",
  "emailAddressSource": "String",
  "easServices": "String",
  "easServicesUserOverrideEnabled": true,
  "hostName": "String",
  "requireSmime": true,
  "smimeEnablePerMessageSwitch": true,
  "smimeEncryptByDefaultEnabled": true,
  "smimeSigningEnabled": true,
  "smimeSigningUserOverrideEnabled": true,
  "smimeEncryptByDefaultUserOverrideEnabled": true,
  "smimeSigningCertificateUserOverrideEnabled": true,
  "smimeEncryptionCertificateUserOverrideEnabled": true,
  "requireSsl": true,
  "useOAuth": true,
  "signingCertificateType": "String",
  "encryptionCertificateType": "String"
}
```



