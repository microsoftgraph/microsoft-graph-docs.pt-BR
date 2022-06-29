---
title: Tipo de recurso mobileApp
description: Uma classe abstrata que contém as propriedades base de aplicativos móveis do Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dbccfb27073c15e6a5fbf78842cc894aadea2c1c
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441115"
---
# <a name="mobileapp-resource-type"></a>Tipo de recurso mobileApp

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe abstrata que contém as propriedades base de aplicativos móveis do Intune.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mobileApps](../api/intune-shared-mobileapp-list.md)|Coleção [mobileApp](../resources/intune-shared-mobileapp.md)|Lista propriedades e relações dos objetos [mobileApp](../resources/intune-shared-mobileapp.md).|
|[Obter mobileApp](../api/intune-shared-mobileapp-get.md)|[mobileApp](../resources/intune-shared-mobileapp.md)|Propriedades de leitura e relações do objeto [mobileApp](../resources/intune-shared-mobileapp.md).|
|**Aplicativos**|
|[atribuir ação](../api/intune-shared-mobileapp-assign.md)|Nenhuma|Ainda não documentado|
|[Função getMobileAppCount](../api/intune-shared-mobileapp-getmobileappcount.md)|Int64|Ainda não documentado|
|[Função getTopMobileApps](../api/intune-shared-mobileapp-gettopmobileapps.md)|Coleção [mobileApp](../resources/intune-shared-mobileapp.md)|Ainda não documentado|
|[Ação updateRelationships](../api/intune-shared-mobileapp-updaterelationships.md)|Nenhuma|Ainda não documentado|
|[Função getRelatedAppStates](../api/intune-shared-mobileapp-getrelatedappstates.md)|[coleção mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md)|Ainda não documentado|
|**Conjunto de Políticas**|
|[Ação hasPayloadLinks](../api/intune-shared-mobileapp-haspayloadlinks.md)|[coleção hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|displayName|Cadeia de caracteres|O título do aplicativo importado ou definido pelo administrador.|
|descrição|String|A descrição do aplicativo.|
|publisher|String|O publicador do aplicativo.|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.|
|createdDateTime|DateTimeOffset|A data e a hora da criação do aplicativo.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora que o aplicativo foi modificado pela última vez.|
|isFeatured|Booliano|O valor que indica se o aplicativo está marcado como em destaque pelo administrador.|
|privacyInformationUrl|String|A URL da declaração de privacidade.|
|informationUrl|String|A URL de informações adicionais.|
|owner|String|O proprietário do conteúdo.|
|developer|String|O desenvolvedor do aplicativo.|
|notes|String|Anotações do aplicativo.|
|uploadState|Int32|O estado de carregamento.|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|O estado de publicação do aplicativo. O aplicativo não pode ser assinado, a menos que ele seja publicado. Os valores possíveis são: `notPublished`, `processing`, `published`.|
|isAssigned|Boolean|O valor que indica se o aplicativo é atribuído a pelo menos um grupo.|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de IDs de marca de escopo para este aplicativo móvel.|
|dependentAppCount|Int32|O número total de dependências que o aplicativo filho tem.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|**Aplicativos**|
|categories|Coleção [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|A lista de categorias para este aplicativo.|
|assignments|Coleção [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|A lista de atribuições de grupo para esse aplicativo móvel.|
|installSummary|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)|Resumo de instalação do aplicativo móvel.|
|deviceStatuses|[Coleção mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|A lista de estados de instalação para este aplicativo móvel.|
|userStatuses|[coleção userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|A lista de estados de instalação para este aplicativo móvel.|
|Relações|[coleção mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|Lista de relações para este aplicativo móvel.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileApp",
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
  "dependentAppCount": 1024
}
```



