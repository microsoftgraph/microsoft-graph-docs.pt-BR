---
title: tipo de recurso synchronizationError
description: Representa um erro que ocorreu durante o processo de sincronização.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5a754b03379d1e40ba7310283a0efdd94ff30631
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520076"
---
# <a name="synchronizationerror-resource-type"></a><span data-ttu-id="64c54-103">tipo de recurso synchronizationError</span><span class="sxs-lookup"><span data-stu-id="64c54-103">synchronizationError resource type</span></span>

<span data-ttu-id="64c54-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="64c54-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64c54-105">Representa um erro que ocorreu durante o processo de sincronização.</span><span class="sxs-lookup"><span data-stu-id="64c54-105">Represents an error that occurred during the synchronization process.</span></span>

## <a name="properties"></a><span data-ttu-id="64c54-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="64c54-106">Properties</span></span>

<!-- Add descriptions for the properties. -->
| <span data-ttu-id="64c54-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64c54-107">Property</span></span>     | <span data-ttu-id="64c54-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="64c54-108">Type</span></span>   |<span data-ttu-id="64c54-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="64c54-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64c54-110">código</span><span class="sxs-lookup"><span data-stu-id="64c54-110">code</span></span>|<span data-ttu-id="64c54-111">String</span><span class="sxs-lookup"><span data-stu-id="64c54-111">String</span></span>||
|<span data-ttu-id="64c54-112">mensagem</span><span class="sxs-lookup"><span data-stu-id="64c54-112">message</span></span>|<span data-ttu-id="64c54-113">String</span><span class="sxs-lookup"><span data-stu-id="64c54-113">String</span></span>||
|<span data-ttu-id="64c54-114">tenantActionable</span><span class="sxs-lookup"><span data-stu-id="64c54-114">tenantActionable</span></span>|<span data-ttu-id="64c54-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="64c54-115">Boolean</span></span>||

## <a name="json-representation"></a><span data-ttu-id="64c54-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="64c54-116">JSON representation</span></span>

<span data-ttu-id="64c54-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="64c54-117">The following is a JSON representation of the resource.</span></span>

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
