---
title: Tipo de recurso androidManagedStoreWebApp
description: Contém propriedades e propriedades herdadas para aplicativos Web configurados para serem distribuídos por meio da loja de aplicativos Android gerenciada.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 75729e972cd08b9c61d9992e7c46dfe2d99200e5
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66669361"
---
# <a name="androidmanagedstorewebapp-resource-type"></a>Tipo de recurso androidManagedStoreWebApp

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades e propriedades herdadas para aplicativos Web configurados para serem distribuídos por meio da loja de aplicativos Android gerenciada.


Herda de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar androidManagedStoreWebApps](../api/intune-apps-androidmanagedstorewebapp-list.md)|[coleção androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)|Listar propriedades e relações dos objetos [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) .|
|[Obter androidManagedStoreWebApp](../api/intune-apps-androidmanagedstorewebapp-get.md)|[androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)|Ler propriedades e relações do objeto [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) .|
|[Criar androidManagedStoreWebApp](../api/intune-apps-androidmanagedstorewebapp-create.md)|[androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)|Crie um novo [objeto androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) .|
|[Excluir androidManagedStoreWebApp](../api/intune-apps-androidmanagedstorewebapp-delete.md)|Nenhum|Exclui um [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md).|
|[Atualizar androidManagedStoreWebApp](../api/intune-apps-androidmanagedstorewebapp-update.md)|[androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)|Atualize as propriedades de um [objeto androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|displayName|Cadeia de caracteres|O título do aplicativo importado ou definido pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|descrição|Cadeia de caracteres|A descrição do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|publicador|String|O publicador do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|createdDateTime|DateTimeOffset|A data e a hora da criação do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora que o aplicativo foi modificado pela última vez. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|isFeatured|Boolean|O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|privacyInformationUrl|String|A URL da declaração de privacidade. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|informationUrl|String|A URL de informações adicionais. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|owner|Cadeia de caracteres|O proprietário do conteúdo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|developer|String|O desenvolvedor do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|notes|String|Anotações do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|uploadState|Int32|O estado de carregamento. Os valores possíveis são: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|O estado de publicação do aplicativo. O aplicativo não pode ser assinado, a menos que ele seja publicado. Herdado do [mobileApp](../resources/intune-apps-mobileapp.md). Os valores possíveis são: `notPublished`, `processing`, `published`.|
|isAssigned|Boolean|O valor que indica se o aplicativo é atribuído a pelo menos um grupo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|roleScopeTagIds|Conjunto de cadeias de caracteres|Lista de IDs de marca de escopo para este aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|dependentAppCount|Int32|O número total de dependências que o aplicativo filho tem. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|supersedingAppCount|Int32|O número total de aplicativos que esse aplicativo substitui direta ou indiretamente. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|supersededAppCount|Int32|O número total de aplicativos que esse aplicativo é substituído direta ou indiretamente. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|packageId|String|O identificador do pacote. Herdado [de androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|appIdentifier|String|O Nome da Identidade. Herdado [de androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|usedLicenseCount|Int32|O número de aplicativos VPP em uso. Herdado [de androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|totalLicenseCount|Int32|O número total de licenças VPP. Herdado [de androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|appStoreUrl|String|A URL do aplicativo Play for Work Store. Herdado [de androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|Isprivate|Boolean|Indica se o aplicativo só está disponível para os usuários de uma determinada empresa. Herdado [de androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|isSystemApp|Booliano|Indica se o aplicativo é um aplicativo do sistema pré-instalado. Herdado [de androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|appTracks|[coleção androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md)|As faixas visíveis para essa empresa. Herdado [de androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|supportsOemConfig|Booliano|Se esse aplicativo dá suporte à política OEMConfig. Herdado [de androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|categories|Coleção [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|A lista de categorias para este aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|assignments|Coleção [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|A lista de atribuições de grupo para esse aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Resumo de instalação do aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|deviceStatuses|[Coleção mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|A lista de estados de instalação para este aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|userStatuses|[coleção userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|A lista de estados de instalação para este aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|Relações|[coleção mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|O conjunto de relações diretas para este aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedStoreWebApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreWebApp",
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
  "packageId": "String",
  "appIdentifier": "String",
  "usedLicenseCount": 1024,
  "totalLicenseCount": 1024,
  "appStoreUrl": "String",
  "isPrivate": true,
  "isSystemApp": true,
  "appTracks": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppTrack",
      "trackId": "String",
      "trackAlias": "String"
    }
  ],
  "supportsOemConfig": true
}
```




