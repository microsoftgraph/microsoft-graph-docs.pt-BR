---
title: Tipo de recurso officeSuiteApp
description: Contém propriedades e propriedades herdadas para o Aplicativo do Office365 Suite.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 905dd84366253b8f346efd42118711a118c61580
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58815166"
---
# <a name="officesuiteapp-resource-type"></a>Tipo de recurso officeSuiteApp

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades e propriedades herdadas para o Aplicativo do Office365 Suite.


Herda de [mobileApp](../resources/intune-shared-mobileapp.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar officeSuiteApps](../api/intune-apps-officesuiteapp-list.md)|[Coleção officeSuiteApp](../resources/intune-apps-officesuiteapp.md)|Listar propriedades e relações dos [objetos officeSuiteApp.](../resources/intune-apps-officesuiteapp.md)|
|[Obter officeSuiteApp](../api/intune-apps-officesuiteapp-get.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)|Leia propriedades e relações do [objeto officeSuiteApp.](../resources/intune-apps-officesuiteapp.md)|
|[Criar officeSuiteApp](../api/intune-apps-officesuiteapp-create.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)|Crie um novo [objeto officeSuiteApp.](../resources/intune-apps-officesuiteapp.md)|
|[Excluir officeSuiteApp](../api/intune-apps-officesuiteapp-delete.md)|Nenhum(a)|Exclui um [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).|
|[Atualizar officeSuiteApp](../api/intune-apps-officesuiteapp-update.md)|[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)|Atualize as propriedades de um [objeto officeSuiteApp.](../resources/intune-apps-officesuiteapp.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|displayName|Cadeia de caracteres|O título do aplicativo importado ou definido pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|descrição|Cadeia de caracteres|A descrição do aplicativo. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|publicador|String|O publicador do aplicativo. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|createdDateTime|DateTimeOffset|A data e a hora da criação do aplicativo. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora que o aplicativo foi modificado pela última vez. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|isFeatured|Boolean|O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|privacyInformationUrl|String|A URL da declaração de privacidade. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|informationUrl|String|A URL de informações adicionais. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|owner|Cadeia de caracteres|O proprietário do conteúdo. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|developer|String|O desenvolvedor do aplicativo. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|notes|String|Anotações do aplicativo. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|uploadState|Int32|O estado de carregamento. Os valores possíveis são: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` . Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|O estado de publicação do aplicativo. O aplicativo não pode ser assinado, a menos que ele seja publicado. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md). Os valores possíveis são: `notPublished`, `processing`, `published`.|
|isAssigned|Boolean|O valor que indica se o aplicativo é atribuído a pelo menos um grupo. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de ids de marca de escopo para este aplicativo móvel. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|dependentAppCount|Int32|O número total de dependências que o aplicativo filho tem. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|supersedingAppCount|Int32|O número total de aplicativos que esse aplicativo sobressede direta ou indiretamente. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|supersededAppCount|Int32|O número total de aplicativos pelos quais esse aplicativo é, direta ou indiretamente, é suplido. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|autoAcceptEula|Boleano|O valor para aceitar o EULA automaticamente no dispositivo do usuário final.|
|productIds|[Coleção officeProductId](../resources/intune-apps-officeproductid.md)|As IDs de produto que representam a SKU do Office365 Suite.|
|excludedApps|[excludedApps](../resources/intune-apps-excludedapps.md)|A propriedade para representar os aplicativos excluídos da ID do Produto do Office365 selecionada.|
|useSharedComputerActivation|Boleano|A propriedade para representar se a ativação do computador compartilhado é usada não para o pacote de aplicativos do Office365.|
|updateChannel|[officeUpdateChannel](../resources/intune-apps-officeupdatechannel.md)|A propriedade para representar o Canal de Atualização do Office365. Os possíveis valores são: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`, `monthlyEnterprise`.|
|officePlatformArchitecture|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|A propriedade para representar a versão do pacote de aplicativos do Office365. Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.|
|localesToInstall|Coleção de cadeias de caracteres|A propriedade para representar as localidades que são instaladas quando os aplicativos do Office365 são instalados. Ele usa o RFC 6033 padrão. Ref: https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx|
|installProgressDisplayLevel|[officeSuiteInstallProgressDisplayLevel](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|Para especificar o nível de exibição para a interface do usuário de instalação de progresso da instalação no Dispositivo. Os valores possíveis são: `none` e `full`.|
|shouldUninstallOlderVersionsOfOffice|Boleano|A propriedade para determinar se deve desinstalar o MSI existente Office se um pacote de aplicativos do Office365 for implantado no dispositivo ou não.|
|targetVersion|Cadeia de caracteres|A propriedade para representar a versão de destino específica do pacote de aplicativos do Office365 que deve ser implantada nos dispositivos.|
|updateVersion|Cadeia de caracteres|A propriedade para representar a versão de atualização na qual a versão de destino específica está disponível para o pacote de aplicativos do Office365.|
|officeConfigurationXml|Binário|A propriedade para representar o arquivo de configuração XML que pode ser especificado para Office ProPlus Apps. Tem precedência sobre todas as outras propriedades. Quando presente, o arquivo de configuração XML será usado para criar o aplicativo.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|categories|Coleção [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|A lista de categorias para este aplicativo. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|assignments|Coleção [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|A lista de atribuições de grupo para esse aplicativo móvel. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Resumo de instalação do aplicativo móvel. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|deviceStatuses|[Coleção mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|A lista de estados de instalação para este aplicativo móvel. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|userStatuses|[Coleção userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|A lista de estados de instalação para este aplicativo móvel. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|relações|[Coleção mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|O conjunto de relações diretas para este aplicativo. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|

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
  "supersedingAppCount": 1024,
  "supersededAppCount": 1024,
  "autoAcceptEula": true,
  "productIds": [
    "String"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "bing": true,
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



