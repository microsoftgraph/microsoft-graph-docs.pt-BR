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
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="8dd47-103">tipo de recurso educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="8dd47-103">educationCsvDataProvider resource type</span></span>

<span data-ttu-id="8dd47-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8dd47-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8dd47-105">Usado para configurar o perfil de sincronização de dados da escola quando os arquivos CSV são a fonte de entrada.</span><span class="sxs-lookup"><span data-stu-id="8dd47-105">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>

<span data-ttu-id="8dd47-106">Derivado de [educationSynchronizationDataProvider].</span><span class="sxs-lookup"><span data-stu-id="8dd47-106">Derived from [educationSynchronizationDataProvider].</span></span>

## <a name="properties"></a><span data-ttu-id="8dd47-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8dd47-107">Properties</span></span>

| <span data-ttu-id="8dd47-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8dd47-108">Property</span></span>       | <span data-ttu-id="8dd47-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8dd47-109">Type</span></span>                                     | <span data-ttu-id="8dd47-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8dd47-110">Description</span></span>                                                           |
| :------------- | :--------------------------------------- | :-------------------------------------------------------------------- |
| <span data-ttu-id="8dd47-111">personalizações</span><span class="sxs-lookup"><span data-stu-id="8dd47-111">customizations</span></span> | <span data-ttu-id="8dd47-112">[educationSynchronizationCustomizations]</span><span class="sxs-lookup"><span data-stu-id="8dd47-112">[educationSynchronizationCustomizations]</span></span> | <span data-ttu-id="8dd47-113">Personalizações opcionais a serem aplicadas ao perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="8dd47-113">Optional customizations to be applied to the synchronization profile.</span></span> |

[educationsynchronizationdataprovider]: educationsynchronizationdataprovider.md
[educationsynchronizationcustomizations]: educationsynchronizationcustomizations.md

## <a name="json-representation"></a><span data-ttu-id="8dd47-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8dd47-116">JSON representation</span></span>

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


