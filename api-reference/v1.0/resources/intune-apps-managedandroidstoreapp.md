---
title: managedAndroidStoreApp resource type
description: Contém propriedades e propriedades herdadas para aplicativos da loja Android que você pode gerenciar com uma política de proteção de aplicativos do Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 368e5dd4837465c51f87a53663ef727c80c2ec62dc574bd1fee591c6227e3051
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141676"
---
# <a name="managedandroidstoreapp-resource-type"></a>managedAndroidStoreApp resource type

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades e propriedades herdadas para aplicativos da loja Android que você pode gerenciar com uma política de proteção de aplicativos do Intune.


Herda de [managedApp](../resources/intune-apps-managedapp.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedAndroidStoreApps](../api/intune-apps-managedandroidstoreapp-list.md)|Coleção [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md)|Lista propriedades e relações dos objetos [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).|
|[Obter managedAndroidStoreApp](../api/intune-apps-managedandroidstoreapp-get.md)|[managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md)|Propriedades de leitura e relações do objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).|
|[Criar managedAndroidStoreApp](../api/intune-apps-managedandroidstoreapp-create.md)|[managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md)|Cria um novo objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).|
|[Excluir managedAndroidStoreApp](../api/intune-apps-managedandroidstoreapp-delete.md)|Nenhum|Exclui um [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).|
|[Atualizar managedAndroidStoreApp](../api/intune-apps-managedandroidstoreapp-update.md)|[managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md)|Atualiza as propriedades de um objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|displayName|Cadeia de caracteres|O título do aplicativo importado ou definido pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|description|String|A descrição do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|publicador|String|O publicador do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|createdDateTime|DateTimeOffset|A data e a hora da criação do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora que o aplicativo foi modificado pela última vez. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|isFeatured|Boolean|O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|privacyInformationUrl|String|A URL da declaração de privacidade. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|informationUrl|String|A URL de informações adicionais. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|proprietário|Cadeia de caracteres|O proprietário do conteúdo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|developer|String|O desenvolvedor do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|notes|String|Anotações do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|O estado de publicação do aplicativo. O aplicativo não pode ser assinado, a menos que ele seja publicado. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md). Os valores possíveis são: `notPublished`, `processing`, `published`.|
|appAvailability|[managedAppAvailability](../resources/intune-apps-managedappavailability.md)|A disponibilidade do Aplicativo. Herdado [de managedApp](../resources/intune-apps-managedapp.md). Os valores possíveis são: `global`, `lineOfBusiness`.|
|version|String|A versão do Aplicativo. Herdado de [managedApp](../resources/intune-apps-managedapp.md)|
|packageId|Cadeia de caracteres|A ID de pacote do aplicativo.|
|appStoreUrl|Cadeia de caracteres|A AppStoreUrl do Android.|
|minimumSupportedOperatingSystem|[androidMinimumOperatingSystem](../resources/intune-apps-androidminimumoperatingsystem.md)|O valor do sistema de operacional mínimo com suporte.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|categories|Coleção [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|A lista de categorias para este aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|assignments|Coleção [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|A lista de atribuições de grupo para esse aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAndroidStoreApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
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
  "appAvailability": "String",
  "version": "String",
  "packageId": "String",
  "appStoreUrl": "String",
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
    "v10_0": true,
    "v11_0": true
  }
}
```




