---
title: tipo de recurso androidEasEmailProfileConfiguration
description: Ao fornecer configurações neste perfil, você pode instruir o cliente de email nativo nos dispositivos do KNOX para se comunicar com um servidor do Exchange e obter email, contatos, calendário, tarefas e anotações. Além disso, você também pode especificar o volume de emails a ser sincronizado e a frequência em que o dispositivo deve ser sincronizado.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 497a629ee500bc522e0ab2c0eb6b7b530983b956
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175196"
---
# <a name="androideasemailprofileconfiguration-resource-type"></a>tipo de recurso androidEasEmailProfileConfiguration

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ao fornecer configurações neste perfil, você pode instruir o cliente de email nativo nos dispositivos do KNOX para se comunicar com um servidor do Exchange e obter email, contatos, calendário, tarefas e anotações. Além disso, você também pode especificar o volume de emails a ser sincronizado e a frequência em que o dispositivo deve ser sincronizado.


Herda de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar androidEasEmailProfileConfigurations](../api/intune-deviceconfig-androideasemailprofileconfiguration-list.md)|coleção [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)|Listar Propriedades e relações dos objetos [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .|
|[Obter androidEasEmailProfileConfiguration](../api/intune-deviceconfig-androideasemailprofileconfiguration-get.md)|[androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)|Leia as propriedades e as relações do objeto [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .|
|[Criar androidEasEmailProfileConfiguration](../api/intune-deviceconfig-androideasemailprofileconfiguration-create.md)|[androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)|Criar um novo objeto [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .|
|[Excluir androidEasEmailProfileConfiguration](../api/intune-deviceconfig-androideasemailprofileconfiguration-delete.md)|Nenhum|Exclui [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md).|
|[Atualizar androidEasEmailProfileConfiguration](../api/intune-deviceconfig-androideasemailprofileconfiguration-update.md)|[androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)|Atualiza as propriedades de um objeto [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância de entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Booliano|Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure. Esta propriedade é somente leitura. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|accountName|String|Nome da conta do Exchange ActiveSync, exibido para os usuários como o nome do perfil EAS (este).|
|authenticationMethod|[easAuthenticationMethod](../resources/intune-deviceconfig-easauthenticationmethod.md)|Método de autenticação para o Exchange ActiveSync. Os valores possíveis são: `usernameAndPassword` e `certificate`.|
|syncCalendar|Booliano|Alterna a sincronização do calendário. Se definido como falso, o calendário será desativado no dispositivo.|
|syncContacts|Booliano|Alterna a sincronização de contatos. Se definido como falso, os contatos serão desativados no dispositivo.|
|syncTasks|Booliano|Alterna a sincronização de tarefas. Se definido como falso, as tarefas serão desativadas no dispositivo.|
|syncNotes|Booliano|Alterna a sincronização das anotações. Se definido como false, as anotações serão desativadas no dispositivo.|
|durationOfEmailToSync|[emailSyncDuration](../resources/intune-deviceconfig-emailsyncduration.md)|Duração de tempo que o email deve ser sincronizado. Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.|
|emailAddresse|[userEmail](../resources/intune-deviceconfig-useremailsource.md)|Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo. Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.|
|emailSyncSchedule|[emailSyncSchedule](../resources/intune-deviceconfig-emailsyncschedule.md)|Agenda de sincronização de email. Os valores possíveis são: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.|
|hostName|Cadeia de caracteres|Local do Exchange (URL) ao qual o aplicativo de email nativo se conecta.|
|requireSmime|Booliano|Indica se o certificado S/MIME deve ou não ser usado.|
|requireSsl|Booliano|Indica se o SSL deve ou não ser usado.|
|usernameSource|[androidUsernameSource](../resources/intune-deviceconfig-androidusernamesource.md)|Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo. Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.|
|userDomainNameSource|[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)|Atributo userDomainname que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo. Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.|
|customDomainName|String|Valor de nome de domínio personalizado usado durante a geração de um perfil de email antes da instalação no dispositivo.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status de instalação da configuração do dispositivo por dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status de instalação da configuração do dispositivo por usuário. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status dos dispositivos na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status dos usuários na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Resumo de dispositivo de estado de configuração do dispositivo Herdada do [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|identityCertificate|[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)|Certificado de identidade.|
|smimeSigningCertificate|[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)|Certificado de assinatura S/MIME.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidEasEmailProfileConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
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
  "accountName": "String",
  "authenticationMethod": "String",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "syncNotes": true,
  "durationOfEmailToSync": "String",
  "emailAddressSource": "String",
  "emailSyncSchedule": "String",
  "hostName": "String",
  "requireSmime": true,
  "requireSsl": true,
  "usernameSource": "String",
  "userDomainNameSource": "String",
  "customDomainName": "String"
}
```




