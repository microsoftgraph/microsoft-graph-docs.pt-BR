---
author: learafa
description: O recurso Adicionadostorageplaninformation fornece informações sobre os planos de cota de armazenamento da unidade.
title: Adicionadostorageplaninformation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: a5e6c10bdbc8a68230a223501844d0ee121014c2
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863772"
---
# <a name="storageplaninformation-resource-type"></a><span data-ttu-id="c26a9-103">tipo de recurso Adicionadostorageplaninformation</span><span class="sxs-lookup"><span data-stu-id="c26a9-103">storagePlanInformation resource type</span></span>

<span data-ttu-id="c26a9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c26a9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c26a9-105">Fornece informações sobre os planos de cota de armazenamento da unidade.</span><span class="sxs-lookup"><span data-stu-id="c26a9-105">Provides information about the drive's storage quota plans.</span></span>

## <a name="properties"></a><span data-ttu-id="c26a9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c26a9-106">Properties</span></span>

| <span data-ttu-id="c26a9-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="c26a9-107">Property name</span></span>     | <span data-ttu-id="c26a9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c26a9-108">Type</span></span>      | <span data-ttu-id="c26a9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c26a9-109">Description</span></span>                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| <span data-ttu-id="c26a9-110">**upgradeAvailable**</span><span class="sxs-lookup"><span data-stu-id="c26a9-110">**upgradeAvailable**</span></span>  | <span data-ttu-id="c26a9-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="c26a9-111">Boolean</span></span>   | <span data-ttu-id="c26a9-112">Indica se há planos de cota de armazenamento mais altos disponíveis.</span><span class="sxs-lookup"><span data-stu-id="c26a9-112">Indicates whether there are higher storage quota plans available.</span></span> <span data-ttu-id="c26a9-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c26a9-113">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c26a9-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c26a9-114">JSON representation</span></span>

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

