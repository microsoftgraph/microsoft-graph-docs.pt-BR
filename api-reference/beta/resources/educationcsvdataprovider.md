---
title: tipo de recurso de educationCsvDataProvider
description: 'Usado para configurar o perfil de sincronização de dados da escola quando arquivos CSV são a fonte de entrada.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bebacbc1c618c7558d81bde2611840e8d225a8fd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529870"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="06256-103">tipo de recurso de educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="06256-103">educationCsvDataProvider resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06256-104">Usado para configurar o perfil de sincronização de dados da escola quando arquivos CSV são a fonte de entrada.</span><span class="sxs-lookup"><span data-stu-id="06256-104">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="06256-105">Derivado do [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="06256-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="06256-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="06256-106">Properties</span></span>

| <span data-ttu-id="06256-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06256-107">Property</span></span> | <span data-ttu-id="06256-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="06256-108">Type</span></span> | <span data-ttu-id="06256-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="06256-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="06256-110">**personalizações**</span><span class="sxs-lookup"><span data-stu-id="06256-110">**customizations**</span></span> | [<span data-ttu-id="06256-111">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="06256-111">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="06256-112">Personalizações opcionais a ser aplicado ao perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="06256-112">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="06256-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="06256-113">JSON representation</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationcsvdataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
