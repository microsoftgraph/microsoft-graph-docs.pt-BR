---
title: tipo de recurso dimensions
description: Uma dimensão no Dynamics 365 Business Central.
author: SusanneWindfeldPedersen
ms.localizationpriority: medium
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: db1a243a9f7eabb8436a6f1ca2b64fe5b74508b5
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767073"
---
# <a name="dimensions-resource-type"></a>Tipo de recurso Dimensions

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma dimensão no Dynamics 365 Business Central.

## <a name="methods"></a>Métodos
| Método       | Tipo de retorno  |Descrição|
|:-------------|:-------------|:----------|
|[Obter dimensões](../api/dynamics-dimension-get.md)|dimension|Obtém uma dimensão.|


## <a name="properties"></a>Propriedades
| Propriedade           | Tipo                  |Descrição               |
|:-------------------|:----------------------|:-------------------------|
|id                  |GUID                   |A ID exclusiva do item.|
|código                |string, tamanho máximo 20|O código de dimensão.       |
|displayName         |string                 |Especifica o nome da dimensão. Esse nome aparecerá onde a dimensão é usada.|
|lastModifiedDateTime|datetime               |A última data em que a dimensão foi modificada.|  


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



