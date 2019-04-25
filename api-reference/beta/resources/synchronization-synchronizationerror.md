---
title: tipo de recurso synchronizationError
description: Representa um erro que ocorreu durante o processo de sincronização.
localization_priority: Normal
ms.openlocfilehash: f37dca5b65a67eb36b2b6a130eee8feb692cd271
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525975"
---
# <a name="synchronizationerror-resource-type"></a><span data-ttu-id="209c1-103">tipo de recurso synchronizationError</span><span class="sxs-lookup"><span data-stu-id="209c1-103">synchronizationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="209c1-104">Representa um erro que ocorreu durante o processo de sincronização.</span><span class="sxs-lookup"><span data-stu-id="209c1-104">Represents an error that occurred during the synchronization process.</span></span>

## <a name="properties"></a><span data-ttu-id="209c1-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="209c1-105">Properties</span></span>

<!-- Add descriptions for the properties. -->
| <span data-ttu-id="209c1-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="209c1-106">Property</span></span>     | <span data-ttu-id="209c1-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="209c1-107">Type</span></span>   |<span data-ttu-id="209c1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="209c1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="209c1-109">código</span><span class="sxs-lookup"><span data-stu-id="209c1-109">code</span></span>|<span data-ttu-id="209c1-110">String</span><span class="sxs-lookup"><span data-stu-id="209c1-110">String</span></span>||
|<span data-ttu-id="209c1-111">mensagem</span><span class="sxs-lookup"><span data-stu-id="209c1-111">message</span></span>|<span data-ttu-id="209c1-112">String</span><span class="sxs-lookup"><span data-stu-id="209c1-112">String</span></span>||
|<span data-ttu-id="209c1-113">tenantActionable</span><span class="sxs-lookup"><span data-stu-id="209c1-113">tenantActionable</span></span>|<span data-ttu-id="209c1-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="209c1-114">Boolean</span></span>||

## <a name="json-representation"></a><span data-ttu-id="209c1-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="209c1-115">JSON representation</span></span>

<span data-ttu-id="209c1-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="209c1-116">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
