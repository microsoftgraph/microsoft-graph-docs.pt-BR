---
title: tipo de recurso educationCsvDataProvider
description: 'Usado para configurar o perfil de sincronização de dados da escola quando os arquivos CSV são a fonte de entrada.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bebacbc1c618c7558d81bde2611840e8d225a8fd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507172"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="8ea7d-103">tipo de recurso educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="8ea7d-103">educationCsvDataProvider resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ea7d-104">Usado para configurar o perfil de sincronização de dados da escola quando os arquivos CSV são a fonte de entrada.</span><span class="sxs-lookup"><span data-stu-id="8ea7d-104">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="8ea7d-105">Derivado de [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="8ea7d-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8ea7d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8ea7d-106">Properties</span></span>

| <span data-ttu-id="8ea7d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ea7d-107">Property</span></span> | <span data-ttu-id="8ea7d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ea7d-108">Type</span></span> | <span data-ttu-id="8ea7d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ea7d-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="8ea7d-110">**personalizações**</span><span class="sxs-lookup"><span data-stu-id="8ea7d-110">**customizations**</span></span> | [<span data-ttu-id="8ea7d-111">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="8ea7d-111">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="8ea7d-112">Personalizações opcionais a serem aplicadas ao perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="8ea7d-112">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8ea7d-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8ea7d-113">JSON representation</span></span>

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
