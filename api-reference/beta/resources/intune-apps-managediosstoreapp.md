---
title: managedIOSStoreApp resource type
description: Contém propriedades e propriedades herdadas para aplicativo da loja iOS que você pode gerenciar com uma política de proteção de aplicativos do Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 11b712aa07acecc0abaf018e0b0ba0aeaca42413
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66667443"
---
# <a name="managediosstoreapp-resource-type"></a>managedIOSStoreApp resource type

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades e propriedades herdadas para aplicativo da loja iOS que você pode gerenciar com uma política de proteção de aplicativos do Intune.


Herda de [managedApp](../resources/intune-apps-managedapp.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedIOSStoreApps](../api/intune-apps-managediosstoreapp-list.md)|Coleção [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md)|Lista propriedades e relações dos objetos [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).|
|[Obter managedIOSStoreApp](../api/intune-apps-managediosstoreapp-get.md)|[managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md)|Propriedades de leitura e relações do objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).|
|[Criar managedIOSStoreApp](../api/intune-apps-managediosstoreapp-create.md)|[managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md)|Cria um novo objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).|
|[Excluir managedIOSStoreApp](../api/intune-apps-managediosstoreapp-delete.md)|Nenhum|Exclui um [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).|
|[Atualizar managedIOSStoreApp](../api/intune-apps-managediosstoreapp-update.md)|[managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md)|Atualiza as propriedades de um objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|displayName|String|O título do aplicativo importado ou definido pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|descrição|String|A descrição do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
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
|appAvailability|[managedAppAvailability](../resources/intune-apps-managedappavailability.md)|A disponibilidade do Aplicativo. Herdado de [managedApp](../resources/intune-apps-managedapp.md). Os valores possíveis são: `global`, `lineOfBusiness`.|
|version|String|A versão do Aplicativo. Herdado de [managedApp](../resources/intune-apps-managedapp.md)|
|bundleId|Cadeia de caracteres|A ID do pacote de aplicativos.|
|appStoreUrl|Cadeia de caracteres|A AppStoreUrl da Apple.|
|applicableDeviceType|[iosDeviceType](../resources/intune-apps-iosdevicetype.md)|A arquitetura do iOS na qual esse aplicativo pode ser executado.|
|minimumSupportedOperatingSystem|[iosMinimumOperatingSystem](../resources/intune-apps-iosminimumoperatingsystem.md)|O valor do sistema de operacional mínimo com suporte.|

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
  "@odata.type": "microsoft.graph.managedIOSStoreApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
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
  "appAvailability": "String",
  "version": "String",
  "bundleId": "String",
  "appStoreUrl": "String",
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
    "v13_0": true,
    "v14_0": true,
    "v15_0": true
  }
}
```




