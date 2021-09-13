---
title: Tipo de recurso securityResource
description: Representa os recursos relacionados a um alerta.
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 377b3828e254676912f549c51aa3776a297edd4b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59054069"
---
# <a name="securityresource-resource-type"></a>Tipo de recurso securityResource

Namespace: microsoft.graph

Representa os recursos relacionados a um alerta.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|recurso|Cadeia de Caracteres|Nome do recurso relacionado ao alerta atual. **Obrigatório**.|
|resourceType|[securityResourceType](#securityresourcetype-values)|Representa o tipo de recursos de segurança relacionados a um alerta. Os valores possíveis são: `attacked` e `related`.|

### <a name="securityresourcetype-values"></a>valores securityResourceType

|Membro|Valor|Descrição|
|-|-|-|
|attacked|1|O recurso foi atacado no alerta.|
|related|2|O recurso está relacionado ao alerta, embora não tenha sido diretamente atacado.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.securityResource"
}-->

```json
{
  "resource": "String",
  "resourceType": "@odata.type: microsoft.graph.securityResourceType"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


