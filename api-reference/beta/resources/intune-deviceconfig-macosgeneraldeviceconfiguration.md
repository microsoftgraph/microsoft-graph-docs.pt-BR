---
title: Tipo de recurso macOSGeneralDeviceConfiguration
description: Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso macOSGeneralDeviceConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 38e99c1df2f570e06fec22e47e0286eeb4dc76ad
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404789"
---
# <a name="macosgeneraldeviceconfiguration-resource-type"></a>Tipo de recurso macOSGeneralDeviceConfiguration

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso macOSGeneralDeviceConfiguration.


Herda de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar macOSGeneralDeviceConfigurations](../api/intune-deviceconfig-macosgeneraldeviceconfiguration-list.md)|Coleção [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md)|Lista propriedades e relações dos objetos [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).|
|[Obter macOSGeneralDeviceConfiguration](../api/intune-deviceconfig-macosgeneraldeviceconfiguration-get.md)|[macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md)|Propriedades de leitura e relações do objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).|
|[Criar macOSGeneralDeviceConfiguration](../api/intune-deviceconfig-macosgeneraldeviceconfiguration-create.md)|[macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md)|Cria um novo objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).|
|[Excluir macOSGeneralDeviceConfiguration](../api/intune-deviceconfig-macosgeneraldeviceconfiguration-delete.md)|Nenhum|Exclui um [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).|
|[Atualizar macOSGeneralDeviceConfiguration](../api/intune-deviceconfig-macosgeneraldeviceconfiguration-update.md)|[macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md)|Atualiza as propriedades de um objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|String collection|Lista de escopo marcas para essa instância da entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Boolean|Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo. Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure. Esta propriedade é somente leitura. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|compliantAppsList|Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)|Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType). Essa coleção pode conter um máximo de 10.000 elementos.|
|compliantAppListType|[appListType](../resources/intune-deviceconfig-applisttype.md)|Lista que está em CompliantAppsList. Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|emailInDomainSuffixes|String collection|Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.|
|passwordBlockSimple|Boolean|Bloquear senhas simples.|
|passwordExpirationDays|Int32|Número de dias antes da expiração da senha.|
|passwordMinimumCharacterSetCount|Int32|Número de conjuntos de caracteres que uma senha deve conter. Valores válidos de 0 a 4|
|passwordMinimumLength|Int32|Comprimento mínimo das senhas.|
|passwordMinutesOfInactivityBeforeLock|Int32|Minutos de inatividade necessários antes que uma senha seja necessária.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Minutos de inatividade necessários antes que a tela atinja o tempo limite.|
|passwordPreviousPasswordBlockCount|Int32|Número de senhas anteriores para bloquear.|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|Tipo de senha necessário. Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordRequired|Boolean|Se uma senha deve ou não ser exigida.|
|keychainBlockCloudSync|Boolean|Indica se é ou não iCloud sincronização de conjunto de chaves bloqueado (macOS 10.12 e posterior).|
|airPrintBlocked|Boolean|Indica se é ou não AirPrint bloqueados (macOS 10.12 e posterior).|
|airPrintForceTrustedTLS|Boolean|Indica se os certificados confiáveis são necessários para a comunicação de impressão de TLS (macOS 10.13 e posterior).|
|airPrintBlockiBeaconDiscovery|Boolean|Indica se ou não iBeacon descoberta de impressoras AirPrint está bloqueada. Isso impede que os avisos de AirPrint Bluetooth artificiais contra phishing para tráfego de rede (macOS 10.3 e posterior).|
|safariBlockAutofill|Boolean|Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.|
|cameraBlocked|Boolean|Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.|
|iTunesBlockMusicService|Boolean|Indica se ou não bloquear o serviço de música e reverter o aplicativo de música para modo clássico.|
|spotlightBlockInternetResults|Boolean|Indica se deve ou não bloquear destaque retornando todos os resultados de uma pesquisa na Internet.|
|keyboardBlockDictation|Boolean|Indica se deve ou não bloquear o usuário usando a entrada de ditado.|
|definitionLookupBlocked|Boolean|Indica se o bloqueio da pesquisa de definição ou não.|
|appleWatchBlockAutoUnlock|Boolean|Indica se ou aos usuários de bloco de desbloquear sua Mac com Apple Watch.|
|iTunesBlockFileSharing|Boolean|Indica se ou não para bloquear arquivos do que está sendo transferido usando iTunes.|
|iCloudBlockDocumentSync|Boolean|Indica se a sincronização de documentos do iCloud deve ou não ser bloqueada.|
|iCloudBlockMail|Boolean|Indica se deve ou não bloquear iCloud de email está sincronizando.|
|iCloudBlockAddressBook|Boolean|Indica se deve ou não bloquear iCloud da sincronização de contatos.|
|iCloudBlockCalendar|Boolean|Indica se deve ou não bloquear iCloud seja sincronizado calendários.|
|iCloudBlockReminders|Boolean|Indica se deve ou não bloquear iCloud lembretes de sincronização.|
|iCloudBlockBookmarks|Boolean|Indica se deve ou não bloquear iCloud indicadores de sincronização.|
|iCloudBlockNotes|Boolean|Indica se deve ou não bloquear iCloud seja sincronizado anotações.|
|airDropBlocked|Boolean|Indica se deve ou não permitir que AirDrop.|
|passwordBlockModification|Boolean|Indica se deve ou não permitir a modificação de uma senha.|
|passwordBlockFingerprintUnlock|Boolean|Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.|
|passwordBlockAutoFill|Boolean|Indica se deve ou não bloquear o recurso de preenchimento automático de senhas.|
|passwordBlockProximityRequests|Boolean|Indica se deve ou não bloquear solicitantes senhas de dispositivos próximos.|
|passwordBlockAirDropSharing|Boolean|Indica se deve ou não bloquear as senhas de compartilhamento com o recurso de senhas AirDrop.|

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
  "@odata.type": "microsoft.graph.macOSGeneralDeviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
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
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "compliantAppListType": "String",
  "emailInDomainSuffixes": [
    "String"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordRequiredType": "String",
  "passwordRequired": true,
  "keychainBlockCloudSync": true,
  "airPrintBlocked": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "safariBlockAutofill": true,
  "cameraBlocked": true,
  "iTunesBlockMusicService": true,
  "spotlightBlockInternetResults": true,
  "keyboardBlockDictation": true,
  "definitionLookupBlocked": true,
  "appleWatchBlockAutoUnlock": true,
  "iTunesBlockFileSharing": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockMail": true,
  "iCloudBlockAddressBook": true,
  "iCloudBlockCalendar": true,
  "iCloudBlockReminders": true,
  "iCloudBlockBookmarks": true,
  "iCloudBlockNotes": true,
  "airDropBlocked": true,
  "passwordBlockModification": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true
}
```




