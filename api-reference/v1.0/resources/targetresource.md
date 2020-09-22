---
title: tipo de recurso targetResource
description: Representa os tipos de recursos de destino associados à atividade de auditoria.
localization_priority: Normal
author: dhanyahk
ms.prod: azure-ad
doc_type: resourcePageType
ms.openlocfilehash: 641097b6e8b4646d878182ba1763fd62ab75b080
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094054"
---
# <a name="targetresource-resource-type"></a>tipo de recurso targetResource

Namespace: microsoft.graph

Representa os tipos de recursos de destino associados à atividade de auditoria. 

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres|Indica a ID exclusiva do recurso.|
|displayName|Cadeia de caracteres|Indica o nome visível definido para o recurso. Normalmente especificado quando o recurso é criado.|
|type|Cadeia de caracteres|Descreve o tipo de recurso.  Os valores de exemplo incluem `Application` ,, `Group` `ServicePrincipal` e `User` .|
|userPrincipalName|Cadeia de caracteres|Quando **Type** está definido como `User` , isso inclui o nome de usuário que iniciou a ação; `null` para outros tipos.|
|groupType|Cadeia de caracteres|Quando **Type** é definido como `Group` , isso indica o tipo de grupo.|
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

