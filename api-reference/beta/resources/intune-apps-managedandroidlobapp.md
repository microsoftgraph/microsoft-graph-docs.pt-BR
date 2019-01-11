---
title: managedAndroidLobApp resource type
description: Contém propriedades e propriedades herdadas para aplicativos de linha de negócios Android gerenciados.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c19928b0bde339962bb00fc3e8f81845e00011dc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822754"
---
# <a name="managedandroidlobapp-resource-type"></a>managedAndroidLobApp resource type

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Contém propriedades e propriedades herdadas para aplicativos de linha de negócios Android gerenciados.

Herda de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedAndroidLobApps](../api/intune-apps-managedandroidlobapp-list.md)|Coleção [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)|Lista propriedades e relações dos objetos [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).|
|[Obter managedAndroidLobApp](../api/intune-apps-managedandroidlobapp-get.md)|[managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)|Propriedades de leitura e relações do objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).|
|[Criar managedAndroidLobApp](../api/intune-apps-managedandroidlobapp-create.md)|[managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)|Cria um novo objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).|
|[Excluir managedAndroidLobApp](../api/intune-apps-managedandroidlobapp-delete.md)|Nenhum|Exclui um [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).|
|[Atualizar managedAndroidLobApp](../api/intune-apps-managedandroidlobapp-update.md)|[managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md)|Atualiza as propriedades de um objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|displayName|Cadeia de caracteres|O título do aplicativo importado ou definido pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|description|Cadeia de caracteres|A descrição do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|publisher|Cadeia de caracteres|O publicador do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|createdDateTime|DateTimeOffset|A data e a hora da criação do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora que o aplicativo foi modificado pela última vez. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|isFeatured|Booliano|O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|privacyInformationUrl|Cadeia de caracteres|A URL da declaração de privacidade. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|informationUrl|Cadeia de caracteres|A URL de informações adicionais. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|owner|Cadeia de caracteres|O proprietário do conteúdo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|developer|Cadeia de caracteres|O desenvolvedor do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|Observações|Cadeia de caracteres|Anotações para o aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|uploadState|Int32|O estado de carregamento. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|O estado de publicação para o aplicativo. O aplicativo não pode ser assinado, a menos que ele seja publicado. Herdada do [mobileApp](../resources/intune-apps-mobileapp.md). Os valores possíveis são: `notPublished`, `processing`, `published`.|
|appAvailability|[managedAppAvailability](../resources/intune-apps-managedappavailability.md)|A disponibilidade do Aplicativo. Herdada do [managedApp](../resources/intune-apps-managedapp.md). Os valores possíveis são: `global`, `lineOfBusiness`.|
|version|Cadeia de caracteres|A versão do Aplicativo. Herdado de [managedApp](../resources/intune-apps-managedapp.md)|
|committedContentVersion|Cadeia de caracteres|A versão do conteúdo interno confirmado. Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)|
|fileName|Cadeia de caracteres|O nome do arquivo do aplicativo Lob principal. Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)|
|size|Int64|O tamanho total, incluindo todos os arquivos carregados. Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)|
|packageId|Cadeia de caracteres|O identificador do pacote.|
|identityName|Cadeia de caracteres|O Nome da Identidade.|
|minimumSupportedOperatingSystem|[androidMinimumOperatingSystem](../resources/intune-apps-androidminimumoperatingsystem.md)|O valor do sistema de operacional mínimo aplicável.|
|versionName|Cadeia de caracteres|O nome da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.|
|versionCode|Cadeia de caracteres|O código da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.|
|identityVersion|Cadeia de caracteres|A versão da identidade.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|categories|Coleção [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|A lista de categorias para este aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|assignments|Coleção [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|A lista de atribuições de grupo para esse aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Resumo de instalação do aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|deviceStatuses|coleção [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|A lista de estados de instalação para esse aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|userStatuses|coleção [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|A lista de estados de instalação para esse aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|contentVersions|Coleção [mobileAppContent](../resources/intune-apps-mobileappcontent.md)|A lista das versões de conteúdo deste aplicativo. Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAndroidLobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "appAvailability": "String",
  "version": "String",
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "packageId": "String",
  "identityName": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "String",
  "versionCode": "String",
  "identityVersion": "String"
}
```





