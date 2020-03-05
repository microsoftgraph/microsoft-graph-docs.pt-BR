---
title: tipo de recurso dimensionValues
description: Um valor de dimensão no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 368fc28f7bd46d8d5385b6e6041cd82255e0271f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42504136"
---
# <a name="dimensionvalues-resource-type"></a>tipo de recurso dimensionValues

Namespace: Microsoft. Graph

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
|displayName         |string                 |Especifica o nome do valor da dimensão. Esse nome aparecerá onde o valor de dimensão é usado.|
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


