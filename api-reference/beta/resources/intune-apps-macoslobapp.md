---
title: tipo de recurso de macOSLobApp
description: Contém propriedades e as propriedades herdadas para o aplicativo de LOB MacOS.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f6a9f76cfe32261cb01d286ef0bc0f898d04943a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402843"
---
# <a name="macoslobapp-resource-type"></a>tipo de recurso de macOSLobApp

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Contém propriedades e as propriedades herdadas para o aplicativo de LOB MacOS.


Herda de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista macOSLobApps](../api/intune-apps-macoslobapp-list.md)|coleção [macOSLobApp](../resources/intune-apps-macoslobapp.md)|Lista as propriedades e os relacionamentos dos objetos [macOSLobApp](../resources/intune-apps-macoslobapp.md) .|
|[Obter macOSLobApp](../api/intune-apps-macoslobapp-get.md)|[macOSLobApp](../resources/intune-apps-macoslobapp.md)|Leia as propriedades e os relacionamentos do objeto [macOSLobApp](../resources/intune-apps-macoslobapp.md) .|
|[Criar macOSLobApp](../api/intune-apps-macoslobapp-create.md)|[macOSLobApp](../resources/intune-apps-macoslobapp.md)|Crie um novo objeto de [macOSLobApp](../resources/intune-apps-macoslobapp.md) .|
|[Excluir macOSLobApp](../api/intune-apps-macoslobapp-delete.md)|Nenhum|Exclui um [macOSLobApp](../resources/intune-apps-macoslobapp.md).|
|[Atualizar macOSLobApp](../api/intune-apps-macoslobapp-update.md)|[macOSLobApp](../resources/intune-apps-macoslobapp.md)|Atualize as propriedades de um objeto [macOSLobApp](../resources/intune-apps-macoslobapp.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|displayName|String|O título do aplicativo importado ou definido pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|description|String|A descrição do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|publisher|String|O publicador do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|createdDateTime|DateTimeOffset|A data e a hora da criação do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora que o aplicativo foi modificado pela última vez. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|isFeatured|Boolean|O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|privacyInformationUrl|String|A URL da declaração de privacidade. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|informationUrl|String|A URL de informações adicionais. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|owner|String|O proprietário do conteúdo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|developer|String|O desenvolvedor do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|Observações|String|Anotações para o aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|uploadState|Int32|O estado de carregamento. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|O estado de publicação para o aplicativo. O aplicativo não pode ser assinado, a menos que ele seja publicado. Herdada do [mobileApp](../resources/intune-apps-mobileapp.md). Os valores possíveis são: `notPublished`, `processing`, `published`.|
|isAssigned|Boolean|O valor que indica se o aplicativo é atribuído a pelo menos um grupo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|roleScopeTagIds|String collection|Lista de ids de marca de escopo para esse aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|committedContentVersion|String|A versão do conteúdo interno confirmado. Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|fileName|String|O nome do arquivo do aplicativo Lob principal. Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|size|Int64|O tamanho total, incluindo todos os arquivos carregados. Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|bundleId|String|A id do pacote.|
|minimumSupportedOperatingSystem|[macOSMinimumOperatingSystem](../resources/intune-apps-macosminimumoperatingsystem.md)|O valor do sistema de operacional mínimo aplicável.|
|buildNumber|String|O número de compilação da linha de MacOS do aplicativo de negócios (LoB).|
|versionNumber|String|O número de versão da linha de MacOS do aplicativo de negócios (LoB).|
|childApps|coleção [macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md)|A lista neste pacote do pacote de aplicativo|
|identityVersion|String|A versão da identidade.|
|md5HashChunkSize|Int32|O tamanho do bloco de hash MD5|
|md5Hash|String collection|Os códigos de hash MD5|
|ignoreVersionDetection|Boolean|Um booliano para controlar se a versão do aplicativo será usada para detectar o aplicativo depois que ele for instalado em um dispositivo. Defina essa opção para verdadeiro para macOS aplicativos de linha de negócios (LoB) que usam um recurso de atualização self.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|categories|Coleção [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|A lista de categorias para este aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|assignments|Coleção [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|A lista de atribuições de grupo para esse aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Resumo de instalação do aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|deviceStatuses|coleção [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|A lista de estados de instalação para esse aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|userStatuses|coleção [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|A lista de estados de instalação para esse aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
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
    "v10_13": true
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
  "ignoreVersionDetection": true
}
```




