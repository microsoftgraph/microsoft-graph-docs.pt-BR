---
title: tipo de recurso synchronizationError
description: Representa um erro que ocorreu durante o processo de sincronização.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2be415a127f7bcef030407be737bb9b48c8a116f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964666"
---
# <a name="synchronizationerror-resource-type"></a><span data-ttu-id="0b471-103">tipo de recurso synchronizationError</span><span class="sxs-lookup"><span data-stu-id="0b471-103">synchronizationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b471-104">Representa um erro que ocorreu durante o processo de sincronização.</span><span class="sxs-lookup"><span data-stu-id="0b471-104">Represents an error that occurred during the synchronization process.</span></span>

## <a name="properties"></a><span data-ttu-id="0b471-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b471-105">Properties</span></span>

<!-- Add descriptions for the properties. -->
| <span data-ttu-id="0b471-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b471-106">Property</span></span>     | <span data-ttu-id="0b471-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b471-107">Type</span></span>   |<span data-ttu-id="0b471-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b471-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b471-109">código</span><span class="sxs-lookup"><span data-stu-id="0b471-109">code</span></span>|<span data-ttu-id="0b471-110">String</span><span class="sxs-lookup"><span data-stu-id="0b471-110">String</span></span>||
|<span data-ttu-id="0b471-111">mensagem</span><span class="sxs-lookup"><span data-stu-id="0b471-111">message</span></span>|<span data-ttu-id="0b471-112">String</span><span class="sxs-lookup"><span data-stu-id="0b471-112">String</span></span>||
|<span data-ttu-id="0b471-113">tenantActionable</span><span class="sxs-lookup"><span data-stu-id="0b471-113">tenantActionable</span></span>|<span data-ttu-id="0b471-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="0b471-114">Boolean</span></span>||

## <a name="json-representation"></a><span data-ttu-id="0b471-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b471-115">JSON representation</span></span>

<span data-ttu-id="0b471-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0b471-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationError"
}-->

```json
{
  "code": "String",
  "message": "String",
  "tenantActionable": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
