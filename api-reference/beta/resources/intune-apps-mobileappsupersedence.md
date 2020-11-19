---
title: tipo de recurso mobileAppSupersedence
description: Descreve uma relação de substituição entre dois aplicativos móveis.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1e63bdfce275b83587557304f79a8490eb45a68c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49217127"
---
# <a name="mobileappsupersedence-resource-type"></a>tipo de recurso mobileAppSupersedence

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Descreve uma relação de substituição entre dois aplicativos móveis.


Herda de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mobileAppSupersedences](../api/intune-apps-mobileappsupersedence-list.md)|coleção [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md)|Listar Propriedades e relações dos objetos [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) .|
|[Obter mobileAppSupersedence](../api/intune-apps-mobileappsupersedence-get.md)|[mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md)|Leia as propriedades e as relações do objeto [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) .|
|[Criar mobileAppSupersedence](../api/intune-apps-mobileappsupersedence-create.md)|[mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md)|Criar um novo objeto [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) .|
|[Excluir mobileAppSupersedence](../api/intune-apps-mobileappsupersedence-delete.md)|Nenhum|Exclui [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md).|
|[Atualizar mobileAppSupersedence](../api/intune-apps-mobileappsupersedence-update.md)|[mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md)|Atualiza as propriedades de um objeto [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID da entidade de relação. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetId|String|A ID de aplicativo do aplicativo móvel de destino. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetDisplayName|String|O nome de exibição do aplicativo móvel de destino. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetDisplayVersion|String|A versão de exibição do aplicativo móvel de destino. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetPublisher|String|O fornecedor do aplicativo móvel de destino. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetType|[mobileAppRelationshipType](../resources/intune-apps-mobileapprelationshiptype.md)|O tipo de relação que indica se o destino é um pai ou filho. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md). Os valores possíveis são: `child` e `parent`.|
|supersedenceType|[mobileAppSupersedenceType](../resources/intune-apps-mobileappsupersedencetype.md)|O tipo de relação de substituição entre os aplicativos pai e filho. Os valores possíveis são: `update` e `replace`.|
|supersededAppCount|Int32|O número total de aplicativos diretamente ou indiretamente substituídos pelo aplicativo filho.|
|supersedingAppCount|Int32|O número total de aplicativos que substituem diretamente ou indiretamente o aplicativo pai.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppSupersedence"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppSupersedence",
  "id": "String (identifier)",
  "targetId": "String",
  "targetDisplayName": "String",
  "targetDisplayVersion": "String",
  "targetPublisher": "String",
  "targetType": "String",
  "supersedenceType": "String",
  "supersededAppCount": 1024,
  "supersedingAppCount": 1024
}
```




