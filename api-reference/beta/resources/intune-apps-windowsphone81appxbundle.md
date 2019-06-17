---
title: tipo de recurso windowsPhone81AppXBundle
description: Contém propriedades e propriedades herdadas para a linha de aplicativos comerciais de pacote do Windows Phone 8,1 AppX.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5222b3a9886920991755c9c72908f257037d240e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34975683"
---
# <a name="windowsphone81appxbundle-resource-type"></a>tipo de recurso windowsPhone81AppXBundle

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades e propriedades herdadas para a linha de aplicativos comerciais de pacote do Windows Phone 8,1 AppX.


Herda de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsPhone81AppXBundles](../api/intune-apps-windowsphone81appxbundle-list.md)|coleção [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)|Listar Propriedades e relações dos objetos [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .|
|[Obter windowsPhone81AppXBundle](../api/intune-apps-windowsphone81appxbundle-get.md)|[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)|Leia as propriedades e as relações do objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .|
|[Criar windowsPhone81AppXBundle](../api/intune-apps-windowsphone81appxbundle-create.md)|[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)|Criar um novo objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .|
|[Excluir windowsPhone81AppXBundle](../api/intune-apps-windowsphone81appxbundle-delete.md)|Nenhum|Exclui [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).|
|[Atualizar windowsPhone81AppXBundle](../api/intune-apps-windowsphone81appxbundle-update.md)|[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)|Atualiza as propriedades de um objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .|

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
|committedContentVersion|String|A versão do conteúdo interno confirmado. Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|fileName|String|O nome do arquivo do aplicativo Lob principal. Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|size|Int64|O tamanho total, incluindo todos os arquivos carregados. Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|applicableArchitectures|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|As arquiteturas do Windows nas quais este aplicativo pode ser executado. Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md). Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.|
|identityName|String|O Nome da Identidade. Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)|
|identityPublisherHash|String|O Hash do Publicador de Identidade. Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)|
|identityResourceIdentifier|String|O Identificador de Recurso da Identidade. Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)|
|minimumSupportedOperatingSystem|[windowsMinimumOperatingSystem](../resources/intune-apps-windowsminimumoperatingsystem.md)|O valor do sistema de operacional mínimo aplicável. Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)|
|phoneProductIdentifier|String|O identificador do produto de telefone. Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)|
|phonePublisherId|String|A ID do editor do telefone. herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)|
|identityVersion|String|A versão da identidade. Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)|
|appXPackageInformationList|coleção [windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md)|A lista de informações do pacote AppX.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|categories|Coleção [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|A lista de categorias para este aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|assignments|Coleção [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|A lista de atribuições de grupo para esse aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Resumo de instalação do aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|deviceStatuses|coleção [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|A lista de Estados de instalação para este aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|userStatuses|coleção [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|A lista de Estados de instalação para este aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|relações|coleção [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|Lista de relações para este aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|contentVersions|Coleção [mobileAppContent](../resources/intune-apps-mobileappcontent.md)|A lista das versões de conteúdo deste aplicativo. Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsPhone81AppXBundle"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
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
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "applicableArchitectures": "String",
  "identityName": "String",
  "identityPublisherHash": "String",
  "identityResourceIdentifier": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "phoneProductIdentifier": "String",
  "phonePublisherId": "String",
  "identityVersion": "String",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "String",
      "displayName": "String",
      "identityName": "String",
      "identityPublisher": "String",
      "identityResourceIdentifier": "String",
      "identityVersion": "String",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true,
        "v10_1809": true,
        "v10_1903": true
      }
    }
  ]
}
```





