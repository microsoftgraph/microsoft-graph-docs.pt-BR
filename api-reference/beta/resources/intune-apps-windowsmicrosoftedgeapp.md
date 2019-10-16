---
title: tipo de recurso windowsMicrosoftEdgeApp
description: Contém propriedades e propriedades herdadas do aplicativo Microsoft Edge no Windows.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 447d25d95ca97673b0d735547fa2823022089190
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538522"
---
# <a name="windowsmicrosoftedgeapp-resource-type"></a>tipo de recurso windowsMicrosoftEdgeApp

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades e propriedades herdadas do aplicativo Microsoft Edge no Windows.


Herda de [mobileApp](../resources/intune-shared-mobileapp.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsMicrosoftEdgeApps](../api/intune-apps-windowsmicrosoftedgeapp-list.md)|coleção [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md)|Listar Propriedades e relações dos objetos [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) .|
|[Obter windowsMicrosoftEdgeApp](../api/intune-apps-windowsmicrosoftedgeapp-get.md)|[windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md)|Leia as propriedades e as relações do objeto [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) .|
|[Criar windowsMicrosoftEdgeApp](../api/intune-apps-windowsmicrosoftedgeapp-create.md)|[windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md)|Criar um novo objeto [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) .|
|[Excluir windowsMicrosoftEdgeApp](../api/intune-apps-windowsmicrosoftedgeapp-delete.md)|Nenhum|Exclui [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md).|
|[Atualizar windowsMicrosoftEdgeApp](../api/intune-apps-windowsmicrosoftedgeapp-update.md)|[windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md)|Atualiza as propriedades de um objeto [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|displayName|Cadeia de caracteres|O título do aplicativo importado ou definido pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|description|Cadeia de caracteres|A descrição do aplicativo. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|publicador|Cadeia de caracteres|O publicador do aplicativo. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|createdDateTime|DateTimeOffset|A data e a hora da criação do aplicativo. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora que o aplicativo foi modificado pela última vez. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|isFeatured|Boolean|O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|privacyInformationUrl|Cadeia de caracteres|A URL da declaração de privacidade. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|informationUrl|Cadeia de caracteres|A URL de informações adicionais. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|owner|Cadeia de caracteres|O proprietário do conteúdo. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|developer|Cadeia de caracteres|O desenvolvedor do aplicativo. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|notes|String|Anotações do aplicativo. Herdada de [mobileApp](../resources/intune-shared-mobileapp.md)|
|uploadState|Int32|O estado de upload. Herdada de [mobileApp](../resources/intune-shared-mobileapp.md)|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|O estado de publicação do aplicativo. O aplicativo não pode ser assinado, a menos que ele seja publicado. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md). Os valores possíveis são: `notPublished`, `processing`, `published`.|
|isAssigned|Boolean|O valor que indica se o aplicativo é atribuído a pelo menos um grupo. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|roleScopeTagIds|String collection|Lista de IDs de marca de escopo para este aplicativo móvel. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|dependentAppCount|Int32|O número total de dependências do aplicativo filho. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)|
|canal|[microsoftEdgeChannel](../resources/intune-apps-microsoftedgechannel.md)|O canal a ser instalado nos dispositivos de destino. Os valores possíveis são: `dev`, `beta`, `stable`.|

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
  "@odata.type": "microsoft.graph.windowsMicrosoftEdgeApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMicrosoftEdgeApp",
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
  "channel": "String"
}
```



