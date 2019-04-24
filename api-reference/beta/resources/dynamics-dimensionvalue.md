---
title: tipo de recurso dimensionValues
description: Um valor de dimensão no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: da3935b8e784b05551af123c1832d5dc84a2c81c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507214"
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
|code                |Cadeia de caracteres, tamanho máximo 20|O código do valor da dimensão.                          |
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


