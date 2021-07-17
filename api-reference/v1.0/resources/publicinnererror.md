---
title: Tipo de recurso publicInnerError
description: Representa os detalhes internos de um erro.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f089c120ac4ba1307f0b0ffa2f08f8578613eaa1
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467234"
---
# <a name="publicinnererror-resource-type"></a><span data-ttu-id="6ff57-103">Tipo de recurso publicInnerError</span><span class="sxs-lookup"><span data-stu-id="6ff57-103">publicInnerError resource type</span></span>

<span data-ttu-id="6ff57-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ff57-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6ff57-105">Representa os detalhes internos de [um publicError](../resources/publicerrordetail.md).</span><span class="sxs-lookup"><span data-stu-id="6ff57-105">Represents the inner details of a [publicError](../resources/publicerrordetail.md).</span></span> 
## <a name="properties"></a><span data-ttu-id="6ff57-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6ff57-106">Properties</span></span>
|<span data-ttu-id="6ff57-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6ff57-107">Property</span></span>|<span data-ttu-id="6ff57-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ff57-108">Type</span></span>|<span data-ttu-id="6ff57-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ff57-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ff57-110">código</span><span class="sxs-lookup"><span data-stu-id="6ff57-110">code</span></span>|<span data-ttu-id="6ff57-111">String</span><span class="sxs-lookup"><span data-stu-id="6ff57-111">String</span></span>|<span data-ttu-id="6ff57-112">O código de erro.</span><span class="sxs-lookup"><span data-stu-id="6ff57-112">The error code.</span></span>|
|<span data-ttu-id="6ff57-113">detalhes</span><span class="sxs-lookup"><span data-stu-id="6ff57-113">details</span></span>|<span data-ttu-id="6ff57-114">[Coleção publicErrorDetail](../resources/publicerrordetail.md)</span><span class="sxs-lookup"><span data-stu-id="6ff57-114">[publicErrorDetail](../resources/publicerrordetail.md) collection</span></span>|<span data-ttu-id="6ff57-115">Uma coleção de detalhes de erro.</span><span class="sxs-lookup"><span data-stu-id="6ff57-115">A collection of error details.</span></span>|
|<span data-ttu-id="6ff57-116">mensagem</span><span class="sxs-lookup"><span data-stu-id="6ff57-116">message</span></span>|<span data-ttu-id="6ff57-117">String</span><span class="sxs-lookup"><span data-stu-id="6ff57-117">String</span></span>|<span data-ttu-id="6ff57-118">A mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="6ff57-118">The error message.</span></span>|
|<span data-ttu-id="6ff57-119">destino</span><span class="sxs-lookup"><span data-stu-id="6ff57-119">target</span></span>|<span data-ttu-id="6ff57-120">String</span><span class="sxs-lookup"><span data-stu-id="6ff57-120">String</span></span>|<span data-ttu-id="6ff57-121">O destino do erro.</span><span class="sxs-lookup"><span data-stu-id="6ff57-121">The target of the error.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ff57-122">Relações</span><span class="sxs-lookup"><span data-stu-id="6ff57-122">Relationships</span></span>
<span data-ttu-id="6ff57-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6ff57-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ff57-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6ff57-124">JSON representation</span></span>
<span data-ttu-id="6ff57-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6ff57-125">The following is a JSON representation of the resource.</span></span>
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
