---
title: Tipo de recurso cloudPcAuditResource
description: Representa o recurso de auditoria.Isso mostra a entidade de recurso editada de destino, com várias propriedades editadas.
author: ecmadao
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: c168fa404d00f855659a38a096673f0524938f56
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767144"
---
# <a name="cloudpcauditresource-resource-type"></a>Tipo de recurso cloudPcAuditResource

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o recurso de auditoria.Isso mostra a entidade de recurso editada de destino, com várias propriedades editadas.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição da entidade de recurso.|
|ModifiedProperties|[Coleção cloudPcAuditProperty](../resources/cloudpcauditproperty.md)|Uma lista de propriedades modificadas.|
|type|Cadeia de caracteres|O tipo do recurso de auditoria.|
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
