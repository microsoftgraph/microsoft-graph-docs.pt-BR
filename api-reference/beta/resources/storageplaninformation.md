---
author: psampath
ms.author: psampath
ms.date: 06/20/2018
title: StoragePlanInformation
localization_priority: Normal
ms.openlocfilehash: bbe4faaffbf53c24d4d0f5b8ea1f5ee1e1966a2c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860120"
---
# <a name="storageplaninformation-resource-type"></a><span data-ttu-id="7d656-102">tipo de recurso de storagePlanInformation</span><span class="sxs-lookup"><span data-stu-id="7d656-102">storagePlanInformation resource type</span></span>

> <span data-ttu-id="7d656-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7d656-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d656-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7d656-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7d656-105">O recurso de **storagePlanInformation** fornece informações sobre os planos de cota de armazenamento da unidade.</span><span class="sxs-lookup"><span data-stu-id="7d656-105">The **storagePlanInformation** resource provides information about the drive's storage quota plans.</span></span>

### <a name="json-representation"></a><span data-ttu-id="7d656-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7d656-106">JSON representation</span></span>

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
## <a name="properties"></a><span data-ttu-id="7d656-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7d656-107">Properties</span></span>

| <span data-ttu-id="7d656-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="7d656-108">Property name</span></span>     | <span data-ttu-id="7d656-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d656-109">Type</span></span>      | <span data-ttu-id="7d656-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d656-110">Description</span></span>                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| <span data-ttu-id="7d656-111">upgradeAvailable</span><span class="sxs-lookup"><span data-stu-id="7d656-111">upgradeAvailable</span></span>  | <span data-ttu-id="7d656-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="7d656-112">Boolean</span></span>   | <span data-ttu-id="7d656-113">Indica se os planos de cota de armazenamento mais estarão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="7d656-113">Indicates if there are higher storage quota plans available.</span></span> <span data-ttu-id="7d656-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7d656-114">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "storagePlanInformation resource contains information about storage quota plans that make up the drive's storage space quota.",
  "keywords": "quota,plans,upgradeAvailable",
  "section": "documentation",
  "tocPath": "Resources/StoragePlanInformation"
} -->

