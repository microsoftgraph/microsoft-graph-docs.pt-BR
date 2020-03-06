---
title: Tipo de recurso iosLobApp
description: Contém propriedades e propriedades herdadas para aplicativos de linha de negócios iOS.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fabfdde6b8cc8660ab4880c35c5989cda57e3681
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532843"
---
# <a name="ioslobapp-resource-type"></a>Tipo de recurso iosLobApp

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades e propriedades herdadas para aplicativos de linha de negócios iOS.


Herda de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar iosLobApps](../api/intune-apps-ioslobapp-list.md)|Coleção [iosLobApp](../resources/intune-apps-ioslobapp.md)|Lista propriedades e relações dos objetos [iosLobApp](../resources/intune-apps-ioslobapp.md).|
|[Obter iosLobApp](../api/intune-apps-ioslobapp-get.md)|[iosLobApp](../resources/intune-apps-ioslobapp.md)|Propriedades de leitura e relações do objeto [iosLobApp](../resources/intune-apps-ioslobapp.md).|
|[Criar iosLobApp](../api/intune-apps-ioslobapp-create.md)|[iosLobApp](../resources/intune-apps-ioslobapp.md)|Cria um novo objeto [iosLobApp](../resources/intune-apps-ioslobapp.md).|
|[Excluir iosLobApp](../api/intune-apps-ioslobapp-delete.md)|Nenhum|Exclui um [iosLobApp](../resources/intune-apps-ioslobapp.md).|
|[Atualizar iosLobApp](../api/intune-apps-ioslobapp-update.md)|[iosLobApp](../resources/intune-apps-ioslobapp.md)|Atualiza as propriedades de um objeto [iosLobApp](../resources/intune-apps-ioslobapp.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|displayName|Cadeia de caracteres|O título do aplicativo importado ou definido pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|description|String|A descrição do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|publicador|String|O publicador do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|createdDateTime|DateTimeOffset|A data e a hora da criação do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora que o aplicativo foi modificado pela última vez. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|isFeatured|Boolean|O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|privacyInformationUrl|String|A URL da declaração de privacidade. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|informationUrl|String|A URL de informações adicionais. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|owner|String|O proprietário do conteúdo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|developer|String|O desenvolvedor do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|notes|String|Anotações do aplicativo. Herdada de [mobileApp](../resources/intune-apps-mobileapp.md)|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|O estado de publicação do aplicativo. O aplicativo não pode ser assinado, a menos que ele seja publicado. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md). Os valores possíveis são: `notPublished`, `processing`, `published`.|
|committedContentVersion|String|A versão do conteúdo interno confirmado. Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|fileName|String|O nome do arquivo do aplicativo Lob principal. Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|size|Int64|O tamanho total, incluindo todos os arquivos carregados. Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|
|bundleId|String|O Nome da Identidade.|
|applicableDeviceType|[iosDeviceType](../resources/intune-apps-iosdevicetype.md)|A arquitetura do iOS na qual esse aplicativo pode ser executado.|
|minimumSupportedOperatingSystem|[iosMinimumOperatingSystem](../resources/intune-apps-iosminimumoperatingsystem.md)|O valor do sistema de operacional mínimo aplicável.|
|expirationDateTime|DateTimeOffset|O tempo de expiração.|
|versionNumber|String|O número de versão do aplicativo de Linha de Negócios (LoB) iOS.|
|buildNumber|Cadeia de caracteres|O número de build do aplicativo de Linha de Negócios (LoB) iOS.|

## <a name="relationships"></a>Relacionamento
|Relação|Tipo|Descrição|
|:---|:---|:---|
|categories|Coleção [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|A lista de categorias para este aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|assignments|Coleção [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|A lista de atribuições de grupo para esse aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|contentVersions|Coleção [mobileAppContent](../resources/intune-apps-mobileappcontent.md)|A lista das versões de conteúdo deste aplicativo. Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosLobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobApp",
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
  "publishingState": "String",
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "bundleId": "String",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true
  },
  "expirationDateTime": "String (timestamp)",
  "versionNumber": "String",
  "buildNumber": "String"
}
```




