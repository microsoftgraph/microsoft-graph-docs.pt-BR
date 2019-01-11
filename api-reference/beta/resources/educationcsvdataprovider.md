---
title: tipo de recurso de educationCsvDataProvider
description: 'Usado para configurar o perfil de sincronização de dados da escola quando arquivos CSV são a fonte de entrada.  '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: cb4d08a2a6750310a825f66ecfb0017abacd36fb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878565"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="590af-103">tipo de recurso de educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="590af-103">educationCsvDataProvider resource type</span></span>

> <span data-ttu-id="590af-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="590af-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="590af-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="590af-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="590af-106">Usado para configurar o perfil de sincronização de dados da escola quando arquivos CSV são a fonte de entrada.</span><span class="sxs-lookup"><span data-stu-id="590af-106">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="590af-107">Derivado do [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="590af-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="590af-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="590af-108">Properties</span></span>

| <span data-ttu-id="590af-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="590af-109">Property</span></span> | <span data-ttu-id="590af-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="590af-110">Type</span></span> | <span data-ttu-id="590af-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="590af-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="590af-112">**personalizações**</span><span class="sxs-lookup"><span data-stu-id="590af-112">**customizations**</span></span> | [<span data-ttu-id="590af-113">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="590af-113">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="590af-114">Personalizações opcionais a ser aplicado ao perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="590af-114">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="590af-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="590af-115">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationCsvDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationCsvDataProvider",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
