---
author: psampath
description: O recurso Adicionadostorageplaninformation fornece informações sobre os planos de cota de armazenamento da unidade.
ms.date: 06/20/2018
title: Adicionadostorageplaninformation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: d8ddb39f9f7c6443f0e669052084af27b8fd5cec
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008079"
---
# <a name="storageplaninformation-resource-type"></a><span data-ttu-id="a9ac7-103">tipo de recurso Adicionadostorageplaninformation</span><span class="sxs-lookup"><span data-stu-id="a9ac7-103">storagePlanInformation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9ac7-104">O recurso **adicionadostorageplaninformation** fornece informações sobre os planos de cota de armazenamento da unidade.</span><span class="sxs-lookup"><span data-stu-id="a9ac7-104">The **storagePlanInformation** resource provides information about the drive's storage quota plans.</span></span>

### <a name="json-representation"></a><span data-ttu-id="a9ac7-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a9ac7-105">JSON representation</span></span>

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
## <a name="properties"></a><span data-ttu-id="a9ac7-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a9ac7-106">Properties</span></span>

| <span data-ttu-id="a9ac7-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="a9ac7-107">Property name</span></span>     | <span data-ttu-id="a9ac7-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9ac7-108">Type</span></span>      | <span data-ttu-id="a9ac7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9ac7-109">Description</span></span>                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| <span data-ttu-id="a9ac7-110">upgradeAvailable</span><span class="sxs-lookup"><span data-stu-id="a9ac7-110">upgradeAvailable</span></span>  | <span data-ttu-id="a9ac7-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="a9ac7-111">Boolean</span></span>   | <span data-ttu-id="a9ac7-112">Indica se há planos de cota de armazenamento mais altos disponíveis.</span><span class="sxs-lookup"><span data-stu-id="a9ac7-112">Indicates if there are higher storage quota plans available.</span></span> <span data-ttu-id="a9ac7-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a9ac7-113">Read-only.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "storagePlanInformation resource contains information about storage quota plans that make up the drive's storage space quota.",
  "keywords": "quota,plans,upgradeAvailable",
  "section": "documentation",
  "tocPath": "Resources/StoragePlanInformation",
  "suppressions": []
}
-->

