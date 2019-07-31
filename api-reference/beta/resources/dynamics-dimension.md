---
title: tipo de recurso de dimensões
description: Uma dimensão no Dynamics 365 Business central.
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 5bd5382ae020baaf726db53f9252c4d3498833ee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973622"
---
# <a name="dimensions-resource-type"></a>Tipo de recurso de dimensões
Representa uma dimensão no Dynamics 365 Business central.

## <a name="methods"></a>Métodos
| Método       | Tipo de retorno  |Descrição|
|:-------------|:-------------|:----------|
|[Obter dimensões](../api/dynamics-dimension-get.md)|expressão|Obtém uma dimensão.|


## <a name="properties"></a>Propriedades
| Propriedade           | Tipo                  |Descrição               |
|:-------------------|:----------------------|:-------------------------|
|id                  |GUID                   |A ID exclusiva do item.|
|código                |Cadeia de caracteres, tamanho máximo 20|O código de dimensão.       |
|displayName         |string                 |Especifica o nome da dimensão. Esse nome aparecerá onde a dimensão é usada.|
|lastModifiedDateTime|DateTime               |O último DateTime que a dimensão foi modificada.|  


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```

