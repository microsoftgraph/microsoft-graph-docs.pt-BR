---
title: pendingContentUpdate
description: O recurso pendingContentUpdate indica que uma operação que pode afetar o conteúdo binário do driveItem está aguardando a conclusão.
localization_priority: Normal
author: learafa
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: b1a197ae60dc8bb60533d567c6472a65988c3962
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863800"
---
# <a name="pendingcontentupdate-resource-type"></a><span data-ttu-id="ea1cf-103">tipo de recurso pendingContentUpdate</span><span class="sxs-lookup"><span data-stu-id="ea1cf-103">pendingContentUpdate resource type</span></span>

<span data-ttu-id="ea1cf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea1cf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ea1cf-105">Indica que uma operação que pode afetar o conteúdo binário do **driveItem** está aguardando a conclusão.</span><span class="sxs-lookup"><span data-stu-id="ea1cf-105">Indicates that an operation that might affect the binary content of the **driveItem** is pending completion.</span></span>

## <a name="properties"></a><span data-ttu-id="ea1cf-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea1cf-106">Properties</span></span>

| <span data-ttu-id="ea1cf-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea1cf-107">Property</span></span>     | <span data-ttu-id="ea1cf-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea1cf-108">Type</span></span>         | <span data-ttu-id="ea1cf-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea1cf-109">Description</span></span> |
|:-------------|:-------------|:------------|
|<span data-ttu-id="ea1cf-110">**queuedDateTime**</span><span class="sxs-lookup"><span data-stu-id="ea1cf-110">**queuedDateTime**</span></span>|<span data-ttu-id="ea1cf-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea1cf-111">DateTimeOffset</span></span>|<span data-ttu-id="ea1cf-112">Data e hora em que a operação binária pendente foi enfileirada no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ea1cf-112">Date and time the pending binary operation was queued in UTC time.</span></span> <span data-ttu-id="ea1cf-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea1cf-113">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ea1cf-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea1cf-114">JSON representation</span></span>

<span data-ttu-id="ea1cf-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ea1cf-115">The following is a JSON representation of the resource.</span></span>

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
