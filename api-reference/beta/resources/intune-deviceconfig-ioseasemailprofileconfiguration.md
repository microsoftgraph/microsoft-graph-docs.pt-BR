---
title: Tipo de recurso iosEasEmailProfileConfiguration
description: Ao fornecer configurações neste perfil, você pode instruir o cliente de email nativo em dispositivos iOS a se comunicar com um servidor Exchange e receber emails, contatos, calendário, lembretes e anotações. Além disso, você também pode especificar quanto email sincronizar e com que frequência o dispositivo deve sincronizar.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 341ef1dbf790cfe4ac1398dd7a49488d0fc31399
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58771110"
---
# <a name="ioseasemailprofileconfiguration-resource-type"></a>Tipo de recurso iosEasEmailProfileConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ao fornecer configurações neste perfil, você pode instruir o cliente de email nativo em dispositivos iOS a se comunicar com um servidor Exchange e receber emails, contatos, calendário, lembretes e anotações. Além disso, você também pode especificar quanto email sincronizar e com que frequência o dispositivo deve sincronizar.


Herda de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar iosEasEmailProfileConfigurations](../api/intune-deviceconfig-ioseasemailprofileconfiguration-list.md)|[Coleção iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)|Listar propriedades e relações dos [objetos iosEasEmailProfileConfiguration.](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)|
|[Obter iosEasEmailProfileConfiguration](../api/intune-deviceconfig-ioseasemailprofileconfiguration-get.md)|[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)|Leia propriedades e relações do [objeto iosEasEmailProfileConfiguration.](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)|
|[Criar iosEasEmailProfileConfiguration](../api/intune-deviceconfig-ioseasemailprofileconfiguration-create.md)|[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)|Crie um novo [objeto iosEasEmailProfileConfiguration.](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)|
|[Excluir iosEasEmailProfileConfiguration](../api/intune-deviceconfig-ioseasemailprofileconfiguration-delete.md)|Nenhum(a)|Exclui um [iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md).|
|[Atualizar iosEasEmailProfileConfiguration](../api/intune-deviceconfig-ioseasemailprofileconfiguration-update.md)|[iosEasEmailProfileConfiguration](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)|Atualize as propriedades de [um objeto iosEasEmailProfileConfiguration.](../resources/intune-deviceconfig-ioseasemailprofileconfiguration.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância entity. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Boleano|Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|descrição|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|usernameSource|[userEmailSource](../resources/intune-deviceconfig-useremailsource.md)|Atributo username que é escolhido no AAD e injetado nesse perfil antes de instalar no dispositivo. Herdado [do easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md). Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.|
|usernameAADSource|[usernameSource](../resources/intune-deviceconfig-usernamesource.md)|Nome do campo AAD, que será usado para recuperar UserName para perfil de email. Herdado [do easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md). Os valores possíveis são: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.|
|userDomainNameSource|[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)|Atributo UserDomainname que é escolhido no AAD e injetado nesse perfil antes de instalar no dispositivo. Herdado [do easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md). Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.|
|customDomainName|Cadeia de caracteres|Valor de nome de domínio personalizado usado durante a geração de um perfil de email antes de instalar no dispositivo. Herdado [do easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)|
|accountName|Cadeia de caracteres|Nome da conta.|
|authenticationMethod|[easAuthenticationMethod](../resources/intune-deviceconfig-easauthenticationmethod.md)|Método de autenticação para este perfil de email. Os valores possíveis são: `usernameAndPassword`, `certificate`, `derivedCredential`.|
|blockMovingMessagesToOtherEmailAccounts|Boleano|Indica se deve ou não bloquear a movimentação de mensagens para outras contas de email.|
|blockSendingEmailFromThirdPartyApps|Boleano|Indica se o envio de emails de aplicativos de terceiros deve ou não ser bloqueado.|
|blockSyncingRecentlyUsedEmailAddresses|Boleano|Indica se deve ou não bloquear a sincronização de endereços de email usados recentemente, por exemplo, ao compor novos emails.|
|durationOfEmailToSync|[emailSyncDuration](../resources/intune-deviceconfig-emailsyncduration.md)|A duração do tempo em que o email deve ser sincronizado novamente. . Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.|
|emailAddressSource|[userEmailSource](../resources/intune-deviceconfig-useremailsource.md)|Atributo de email que é escolhido no AAD e injetado nesse perfil antes de instalar no dispositivo. Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.|
|easServices|[easServices](../resources/intune-deviceconfig-easservices.md)|Exchange dados a sincronizar. Os valores possíveis `none` são: `calendars` , , , , , `contacts` `email` `notes` `reminders` .|
|easServicesUserOverrideEnabled|Boleano|Permitir que os usuários alterem as configurações de sincronização.|
|hostName|Cadeia de caracteres|Exchange local que (URL) ao que o aplicativo de email nativo se conecta.|
|requireSmime|Boleano|Indica se o certificado S/MIME deve ou não ser usado.|
|smimeEnablePerMessageSwitch|Boleano|Indica se os emails não criptografados permitirão ou não.|
|smimeEncryptByDefaultEnabled|Boleano|Se definido como criptografia S/MIME verdadeiro estiver habilitado por padrão.|
|smimeSigningEnabled|Boleano|Se definido como a assinatura S/MIME verdadeira estiver habilitada para essa conta|
|smimeSigningUserOverrideEnabled|Boleano|Se for definido como true, o usuário poderá alternar a sessão S/MIME para 1 ou 2016.|
|smimeEncryptByDefaultUserOverrideEnabled|Booliano|Se definido como true, o usuário pode alternar a criptografia por configuração padrão.|
|smimeSigningCertificateUserOverrideEnabled|Boleano|Se for definido como true, o usuário poderá selecionar a identidade de assinatura.|
|smimeEncryptionCertificateUserOverrideEnabled|Boleano|Se definido como true, o usuário poderá selecionar a identidade de criptografia S/MIME. |
|requireSsl|Boleano|Indica se o SSL deve ou não ser usado.|
|useOAuth|Boleano|Especifica se a conexão deve usar OAuth para autenticação.|
|signingCertificateType|[emailCertificateType](../resources/intune-deviceconfig-emailcertificatetype.md)|Tipo de certificado de assinatura para este perfil de email. Os valores possíveis são: `none`, `certificate`, `derivedCredential`.|
|encryptionCertificateType|[emailCertificateType](../resources/intune-deviceconfig-emailcertificatetype.md)|Tipo de certificado de criptografia para este perfil de email. Os valores possíveis são: `none`, `certificate`, `derivedCredential`.|
|perAppVPNProfileId|Cadeia de caracteres|ID de perfil da política Per-App VPN a ser usada para acessar emails do cliente de Email nativo|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|[Coleção deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status da instalação da configuração de dispositivo por dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status da instalação de configuração do dispositivo pelo usuário. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status de dispositivos para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status de usuários para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Visão geral de dispositivos de configuração para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|identityCertificate|[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)|Certificado de identidade.|
|smimeSigningCertificate|[iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md)|Certificado de assinatura S/MIME.|
|smimeEncryptionCertificate|[iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md)|Certificado de criptografia S/MIME.|
|derivedCredentialSettings|[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|Configurações de nível de locatário para as Credenciais Derivadas a serem usadas para autenticação.|

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
  "encryptionCertificateType": "String",
  "perAppVPNProfileId": "String"
}
```



