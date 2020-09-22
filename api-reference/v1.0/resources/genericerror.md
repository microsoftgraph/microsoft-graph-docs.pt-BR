---
title: tipo de recurso genericError
description: Um erro de uso geral.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: b6601dc0975b12e0f21ecea9fa6e9e3063334ab1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018211"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="f0a5b-103">tipo de recurso genericError</span><span class="sxs-lookup"><span data-stu-id="f0a5b-103">genericError resource type</span></span>

<span data-ttu-id="f0a5b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0a5b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f0a5b-105">Um erro de uso geral.</span><span class="sxs-lookup"><span data-stu-id="f0a5b-105">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="f0a5b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f0a5b-106">Properties</span></span>

| <span data-ttu-id="f0a5b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0a5b-107">Property</span></span> | <span data-ttu-id="f0a5b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0a5b-108">Type</span></span> | <span data-ttu-id="f0a5b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0a5b-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="f0a5b-110">mensagem</span><span class="sxs-lookup"><span data-stu-id="f0a5b-110">message</span></span> | <span data-ttu-id="f0a5b-111">String</span><span class="sxs-lookup"><span data-stu-id="f0a5b-111">String</span></span> | <span data-ttu-id="f0a5b-112">A mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="f0a5b-112">The error message.</span></span> |
| <span data-ttu-id="f0a5b-113">código</span><span class="sxs-lookup"><span data-stu-id="f0a5b-113">code</span></span> | <span data-ttu-id="f0a5b-114">String</span><span class="sxs-lookup"><span data-stu-id="f0a5b-114">String</span></span> | <span data-ttu-id="f0a5b-115">O código de erro.</span><span class="sxs-lookup"><span data-stu-id="f0a5b-115">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f0a5b-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f0a5b-116">JSON representation</span></span>

<span data-ttu-id="f0a5b-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f0a5b-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.genericError"
}-->

```json
{
  "message": "String",
  "code": "String"
}
```

