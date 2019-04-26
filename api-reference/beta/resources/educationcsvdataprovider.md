---
title: tipo de recurso educationCsvDataProvider
description: 'Usado para configurar o perfil de sincronização de dados da escola quando os arquivos CSV são a fonte de entrada.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 4dbbf5d5791df1035fcd9fe1a953d8a9a347070a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340564"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="8d2dd-103">tipo de recurso educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="8d2dd-103">educationCsvDataProvider resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d2dd-104">Usado para configurar o perfil de sincronização de dados da escola quando os arquivos CSV são a fonte de entrada.</span><span class="sxs-lookup"><span data-stu-id="8d2dd-104">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="8d2dd-105">Derivado de [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="8d2dd-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8d2dd-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8d2dd-106">Properties</span></span>

| <span data-ttu-id="8d2dd-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d2dd-107">Property</span></span> | <span data-ttu-id="8d2dd-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d2dd-108">Type</span></span> | <span data-ttu-id="8d2dd-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d2dd-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="8d2dd-110">**personalizações**</span><span class="sxs-lookup"><span data-stu-id="8d2dd-110">**customizations**</span></span> | [<span data-ttu-id="8d2dd-111">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="8d2dd-111">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="8d2dd-112">Personalizações opcionais a serem aplicadas ao perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="8d2dd-112">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8d2dd-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8d2dd-113">JSON representation</span></span>

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
