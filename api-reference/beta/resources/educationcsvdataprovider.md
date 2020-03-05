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
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="f62f5-103">tipo de recurso educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="f62f5-103">educationCsvDataProvider resource type</span></span>

<span data-ttu-id="f62f5-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f62f5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f62f5-105">Usado para configurar o perfil de sincronização de dados da escola quando os arquivos CSV são a fonte de entrada.</span><span class="sxs-lookup"><span data-stu-id="f62f5-105">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="f62f5-106">Derivado de [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="f62f5-106">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f62f5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f62f5-107">Properties</span></span>

| <span data-ttu-id="f62f5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f62f5-108">Property</span></span> | <span data-ttu-id="f62f5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f62f5-109">Type</span></span> | <span data-ttu-id="f62f5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f62f5-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="f62f5-111">**personalizações**</span><span class="sxs-lookup"><span data-stu-id="f62f5-111">**customizations**</span></span> | [<span data-ttu-id="f62f5-112">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="f62f5-112">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="f62f5-113">Personalizações opcionais a serem aplicadas ao perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="f62f5-113">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f62f5-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f62f5-114">JSON representation</span></span>

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
