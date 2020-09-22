---
title: tipo de recurso educationCsvDataProvider
description: 'Usado para configurar o perfil de sincronização de dados da escola quando os arquivos CSV são a fonte de entrada.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 60377b1761bcb5c672ae42f3067bb20d41325e9c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095530"
---
# <a name="educationcsvdataprovider-resource-type"></a>tipo de recurso educationCsvDataProvider

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado para configurar o perfil de sincronização de dados da escola quando os arquivos CSV são a fonte de entrada.

Derivado de [educationSynchronizationDataProvider].

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo                                     | Descrição                                                           |
| :------------- | :--------------------------------------- | :-------------------------------------------------------------------- |
| personalizações | [educationSynchronizationCustomizations] | Personalizações opcionais a serem aplicadas ao perfil de sincronização. |

[educationsynchronizationdataprovider]: educationsynchronizationdataprovider.md
[educationsynchronizationcustomizations]: educationsynchronizationcustomizations.md

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCsvDataProvider"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationCsvDataProvider",
  "customizations": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
  }
}
```


