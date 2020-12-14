---
title: tipo de recurso publicError
description: Representa um erro genérico e seus detalhes.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: AkJo
ms.openlocfilehash: 65a75b6eb2756b92f9da6386390fae3b254f818b
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660083"
---
# <a name="publicerror-resource-type"></a><span data-ttu-id="197bc-103">tipo de recurso publicError</span><span class="sxs-lookup"><span data-stu-id="197bc-103">publicError resource type</span></span>

<span data-ttu-id="197bc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="197bc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="197bc-105">Representa um erro genérico e seus detalhes.</span><span class="sxs-lookup"><span data-stu-id="197bc-105">Represents a generic error and its details.</span></span>

## <a name="properties"></a><span data-ttu-id="197bc-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="197bc-106">Properties</span></span>
|<span data-ttu-id="197bc-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="197bc-107">Property</span></span>|<span data-ttu-id="197bc-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="197bc-108">Type</span></span>|<span data-ttu-id="197bc-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="197bc-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="197bc-110">código</span><span class="sxs-lookup"><span data-stu-id="197bc-110">code</span></span>|<span data-ttu-id="197bc-111">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="197bc-111">string</span></span>| <span data-ttu-id="197bc-112">Representa o código de erro.</span><span class="sxs-lookup"><span data-stu-id="197bc-112">Represents the error code.</span></span>
|<span data-ttu-id="197bc-113">detalhes</span><span class="sxs-lookup"><span data-stu-id="197bc-113">details</span></span>|<span data-ttu-id="197bc-114">coleção [publicErrorDetail](publicerrordetail.md)</span><span class="sxs-lookup"><span data-stu-id="197bc-114">[publicErrorDetail](publicerrordetail.md) collection</span></span>|<span data-ttu-id="197bc-115">Detalhes do erro.</span><span class="sxs-lookup"><span data-stu-id="197bc-115">Details of the error.</span></span>|
|<span data-ttu-id="197bc-116">innerError</span><span class="sxs-lookup"><span data-stu-id="197bc-116">innerError</span></span>|[<span data-ttu-id="197bc-117">publicInnerError</span><span class="sxs-lookup"><span data-stu-id="197bc-117">publicInnerError</span></span>](publicinnererror.md)|<span data-ttu-id="197bc-118">Detalhes do erro interno.</span><span class="sxs-lookup"><span data-stu-id="197bc-118">Details of the inner error.</span></span>|
|<span data-ttu-id="197bc-119">mensagem</span><span class="sxs-lookup"><span data-stu-id="197bc-119">message</span></span>|<span data-ttu-id="197bc-120">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="197bc-120">string</span></span>| <span data-ttu-id="197bc-121">Uma mensagem não localizada para o desenvolvedor.</span><span class="sxs-lookup"><span data-stu-id="197bc-121">A non-localized message for the developer.</span></span>
|<span data-ttu-id="197bc-122">destino</span><span class="sxs-lookup"><span data-stu-id="197bc-122">target</span></span>|<span data-ttu-id="197bc-123">String</span><span class="sxs-lookup"><span data-stu-id="197bc-123">String</span></span>|<span data-ttu-id="197bc-124">O destino do erro.</span><span class="sxs-lookup"><span data-stu-id="197bc-124">The target of the error.</span></span>|

## <a name="relationships"></a><span data-ttu-id="197bc-125">Relações</span><span class="sxs-lookup"><span data-stu-id="197bc-125">Relationships</span></span>
<span data-ttu-id="197bc-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="197bc-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="197bc-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="197bc-127">JSON representation</span></span>
<span data-ttu-id="197bc-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="197bc-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.publicError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.publicError",
  "code": "String",
  "message": "String",
  "target": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.publicErrorDetail"
    }
  ],
  "innerError": {
    "@odata.type": "microsoft.graph.publicInnerError"
  }
}
```

