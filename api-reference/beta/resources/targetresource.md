---
title: tipo complexo de recurso de targetResource-API do Microsoft Graph
description: Define o tipo complexo de recurso de entidade de targetResource da API do Microsoft Graph que oferece suporte à atividade de locatário de relatórios de log de auditoria (locatário).
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bec25af7e0f39a4adf15577c21d4141e1a3c431a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985647"
---
# <a name="targetresource-resource-type"></a>tipo de recurso targetResource

Namespace: microsoft.graph

Representa os tipos de recursos de destino associados à atividade de auditoria. 


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String|Indica a ID exclusiva do recurso.|
|displayName|String|Indica o nome visível definido para o recurso. Normalmente especificado quando o recurso é criado.|
|tipo|String|Descreve o tipo de recurso.  Os valores de exemplo incluem `Application` ,, `Group` `ServicePrincipal` e `User` .|
|userPrincipalName|String|Quando **Type** está definido como `User` , isso inclui o nome de usuário que iniciou a ação; `null` para outros tipos.|
|groupType|String|Quando **Type** é definido como `Group` , isso indica o tipo de grupo.|
|ModifiedProperties|coleção [modifiedproperty](modifiedproperty.md)|Indica o nome, o valor antigo e o novo valor de cada atributo que foi alterado. Os valores de propriedade dependem do **tipo**de operação.|

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


