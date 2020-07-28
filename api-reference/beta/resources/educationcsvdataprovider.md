---
title: tipo de recurso educationCsvDataProvider
description: 'Usado para configurar o perfil de sincronização de dados da escola quando os arquivos CSV são a fonte de entrada.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 33cb0268eeb8c6d6b896dfb8ab02f7bb59b00e98
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434981"
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
