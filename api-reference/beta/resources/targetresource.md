---
title: tipo complexo de recurso de targetResource-API do Microsoft Graph
description: Define o tipo complexo de recurso de entidade de targetResource da API do Microsoft Graph que oferece suporte à atividade de locatário de relatórios de log de auditoria (locatário).
author: davidmu1
localization_priority: Normal
doc_type: resourcePageType
ms.prod: azure-ad
ms.openlocfilehash: a67cfbccf9d05872ec0d9207ac54c51cda222053
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964575"
---
# <a name="targetresource-resource-type"></a>tipo de recurso targetResource

Representa os tipos de recursos de destino associados à atividade de auditoria. 


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String|Indica a ID exclusiva do recurso.|
|displayName|String|Indica o nome visível definido para o recurso. Normalmente especificado quando o recurso é criado.|
|type|String|Descreve o tipo de recurso.  Os valores de `Application`exemplo `Group`incluem `ServicePrincipal`,, `User`e.|
|userPrincipalName|Cadeia de caracteres|Quando o **tipo** está definido `User`como, isso inclui o nome de usuário que iniciou a ação; `null` para outros tipos.|
|groupType|String|Quando **Type** é definido como `Group`, isso indica o tipo de grupo.|
|ModifiedProperties|[](modifiedproperty.md) coleção modifiedproperty|Indica o nome, o valor antigo e o novo valor de cada atributo que foi alterado. Os valores de propriedade dependem do **tipo**de operação.|

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
