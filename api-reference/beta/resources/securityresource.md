---
title: Tipo de recurso securityResource
description: Representa os recursos relacionados a um alerta.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: f8beb524375db5fc4187f210b8602e534835a53f3dc9c52b60ee57085f904ce2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54212931"
---
# <a name="securityresource-resource-type"></a>Tipo de recurso securityResource

Namespace: microsoft.graph

Representa os recursos relacionados a um alerta.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|recurso|Cadeia de caracteres|Nome do recurso relacionado ao alerta atual. **Obrigatório**.|
|resourceType|[securityResourceType](#securityresourcetype-values)|Representa o tipo de recursos de segurança relacionados a um alerta. Os valores possíveis são: `attacked` e `related`.|

### <a name="securityresourcetype-values"></a>valores securityResourceType

|Membro|Valor|Descrição|
|-|-|-|
|attacked|1 |O recurso foi atacado no alerta.|
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


