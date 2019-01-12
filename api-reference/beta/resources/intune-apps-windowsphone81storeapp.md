---
title: tipo de recurso de windowsPhone81StoreApp
description: Contém propriedades e as propriedades herdadas para aplicativos do Windows Phone 8.1 repositório.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3abdf94b66698d2f58b5c7c3143f3f0345d7ce4f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961117"
---
# <a name="windowsphone81storeapp-resource-type"></a>tipo de recurso de windowsPhone81StoreApp

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Contém propriedades e as propriedades herdadas para aplicativos do Windows Phone 8.1 repositório.

Herda de [mobileApp](../resources/intune-apps-mobileapp.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista windowsPhone81StoreApps](../api/intune-apps-windowsphone81storeapp-list.md)|coleção [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md)|Lista as propriedades e os relacionamentos dos objetos [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) .|
|[Obter windowsPhone81StoreApp](../api/intune-apps-windowsphone81storeapp-get.md)|[windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md)|Leia as propriedades e os relacionamentos do objeto [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) .|
|[Criar windowsPhone81StoreApp](../api/intune-apps-windowsphone81storeapp-create.md)|[windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md)|Crie um novo objeto de [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) .|
|[Excluir windowsPhone81StoreApp](../api/intune-apps-windowsphone81storeapp-delete.md)|Nenhum|Exclui um [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md).|
|[Atualizar windowsPhone81StoreApp](../api/intune-apps-windowsphone81storeapp-update.md)|[windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md)|Atualize as propriedades de um objeto [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) .|

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
|appStoreUrl|Cadeia de caracteres|A URL do repositório do Windows Phone 8.1 app.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|categories|Coleção [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|A lista de categorias para este aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|assignments|Coleção [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|A lista de atribuições de grupo para esse aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Resumo de instalação do aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|deviceStatuses|coleção [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|A lista de estados de instalação para esse aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|userStatuses|coleção [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|A lista de estados de instalação para esse aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsPhone81StoreApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPhone81StoreApp",
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
  "appStoreUrl": "String"
}
```





