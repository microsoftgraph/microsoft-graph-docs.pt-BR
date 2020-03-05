---
author: psampath
description: O recurso Adicionadostorageplaninformation fornece informações sobre os planos de cota de armazenamento da unidade.
ms.date: 06/20/2018
title: Adicionadostorageplaninformation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 79254efa033528bd8fd4cf66a07959a71e3fef1a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520433"
---
# <a name="storageplaninformation-resource-type"></a><span data-ttu-id="bf9a9-103">tipo de recurso Adicionadostorageplaninformation</span><span class="sxs-lookup"><span data-stu-id="bf9a9-103">storagePlanInformation resource type</span></span>

<span data-ttu-id="bf9a9-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bf9a9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf9a9-105">O recurso **adicionadostorageplaninformation** fornece informações sobre os planos de cota de armazenamento da unidade.</span><span class="sxs-lookup"><span data-stu-id="bf9a9-105">The **storagePlanInformation** resource provides information about the drive's storage quota plans.</span></span>

### <a name="json-representation"></a><span data-ttu-id="bf9a9-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bf9a9-106">JSON representation</span></span>

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
## <a name="properties"></a><span data-ttu-id="bf9a9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bf9a9-107">Properties</span></span>

| <span data-ttu-id="bf9a9-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="bf9a9-108">Property name</span></span>     | <span data-ttu-id="bf9a9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf9a9-109">Type</span></span>      | <span data-ttu-id="bf9a9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf9a9-110">Description</span></span>                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| <span data-ttu-id="bf9a9-111">upgradeAvailable</span><span class="sxs-lookup"><span data-stu-id="bf9a9-111">upgradeAvailable</span></span>  | <span data-ttu-id="bf9a9-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf9a9-112">Boolean</span></span>   | <span data-ttu-id="bf9a9-113">Indica se há planos de cota de armazenamento mais altos disponíveis.</span><span class="sxs-lookup"><span data-stu-id="bf9a9-113">Indicates if there are higher storage quota plans available.</span></span> <span data-ttu-id="bf9a9-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bf9a9-114">Read-only.</span></span> |


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

