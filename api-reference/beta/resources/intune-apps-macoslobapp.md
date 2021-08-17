---
title: Tipo de recurso macOSLobApp
description: Contém propriedades e propriedades herdadas para o Aplicativo LOB do MacOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fd11ce13e39d2c2caf9ee3a910186c7fd9d3e5d00310a9dcd05ecf48931f5ffc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54131294"
---
# <a name="macoslobapp-resource-type"></a>Tipo de recurso macOSLobApp

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades e propriedades herdadas para o Aplicativo LOB do MacOS.


Herda de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar macOSLobApps](../api/intune-apps-macoslobapp-list.md)|[Coleção macOSLobApp](../resources/intune-apps-macoslobapp.md)|Listar propriedades e relações dos [objetos macOSLobApp.](../resources/intune-apps-macoslobapp.md)|
|[Obter macOSLobApp](../api/intune-apps-macoslobapp-get.md)|[macOSLobApp](../resources/intune-apps-macoslobapp.md)|Leia propriedades e relações do [objeto macOSLobApp.](../resources/intune-apps-macoslobapp.md)|
|[Criar macOSLobApp](../api/intune-apps-macoslobapp-create.md)|[macOSLobApp](../resources/intune-apps-macoslobapp.md)|Crie um novo [objeto macOSLobApp.](../resources/intune-apps-macoslobapp.md)|
|[Excluir macOSLobApp](../api/intune-apps-macoslobapp-delete.md)|Nenhum|Exclui um [macOSLobApp](../resources/intune-apps-macoslobapp.md).|
|[Atualizar macOSLobApp](../api/intune-apps-macoslobapp-update.md)|[macOSLobApp](../resources/intune-apps-macoslobapp.md)|Atualize as propriedades de um [objeto macOSLobApp.](../resources/intune-apps-macoslobapp.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|displayName|Cadeia de caracteres|O título do aplicativo importado ou definido pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|description|Cadeia de caracteres|A descrição do aplicativo. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
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
|roleScopeTagIds|String collection|Lista de ids de marca de escopo para este aplicativo móvel. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|dependentAppCount|Int32|O número total de dependências que o aplicativo filho tem. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|supersedingAppCount|Int32|O número total de aplicativos que esse aplicativo sobressede direta ou indiretamente. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|supersededAppCount|Int32|O número total de aplicativos pelos quais esse aplicativo é, direta ou indiretamente, é suplido. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|committedContentVersion|String|A versão do conteúdo interno confirmado. Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|fileName|String|O nome do arquivo do aplicativo Lob principal. Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|size|Int64|O tamanho total, incluindo todos os arquivos carregados. Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|bundleId|String|A ID do pacote.|
|minimumSupportedOperatingSystem|[macOSMinimumOperatingSystem](../resources/intune-apps-macosminimumoperatingsystem.md)|O valor do sistema de operacional mínimo aplicável.|
|buildNumber|String|O número de composição do aplicativo MacOS Line of Business (LoB).|
|versionNumber|String|O número de versão do aplicativo MacOS Line of Business (LoB).|
|childApps|[Coleção macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md)|A lista de aplicativos neste pacote de pacotes|
|identityVersion|String|A versão da identidade.|
|md5HashChunkSize|Int32|O tamanho da parte do hash MD5|
|md5Hash|String collection|Os códigos de hash MD5|
|ignoreVersionDetection|Boolean|Um booliano para controlar se a versão do aplicativo será usada para detectar o aplicativo depois que ele for instalado em um dispositivo. Defina isso como true para aplicativos macOS Line of Business (LoB) que usam um recurso de atualização automática.|
|installAsManaged|Boolean|Um booleano para controlar se o aplicativo será instalado como gerenciado (exige macOS 11.0 e outras restrições de PKG).|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|categories|Coleção [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|A lista de categorias para este aplicativo. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|assignments|Coleção [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|A lista de atribuições de grupo para esse aplicativo móvel. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Resumo de instalação do aplicativo móvel. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|deviceStatuses|[Coleção mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|A lista de estados de instalação para este aplicativo móvel. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|userStatuses|[Coleção userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|A lista de estados de instalação para este aplicativo móvel. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|relações|[Coleção mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|O conjunto de relações diretas para este aplicativo. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|contentVersions|Coleção [mobileAppContent](../resources/intune-apps-mobileappcontent.md)|A lista das versões de conteúdo deste aplicativo. Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSLobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLobApp",
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
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "bundleId": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true,
    "v10_14": true,
    "v10_15": true,
    "v11_0": true
  },
  "buildNumber": "String",
  "versionNumber": "String",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "String",
      "buildNumber": "String",
      "versionNumber": "String"
    }
  ],
  "identityVersion": "String",
  "md5HashChunkSize": 1024,
  "md5Hash": [
    "String"
  ],
  "ignoreVersionDetection": true,
  "installAsManaged": true
}
```




