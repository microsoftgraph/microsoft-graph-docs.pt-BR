---
author: learafa
description: O recurso Adicionadostorageplaninformation fornece informações sobre os planos de cota de armazenamento da unidade.
title: Adicionadostorageplaninformation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: b8b4778a4726c227bfe79ad13ecb14507b13a889
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036951"
---
# <a name="storageplaninformation-resource-type"></a><span data-ttu-id="ad13c-103">tipo de recurso Adicionadostorageplaninformation</span><span class="sxs-lookup"><span data-stu-id="ad13c-103">storagePlanInformation resource type</span></span>

<span data-ttu-id="ad13c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad13c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ad13c-105">Fornece informações sobre os planos de cota de armazenamento da unidade.</span><span class="sxs-lookup"><span data-stu-id="ad13c-105">Provides information about the drive's storage quota plans.</span></span>

## <a name="properties"></a><span data-ttu-id="ad13c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ad13c-106">Properties</span></span>

| <span data-ttu-id="ad13c-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="ad13c-107">Property name</span></span>     | <span data-ttu-id="ad13c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad13c-108">Type</span></span>      | <span data-ttu-id="ad13c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad13c-109">Description</span></span>                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| <span data-ttu-id="ad13c-110">**upgradeAvailable**</span><span class="sxs-lookup"><span data-stu-id="ad13c-110">**upgradeAvailable**</span></span>  | <span data-ttu-id="ad13c-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad13c-111">Boolean</span></span>   | <span data-ttu-id="ad13c-112">Indica se há planos de cota de armazenamento mais altos disponíveis.</span><span class="sxs-lookup"><span data-stu-id="ad13c-112">Indicates whether there are higher storage quota plans available.</span></span> <span data-ttu-id="ad13c-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ad13c-113">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ad13c-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ad13c-114">JSON representation</span></span>

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


