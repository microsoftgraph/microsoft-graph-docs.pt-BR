---
title: tipo de recurso de educationCsvDataProvider
description: 'Usado para configurar o perfil de sincronização de dados da escola quando arquivos CSV são a fonte de entrada.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 19ef77671f862a0b59b5697b76bb54dc20e42856
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952752"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="27a3a-103">tipo de recurso de educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="27a3a-103">educationCsvDataProvider resource type</span></span>

> <span data-ttu-id="27a3a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="27a3a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27a3a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="27a3a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="27a3a-106">Usado para configurar o perfil de sincronização de dados da escola quando arquivos CSV são a fonte de entrada.</span><span class="sxs-lookup"><span data-stu-id="27a3a-106">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="27a3a-107">Derivado do [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="27a3a-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="27a3a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="27a3a-108">Properties</span></span>

| <span data-ttu-id="27a3a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27a3a-109">Property</span></span> | <span data-ttu-id="27a3a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="27a3a-110">Type</span></span> | <span data-ttu-id="27a3a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="27a3a-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="27a3a-112">**personalizações**</span><span class="sxs-lookup"><span data-stu-id="27a3a-112">**customizations**</span></span> | [<span data-ttu-id="27a3a-113">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="27a3a-113">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="27a3a-114">Personalizações opcionais a ser aplicado ao perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="27a3a-114">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="27a3a-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="27a3a-115">JSON representation</span></span>

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
