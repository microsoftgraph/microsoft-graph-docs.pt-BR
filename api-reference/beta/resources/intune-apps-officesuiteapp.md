---
title: tipo de recurso officeSuiteApp
description: Contém propriedades e propriedades herdadas para o aplicativo do pacote do office365.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b2af74f6c917004a254e5f3b33d9d6f3b7fafea9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005097"
---
# <a name="officesuiteapp-resource-type"></a>tipo de recurso officeSuiteApp

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades e propriedades herdadas para o aplicativo do pacote do office365.


Herda de [mobileApp](../resources/intune-apps-mobileapp.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar officeSuiteApps](../api/intune-apps-officesuiteapp-list.md)|coleção [officeSuiteApp](../resources/intune-apps-officesuiteapp.md)|Listar Propriedades e relações dos objetos [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .|
|[Obter officeSuiteApp](../api/intune-apps-officesuiteapp-get.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)|Leia as propriedades e as relações do objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .|
|[Criar officeSuiteApp](../api/intune-apps-officesuiteapp-create.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)|Criar um novo objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .|
|[Excluir officeSuiteApp](../api/intune-apps-officesuiteapp-delete.md)|Nenhum|Exclui [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).|
|[Atualizar officeSuiteApp](../api/intune-apps-officesuiteapp-update.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)|Atualiza as propriedades de um objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|displayName|String|O título do aplicativo importado ou definido pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|descrição|String|A descrição do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|publicador|String|O publicador do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|createdDateTime|DateTimeOffset|A data e a hora da criação do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora que o aplicativo foi modificado pela última vez. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|isFeatured|Boolean|O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|privacyInformationUrl|String|A URL da declaração de privacidade. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|informationUrl|String|A URL de informações adicionais. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|owner|String|O proprietário do conteúdo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|developer|String|O desenvolvedor do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|notes|String|Anotações do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|uploadState|Int32|O estado de upload. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|O estado de publicação do aplicativo. O aplicativo não pode ser assinado, a menos que ele seja publicado. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md). Os valores possíveis são: `notPublished`, `processing`, `published`.|
|isAssigned|Boolean|O valor que indica se o aplicativo é atribuído a pelo menos um grupo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de IDs de marca de escopo para este aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|dependentAppCount|Int32|O número total de dependências do aplicativo filho. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|autoAcceptEula|Booliano|O valor para aceitar o EULA automaticamente no dispositivo do usuário.|
|productIds|coleção [officeProductId](../resources/intune-apps-officeproductid.md)|As IDs de produto que representam a SKU do pacote do office365.|
|excludedApps|[excludedApps](../resources/intune-apps-excludedapps.md)|A propriedade para representar os aplicativos que são excluídos da ID de produto do Office365 selecionado.|
|Propriedades usesharedcomputeractivation|Booliano|A propriedade que representa se a ativação de computador compartilhado é usada não para o pacote de aplicativos do office365.|
|updateChannel|[officeUpdateChannel](../resources/intune-apps-officeupdatechannel.md)|A propriedade para representar o canal de atualização do office365. Os valores possíveis são: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.|
|officePlatformArchitecture|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|A propriedade para representar a versão do pacote de aplicativos do office365. Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.|
|localesToInstall|Coleção de cadeias de caracteres|A propriedade para representar os locais que são instalados quando os aplicativos do Office365 estão instalados. Ele usa RFC 6033 padrão. Refhttps://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx|
|installProgressDisplayLevel|[officeSuiteInstallProgressDisplayLevel](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|Para especificar o nível de exibição da interface do usuário da configuração de progresso da instalação no dispositivo. Os valores possíveis são: `none` e `full`.|
|shouldUninstallOlderVersionsOfOffice|Booliano|A propriedade para determinar se deve desinstalar o Office MSI existente se um pacote de aplicativos do Office365 for implantado no dispositivo ou não.|
|targetVersion|String|A propriedade para representar a versão de destino específica para o pacote de aplicativos do Office365 que deve permanecer implantado nos dispositivos.|
|updateVersion|String|A propriedade para representar a versão de atualização na qual a versão de destino específica está disponível para o pacote de aplicativos do office365.|
|officeConfigurationXml|Binária|A propriedade para representar o arquivo de configuração XML que pode ser especificado para aplicativos do Office ProPlus. Tem precedência sobre todas as outras propriedades. Quando presente, o arquivo de configuração XML será usado para criar o aplicativo.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|categories|Coleção [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|A lista de categorias para este aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|assignments|Coleção [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|A lista de atribuições de grupo para esse aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Resumo de instalação do aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|deviceStatuses|coleção [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|A lista de Estados de instalação para este aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|userStatuses|coleção [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|A lista de Estados de instalação para este aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|relações|coleção [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|Lista de relações para este aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeSuiteApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeSuiteApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "uploadState": 1024,
  "publishingState": "String",
  "isAssigned": true,
  "roleScopeTagIds": [
    "String"
  ],
  "dependentAppCount": 1024,
  "autoAcceptEula": true,
  "productIds": [
    "String"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "excel": true,
    "groove": true,
    "infoPath": true,
    "lync": true,
    "oneDrive": true,
    "oneNote": true,
    "outlook": true,
    "powerPoint": true,
    "publisher": true,
    "sharePointDesigner": true,
    "teams": true,
    "visio": true,
    "word": true
  },
  "useSharedComputerActivation": true,
  "updateChannel": "String",
  "officePlatformArchitecture": "String",
  "localesToInstall": [
    "String"
  ],
  "installProgressDisplayLevel": "String",
  "shouldUninstallOlderVersionsOfOffice": true,
  "targetVersion": "String",
  "updateVersion": "String",
  "officeConfigurationXml": "binary"
}
```





