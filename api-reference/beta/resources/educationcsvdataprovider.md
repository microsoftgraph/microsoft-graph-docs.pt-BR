---
title: tipo de recurso educationCsvDataProvider
description: 'Usado para configurar o perfil de sincronização de dados da escola quando os arquivos CSV são a fonte de entrada.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f515744f5206ea132531373e3df317e02dd6cbb4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006399"
---
# <a name="educationcsvdataprovider-resource-type"></a>tipo de recurso educationCsvDataProvider

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
