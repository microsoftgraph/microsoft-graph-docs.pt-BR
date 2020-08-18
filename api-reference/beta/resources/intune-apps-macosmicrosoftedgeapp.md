---
title: tipo de recurso macOSMicrosoftEdgeApp
description: Contém propriedades e propriedades herdadas para o aplicativo MacOS Microsoft Edge.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b13783ba95f5ddd3f7d9e225fef8bda52395c122
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792398"
---
# <a name="macosmicrosoftedgeapp-resource-type"></a>tipo de recurso macOSMicrosoftEdgeApp

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades e propriedades herdadas para o aplicativo MacOS Microsoft Edge.


Herda de [mobileApp](../resources/intune-shared-mobileapp.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar macOSMicrosoftEdgeApps](../api/intune-apps-macosmicrosoftedgeapp-list.md)|coleção [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md)|Listar Propriedades e relações dos objetos [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) .|
|[Obter macOSMicrosoftEdgeApp](../api/intune-apps-macosmicrosoftedgeapp-get.md)|[macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md)|Leia as propriedades e as relações do objeto [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) .|
|[Criar macOSMicrosoftEdgeApp](../api/intune-apps-macosmicrosoftedgeapp-create.md)|[macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md)|Criar um novo objeto [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) .|
|[Excluir macOSMicrosoftEdgeApp](../api/intune-apps-macosmicrosoftedgeapp-delete.md)|Nenhum|Exclui [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md).|
|[Atualizar macOSMicrosoftEdgeApp](../api/intune-apps-macosmicrosoftedgeapp-update.md)|[macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md)|Atualiza as propriedades de um objeto [macOSMicrosoftEdgeApp](../resources/intune-apps-macosmicrosoftedgeapp.md) .|

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
|channel|[microsoftEdgeChannel](../resources/intune-apps-microsoftedgechannel.md)|O canal a ser instalado nos dispositivos de destino. Os valores possíveis são: `dev`, `beta`, `stable`.|

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
  "@odata.type": "microsoft.graph.macOSMicrosoftEdgeApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSMicrosoftEdgeApp",
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



