---
title: tipo de recurso androidManagedStoreWebApp
description: Contém propriedades e propriedades herdadas para aplicativos Web configurados para serem distribuídos por meio do repositório de aplicativos Android gerenciado.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 91eff55615fb8cad22c02b023968f54fdec8e295
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791306"
---
# <a name="androidmanagedstorewebapp-resource-type"></a>tipo de recurso androidManagedStoreWebApp

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades e propriedades herdadas para aplicativos Web configurados para serem distribuídos por meio do repositório de aplicativos Android gerenciado.


Herda de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar androidManagedStoreWebApps](../api/intune-apps-androidmanagedstorewebapp-list.md)|coleção [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)|Listar Propriedades e relações dos objetos [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) .|
|[Obter androidManagedStoreWebApp](../api/intune-apps-androidmanagedstorewebapp-get.md)|[androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)|Leia as propriedades e as relações do objeto [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) .|
|[Criar androidManagedStoreWebApp](../api/intune-apps-androidmanagedstorewebapp-create.md)|[androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)|Criar um novo objeto [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) .|
|[Excluir androidManagedStoreWebApp](../api/intune-apps-androidmanagedstorewebapp-delete.md)|Nenhum|Exclui [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md).|
|[Atualizar androidManagedStoreWebApp](../api/intune-apps-androidmanagedstorewebapp-update.md)|[androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md)|Atualiza as propriedades de um objeto [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|displayName|String|O título do aplicativo importado ou definido pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|description|String|A descrição do aplicativo. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|publicador|String|O publicador do aplicativo. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|createdDateTime|DateTimeOffset|A data e a hora da criação do aplicativo. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora que o aplicativo foi modificado pela última vez. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|isFeatured|Boolean|O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|privacyInformationUrl|String|A URL da declaração de privacidade. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|informationUrl|String|A URL de informações adicionais. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|owner|String|O proprietário do conteúdo. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|developer|String|O desenvolvedor do aplicativo. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|notes|String|Anotações do aplicativo. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|uploadState|Int32|O estado de upload. Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` . Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|O estado de publicação do aplicativo. O aplicativo não pode ser assinado, a menos que ele seja publicado. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md). Os valores possíveis são: `notPublished`, `processing`, `published`.|
|isAssigned|Boolean|O valor que indica se o aplicativo é atribuído a pelo menos um grupo. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|roleScopeTagIds|Coleção de cadeia de caracteres|Lista de IDs de marca de escopo para este aplicativo móvel. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|dependentAppCount|Int32|O número total de dependências do aplicativo filho. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|packageId|String|O identificador do pacote. Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|appIdentifier|String|O Nome da Identidade. Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|usedLicenseCount|Int32|O número de aplicativos VPP em uso. Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|totalLicenseCount|Int32|O número total de licenças VPP. Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|appStoreUrl|String|A URL do aplicativo de reproduzir para o repositório de trabalho. Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|IsPrivate|Booliano|Indica se o aplicativo está disponível somente para os usuários de uma empresa. Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|isSystemApp|Booliano|Indica se o aplicativo é um aplicativo de sistema pré-instalado. Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|appTracks|coleção [androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md)|As faixas que são visíveis para esta empresa. Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|
|supportsOemConfig|Booliano|Se este aplicativo dá suporte à política OEMConfig. Herdado de [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|categories|Coleção [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|A lista de categorias para este aplicativo. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|assignments|Coleção [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|A lista de atribuições de grupo para esse aplicativo móvel. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Resumo de instalação do aplicativo móvel. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|deviceStatuses|coleção [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|A lista de Estados de instalação para este aplicativo móvel. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|userStatuses|coleção [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|A lista de Estados de instalação para este aplicativo móvel. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|relações|coleção [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|Lista de relações para este aplicativo móvel. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|

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



