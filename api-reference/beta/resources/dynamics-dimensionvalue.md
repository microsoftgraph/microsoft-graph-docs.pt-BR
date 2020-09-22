---
title: tipo de recurso dimensionValues
description: Um valor de dimensão no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: acb1c8d34f8ee876c39ac99d5f43feb7f9a128c7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071343"
---
# <a name="dimensionvalues-resource-type"></a>tipo de recurso dimensionValues

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um valor de dimensão no Dynamics 365 Business central.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição                   |
|:-------------|:-------------|:-----------------------------|
|[Obter dimensionValues](../api/dynamics-dimensionvalue-get.md)|dimensionValues|Obtém um objeto de valor de dimensão.|


## <a name="properties"></a>Propriedades
| Propriedade           | Tipo                  |Descrição                                        |
|:-------------------|:----------------------|:--------------------------------------------------|
|id                  |GUID                   |A ID exclusiva do item.                         |
|código                |Cadeia de caracteres, tamanho máximo 20|O código do valor da dimensão.                          |
|displayName         |cadeia de caracteres                 |Especifica o nome do valor da dimensão. Esse nome aparecerá onde o valor de dimensão é usado.|
|lastModifiedDateTime|datetime               |A última data/hora em que o valor de dimensão foi modificado.|  


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




