---
title: Tipo complexo de recurso targetResource - API do Microsoft Graph
description: Define o tipo complexo de recurso da entidade targetResource da API do Microsoft Graph que oferece suporte à atividade da organização de relatório de log de auditoria (locatário).
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
ms.openlocfilehash: 2dc8adea2edf11674d844cee4e5548da96882f7d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137582"
---
# <a name="targetresource-resource-type"></a>Tipo de recurso targetResource

Namespace: microsoft.graph

Representa os tipos de recursos de destino associados à atividade de auditoria. 


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String|Indica a ID exclusiva do recurso.|
|displayName|String|Indica o nome visível definido para o recurso. Normalmente especificado quando o recurso é criado.|
|type|String|Descreve o tipo de recurso.  Os valores de `Application` exemplo `Group` incluem , `ServicePrincipal` e `User` .|
|userPrincipalName|String|Quando **o** tipo é definido `User` como , isso inclui o nome de usuário que iniciou a ação; `null` para outros tipos.|
|groupType|String|Quando **o** tipo é definido `Group` como , isso indica o tipo de grupo.|
|ModifiedProperties|[Coleção modifiedProperty](modifiedproperty.md)|Indica o nome, o valor antigo e o novo valor de cada atributo que foi alterado. Os valores de propriedade dependem do tipo de **operação.**|

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


