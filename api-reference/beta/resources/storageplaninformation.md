---
author: psampath
ms.author: psampath
ms.date: 06/20/2018
title: Adicionadostorageplaninformation
localization_priority: Normal
ms.openlocfilehash: 3911d3af5f2149d1043ed246e7c11d287c840842
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342916"
---
# <a name="storageplaninformation-resource-type"></a><span data-ttu-id="c064c-102">tipo de recurso Adicionadostorageplaninformation</span><span class="sxs-lookup"><span data-stu-id="c064c-102">storagePlanInformation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c064c-103">O recurso **adicionadostorageplaninformation** fornece informações sobre os planos de cota de armazenamento da unidade.</span><span class="sxs-lookup"><span data-stu-id="c064c-103">The **storagePlanInformation** resource provides information about the drive's storage quota plans.</span></span>

### <a name="json-representation"></a><span data-ttu-id="c064c-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c064c-104">JSON representation</span></span>

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
## <a name="properties"></a><span data-ttu-id="c064c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c064c-105">Properties</span></span>

| <span data-ttu-id="c064c-106">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="c064c-106">Property name</span></span>     | <span data-ttu-id="c064c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c064c-107">Type</span></span>      | <span data-ttu-id="c064c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c064c-108">Description</span></span>                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| <span data-ttu-id="c064c-109">upgradeAvailable</span><span class="sxs-lookup"><span data-stu-id="c064c-109">upgradeAvailable</span></span>  | <span data-ttu-id="c064c-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="c064c-110">Boolean</span></span>   | <span data-ttu-id="c064c-111">Indica se há planos de cota de armazenamento mais altos disponíveis.</span><span class="sxs-lookup"><span data-stu-id="c064c-111">Indicates if there are higher storage quota plans available.</span></span> <span data-ttu-id="c064c-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c064c-112">Read-only.</span></span> |


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

