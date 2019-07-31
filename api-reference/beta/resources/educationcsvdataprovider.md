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
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="93337-103">tipo de recurso educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="93337-103">educationCsvDataProvider resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93337-104">Usado para configurar o perfil de sincronização de dados da escola quando os arquivos CSV são a fonte de entrada.</span><span class="sxs-lookup"><span data-stu-id="93337-104">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="93337-105">Derivado de [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="93337-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="93337-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="93337-106">Properties</span></span>

| <span data-ttu-id="93337-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93337-107">Property</span></span> | <span data-ttu-id="93337-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="93337-108">Type</span></span> | <span data-ttu-id="93337-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="93337-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="93337-110">**personalizações**</span><span class="sxs-lookup"><span data-stu-id="93337-110">**customizations**</span></span> | [<span data-ttu-id="93337-111">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="93337-111">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="93337-112">Personalizações opcionais a serem aplicadas ao perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="93337-112">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="93337-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="93337-113">JSON representation</span></span>

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
