---
title: tipo de recurso publicInnerError
description: Representa os detalhes internos de um erro.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e8380e8836076687a2d6ab3e8a0a4a53b8bd6964
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658322"
---
# <a name="publicinnererror-resource-type"></a><span data-ttu-id="09407-103">tipo de recurso publicInnerError</span><span class="sxs-lookup"><span data-stu-id="09407-103">publicInnerError resource type</span></span>

<span data-ttu-id="09407-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09407-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="09407-105">Representa os detalhes internos de um [publicError](../resources/publicerrordetail.md).</span><span class="sxs-lookup"><span data-stu-id="09407-105">Represents the inner details of a [publicError](../resources/publicerrordetail.md).</span></span> 
## <a name="properties"></a><span data-ttu-id="09407-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="09407-106">Properties</span></span>
|<span data-ttu-id="09407-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09407-107">Property</span></span>|<span data-ttu-id="09407-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="09407-108">Type</span></span>|<span data-ttu-id="09407-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="09407-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09407-110">código</span><span class="sxs-lookup"><span data-stu-id="09407-110">code</span></span>|<span data-ttu-id="09407-111">String</span><span class="sxs-lookup"><span data-stu-id="09407-111">String</span></span>|<span data-ttu-id="09407-112">O código de erro.</span><span class="sxs-lookup"><span data-stu-id="09407-112">The error code.</span></span>|
|<span data-ttu-id="09407-113">detalhes</span><span class="sxs-lookup"><span data-stu-id="09407-113">details</span></span>|<span data-ttu-id="09407-114">coleção [publicErrorDetail](../resources/publicerrordetail.md)</span><span class="sxs-lookup"><span data-stu-id="09407-114">[publicErrorDetail](../resources/publicerrordetail.md) collection</span></span>|<span data-ttu-id="09407-115">Uma coleção de detalhes de erro.</span><span class="sxs-lookup"><span data-stu-id="09407-115">A collection of error details.</span></span>|
|<span data-ttu-id="09407-116">mensagem</span><span class="sxs-lookup"><span data-stu-id="09407-116">message</span></span>|<span data-ttu-id="09407-117">String</span><span class="sxs-lookup"><span data-stu-id="09407-117">String</span></span>|<span data-ttu-id="09407-118">A mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="09407-118">The error message.</span></span>|
|<span data-ttu-id="09407-119">destino</span><span class="sxs-lookup"><span data-stu-id="09407-119">target</span></span>|<span data-ttu-id="09407-120">String</span><span class="sxs-lookup"><span data-stu-id="09407-120">String</span></span>|<span data-ttu-id="09407-121">O destino do erro.</span><span class="sxs-lookup"><span data-stu-id="09407-121">The target of the error.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09407-122">Relações</span><span class="sxs-lookup"><span data-stu-id="09407-122">Relationships</span></span>
<span data-ttu-id="09407-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="09407-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="09407-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="09407-124">JSON representation</span></span>
<span data-ttu-id="09407-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="09407-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.publicInnerError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.publicInnerError",
  "code": "String",
  "message": "String",
  "target": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.publicErrorDetail"
    }
  ]
}
```

