---
title: tipo de recurso educationCsvDataProvider
description: 'Usado para configurar o perfil de sincronização de dados da escola quando os arquivos CSV são a fonte de entrada.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 207fee7f889c4369862918943371e2d629c8fab9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502169"
---
# <a name="educationcsvdataprovider-resource-type"></a>tipo de recurso educationCsvDataProvider

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado para configurar o perfil de sincronização de dados da escola quando os arquivos CSV são a fonte de entrada.  

Derivado de [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **personalizações** | [educationSynchronizationCustomizations](educationsynchronizationcustomizations.md) | Personalizações opcionais a serem aplicadas ao perfil de sincronização.|

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
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
