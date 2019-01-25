---
author: psampath
ms.author: psampath
ms.date: 06/20/2018
title: StoragePlanInformation
localization_priority: Normal
ms.openlocfilehash: 05140b3256e434449d663c4992e74298bbdedd30
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519231"
---
# <a name="storageplaninformation-resource-type"></a><span data-ttu-id="63401-102">tipo de recurso de storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="63401-102">storagePlanInformation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63401-103">O recurso de **storagePlanInformation** fornece informações sobre os planos de cota de armazenamento da unidade.</span><span class="sxs-lookup"><span data-stu-id="63401-103">The **storagePlanInformation** resource provides information about the drive's storage quota plans.</span></span>

### <a name="json-representation"></a><span data-ttu-id="63401-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="63401-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
   "@odata.type": "microsoft.graph.storagePlanInformation",
} -->

```json
{
  "upgradeAvailable": true
}

```
## <a name="properties"></a><span data-ttu-id="63401-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="63401-105">Properties</span></span>

| <span data-ttu-id="63401-106">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="63401-106">Property name</span></span>     | <span data-ttu-id="63401-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="63401-107">Type</span></span>      | <span data-ttu-id="63401-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="63401-108">Description</span></span>                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| <span data-ttu-id="63401-109">upgradeAvailable</span><span class="sxs-lookup"><span data-stu-id="63401-109">upgradeAvailable</span></span>  | <span data-ttu-id="63401-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="63401-110">Boolean</span></span>   | <span data-ttu-id="63401-111">Indica se os planos de cota de armazenamento mais estarão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="63401-111">Indicates if there are higher storage quota plans available.</span></span> <span data-ttu-id="63401-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="63401-112">Read-only.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "storagePlanInformation resource contains information about storage quota plans that make up the drive's storage space quota.",
  "keywords": "quota,plans,upgradeAvailable",
  "section": "documentation",
  "tocPath": "Resources/StoragePlanInformation",
  "suppressions": [
    "Error: /api-reference/beta/resources/storageplaninformation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

