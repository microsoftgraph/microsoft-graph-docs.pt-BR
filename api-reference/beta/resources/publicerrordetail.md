---
title: tipo de recurso publicErrorDetail
description: Representa os detalhes de um erro.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8620d19d1cd540f7ed523a392e71c304cbbf1774
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659398"
---
# <a name="publicerrordetail-resource-type"></a><span data-ttu-id="2f0e3-103">tipo de recurso publicErrorDetail</span><span class="sxs-lookup"><span data-stu-id="2f0e3-103">publicErrorDetail resource type</span></span>

<span data-ttu-id="2f0e3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f0e3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2f0e3-105">Representa os detalhes de [publicError](../resources/publicerror.md) ou [publicInnerError](../resources/publicinnererror.md).</span><span class="sxs-lookup"><span data-stu-id="2f0e3-105">Represents the details of [publicError](../resources/publicerror.md) or [publicInnerError](../resources/publicinnererror.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2f0e3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2f0e3-106">Properties</span></span>
|<span data-ttu-id="2f0e3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f0e3-107">Property</span></span>|<span data-ttu-id="2f0e3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f0e3-108">Type</span></span>|<span data-ttu-id="2f0e3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f0e3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f0e3-110">código</span><span class="sxs-lookup"><span data-stu-id="2f0e3-110">code</span></span>|<span data-ttu-id="2f0e3-111">String</span><span class="sxs-lookup"><span data-stu-id="2f0e3-111">String</span></span>|<span data-ttu-id="2f0e3-112">O código de erro.</span><span class="sxs-lookup"><span data-stu-id="2f0e3-112">The error code.</span></span>|
|<span data-ttu-id="2f0e3-113">mensagem</span><span class="sxs-lookup"><span data-stu-id="2f0e3-113">message</span></span>|<span data-ttu-id="2f0e3-114">String</span><span class="sxs-lookup"><span data-stu-id="2f0e3-114">String</span></span>|<span data-ttu-id="2f0e3-115">A mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="2f0e3-115">The error message.</span></span>|
|<span data-ttu-id="2f0e3-116">destino</span><span class="sxs-lookup"><span data-stu-id="2f0e3-116">target</span></span>|<span data-ttu-id="2f0e3-117">String</span><span class="sxs-lookup"><span data-stu-id="2f0e3-117">String</span></span>|<span data-ttu-id="2f0e3-118">O destino do erro.</span><span class="sxs-lookup"><span data-stu-id="2f0e3-118">The target of the error.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f0e3-119">Relações</span><span class="sxs-lookup"><span data-stu-id="2f0e3-119">Relationships</span></span>
<span data-ttu-id="2f0e3-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2f0e3-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f0e3-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2f0e3-121">JSON representation</span></span>
<span data-ttu-id="2f0e3-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2f0e3-122">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.publicErrorDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.publicErrorDetail",
  "code": "String",
  "message": "String",
  "target": "String"
}
```

