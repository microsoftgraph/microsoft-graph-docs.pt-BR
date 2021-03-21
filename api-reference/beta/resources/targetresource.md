---
title: tipo complexo de recurso targetResource - API do Microsoft Graph
description: Define o tipo complexo de recurso da entidade targetResource da API do Microsoft Graph que dá suporte à atividade de organização de relatórios de log de auditoria (locatário).
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
ms.openlocfilehash: 12030bdb5c51e41e821218e3db67c4878a90c53d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954955"
---
# <a name="targetresource-resource-type"></a>tipo de recurso targetResource

Namespace: microsoft.graph

Representa tipos de recursos de destino associados à atividade de auditoria. 


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres|Indica a ID exclusiva do recurso.|
|displayName|Cadeia de caracteres|Indica o nome visível definido para o recurso. Normalmente especificado quando o recurso é criado.|
|tipo|Cadeia de caracteres|Descreve o tipo de recurso.  Os valores de `Application` exemplo `Group` incluem , `ServicePrincipal` , e `User` .|
|userPrincipalName|Cadeia de caracteres|Quando **o** tipo é definido como , isso inclui o nome de usuário que iniciou a `User` ação; para outros `null` tipos.|
|groupType|groupType|Quando **o** tipo é definido como `Group` , isso indica o tipo de grupo.  Os valores possíveis são: `unifiedGroups` `azureAD` , e `unknownFutureValue`|
|ModifiedProperties|[Coleção modifiedProperty](modifiedproperty.md)|Indica nome, valor antigo e novo valor de cada atributo que foi alterado. Os valores de propriedade dependem do tipo de **operação**.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResource"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "type": "String",
  "userPrincipalName": "String",
  "groupType": "String", 
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


