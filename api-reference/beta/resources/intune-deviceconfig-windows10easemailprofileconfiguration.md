---
title: tipo de recurso de windows10EasEmailProfileConfiguration
description: Fornecendo configurações neste perfil, você poderá instruir o cliente de email nativo (Outlook) em dispositivos Windows 10 para se comunicar com um servidor Exchange e obter email, calendário, contatos e tarefas. Além disso, você também pode especificar o quanto email para sincronização e com que frequência o dispositivo deve sincronizar.
localization_priority: Normal
ms.openlocfilehash: be74fa183836c271f9a86b299c03c05972eccf0c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816664"
---
# <a name="windows10easemailprofileconfiguration-resource-type"></a>tipo de recurso de windows10EasEmailProfileConfiguration

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Fornecendo configurações neste perfil, você poderá instruir o cliente de email nativo (Outlook) em dispositivos Windows 10 para se comunicar com um servidor Exchange e obter email, calendário, contatos e tarefas. Além disso, você também pode especificar o quanto email para sincronização e com que frequência o dispositivo deve sincronizar.

Herda de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista windows10EasEmailProfileConfigurations](../api/intune-deviceconfig-windows10easemailprofileconfiguration-list.md)|coleção [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)|Lista as propriedades e os relacionamentos dos objetos [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) .|
|[Obter windows10EasEmailProfileConfiguration](../api/intune-deviceconfig-windows10easemailprofileconfiguration-get.md)|[windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)|Leia as propriedades e os relacionamentos do objeto [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) .|
|[Criar windows10EasEmailProfileConfiguration](../api/intune-deviceconfig-windows10easemailprofileconfiguration-create.md)|[windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)|Crie um novo objeto de [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) .|
|[Excluir windows10EasEmailProfileConfiguration](../api/intune-deviceconfig-windows10easemailprofileconfiguration-delete.md)|Nenhum|Exclui um [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md).|
|[Atualizar windows10EasEmailProfileConfiguration](../api/intune-deviceconfig-windows10easemailprofileconfiguration-update.md)|[windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)|Atualize as propriedades de um objeto [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) .|

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
|usernameSource|[userEmailSource](../resources/intune-deviceconfig-useremailsource.md)|Atributo de nome de usuário que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo. Herdada do [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md). Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.|
|usernameAADSource|[usernameSource](../resources/intune-deviceconfig-usernamesource.md)|Nome do campo AAD, que será usado para recuperar o nome de usuário para o perfil de email. Herdada do [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md). Os valores possíveis são: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.|
|userDomainNameSource|[domainNameSource](../resources/intune-deviceconfig-domainnamesource.md)|Atributo nome_do_domínio que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo. Herdada do [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md). Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.|
|customDomainName|Cadeia de caracteres|Valor de nome de domínio personalizado usado ao gerar um perfil de email antes de instalar no dispositivo. Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)|
|accountName|Cadeia de caracteres|Nome da conta.|
|syncCalendar|Booliano|Se deseja ou não sincronizar o calendário.|
|syncContacts|Booliano|Se deseja ou não sincronizar contatos.|
|syncTasks|Booliano|Se deseja ou não sincronizar tarefas.|
|durationOfEmailToSync|[emailSyncDuration](../resources/intune-deviceconfig-emailsyncduration.md)|Duração de email para sincronizar. Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.|
|emailAddressSource|[userEmailSource](../resources/intune-deviceconfig-useremailsource.md)|Atributo de email que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo. Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.|
|emailSyncSchedule|[emailSyncSchedule](../resources/intune-deviceconfig-emailsyncschedule.md)|Agenda de sincronização de email. Os valores possíveis são: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.|
|hostName|Cadeia de caracteres|Local do Exchange que (URL) que o aplicativo de email nativo se conecta ao.|
|requireSsl|Booliano|Indica se deve ou não usar SSL.|

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
  "@odata.type": "microsoft.graph.windows10EasEmailProfileConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
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
  "usernameSource": "String",
  "usernameAADSource": "String",
  "userDomainNameSource": "String",
  "customDomainName": "String",
  "accountName": "String",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "durationOfEmailToSync": "String",
  "emailAddressSource": "String",
  "emailSyncSchedule": "String",
  "hostName": "String",
  "requireSsl": true
}
```





