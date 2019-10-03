---
title: Tipo de recurso mobileApp
description: Uma classe abstrata que contém as propriedades base de aplicativos móveis do Intune.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 69e1e604fe3cc2cfc0702f54fcdc48e8941cf7ed
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37368103"
---
# <a name="mobileapp-resource-type"></a>Tipo de recurso mobileApp

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe abstrata que contém as propriedades base de aplicativos móveis do Intune.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mobileApps](../api/intune-apps-mobileapp-list.md)|Coleção [mobileApp](../resources/intune-apps-mobileapp.md)|Lista propriedades e relações dos objetos [mobileApp](../resources/intune-apps-mobileapp.md).|
|[Obter mobileApp](../api/intune-apps-mobileapp-get.md)|[mobileApp](../resources/intune-apps-mobileapp.md)|Propriedades de leitura e relações do objeto [mobileApp](../resources/intune-apps-mobileapp.md).|
|[ação assign](../api/intune-apps-mobileapp-assign.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|displayName|String|O título do aplicativo importado ou definido pelo administrador.|
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
|notes|String|Anotações para o aplicativo.|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|O estado de publicação do aplicativo. O aplicativo não pode ser assinado, a menos que ele seja publicado. Os valores possíveis são: `notPublished`, `processing`, `published`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|categories|Coleção [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|A lista de categorias para este aplicativo.|
|assignments|Coleção [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|A lista de atribuições de grupo para esse aplicativo móvel.|

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
  "publishingState": "String"
}
```




