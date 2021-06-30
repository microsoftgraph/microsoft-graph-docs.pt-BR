---
title: Tipo de recurso cloudPcAuditResource
description: Representa o recurso de auditoria.Isso mostra a entidade de recurso editada de destino, com várias propriedades editadas.
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: ebd61a14680c5e5f2917e273456bcce60672149e
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211212"
---
# <a name="cloudpcauditresource-resource-type"></a>Tipo de recurso cloudPcAuditResource

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o recurso de auditoria.Isso mostra a entidade de recurso editada de destino, com várias propriedades editadas.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome de exibição da entidade de recurso.|
|ModifiedProperties|[Coleção cloudPcAuditProperty](../resources/cloudpcauditproperty.md)|Uma lista de propriedades modificadas.|
|tipo|String|O tipo do recurso de auditoria.|
|resourceId|Cadeia de caracteres|A ID do recurso de auditoria.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcAuditResource"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcAuditResource",
  "displayName": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.cloudPcAuditProperty",
      "displayName": "String",
      "oldValue": "String",
      "newValue": "String"
    }
  ],
  "type": "String",
  "resourceId": "String"
}
```
