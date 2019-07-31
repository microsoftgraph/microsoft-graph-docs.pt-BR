---
title: tipo de recurso dimensionValues
description: Um valor de dimensão no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: af7ba3b49051a4e89fcdf2a4a408a1f72fc547ad
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973612"
---
# <a name="dimensionvalues-resource-type"></a>tipo de recurso dimensionValues
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
|lastModifiedDateTime|DateTime               |A última data/hora em que o valor de dimensão foi modificado.|  


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


