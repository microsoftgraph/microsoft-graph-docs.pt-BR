---
title: tipo de recurso de dimensões
description: Uma dimensão no Dynamics 365 Business central.
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: ed7c7a389778e651af8d2c11c53277a27e022ce1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42504535"
---
# <a name="dimensions-resource-type"></a>Tipo de recurso de dimensões

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|lastModifiedDateTime|datetime               |O último DateTime que a dimensão foi modificada.|  


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

