---
title: pendingContentUpdate
description: O recurso pendingContentUpdate indica que uma operação que pode afetar o conteúdo binário do driveItem está aguardando a conclusão.
localization_priority: Normal
author: JeremyKelley
ms.date: 08/06/2019
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7862d8da186448d08d6dfd5691ae83e29bd57a5e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521973"
---
# <a name="pendingcontentupdate-resource-type"></a><span data-ttu-id="f72a0-103">tipo de recurso pendingContentUpdate</span><span class="sxs-lookup"><span data-stu-id="f72a0-103">pendingContentUpdate resource type</span></span>

<span data-ttu-id="f72a0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f72a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f72a0-105">Indica que uma operação que pode afetar o conteúdo binário do **driveItem** está aguardando a conclusão.</span><span class="sxs-lookup"><span data-stu-id="f72a0-105">Indicates that an operation that might affect the binary content of the **driveItem** is pending completion.</span></span>

## <a name="properties"></a><span data-ttu-id="f72a0-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f72a0-106">Properties</span></span>

| <span data-ttu-id="f72a0-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f72a0-107">Property</span></span>     | <span data-ttu-id="f72a0-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f72a0-108">Type</span></span>         | <span data-ttu-id="f72a0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f72a0-109">Description</span></span> |
|:-------------|:-------------|:------------|
|<span data-ttu-id="f72a0-110">queuedDateTime</span><span class="sxs-lookup"><span data-stu-id="f72a0-110">queuedDateTime</span></span>|<span data-ttu-id="f72a0-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f72a0-111">DateTimeOffset</span></span>|<span data-ttu-id="f72a0-112">Data e hora em que a operação binária pendente foi enfileirada no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f72a0-112">Date and time the pending binary operation was queued in UTC time.</span></span> <span data-ttu-id="f72a0-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f72a0-113">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f72a0-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f72a0-114">JSON representation</span></span>

<span data-ttu-id="f72a0-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f72a0-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.pendingContentUpdate",
  "baseType": null
}-->

```json
{
  "queuedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The pendingContentUpdate resource indicates that an operation that may affect the binary content of the DriveItem is pending completion.",
  "keywords": "pendingoperation,operation,pendingcontentupdate",
  "section": "documentation",
  "tocPath": ""
}-->
