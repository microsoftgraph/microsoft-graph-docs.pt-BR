---
title: Tipo de recurso publicErrorDetail
description: Representa os detalhes de um erro.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ac86f2aa50e1447702099f3c73f31979b6e6eb16
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467235"
---
# <a name="publicerrordetail-resource-type"></a><span data-ttu-id="230e0-103">Tipo de recurso publicErrorDetail</span><span class="sxs-lookup"><span data-stu-id="230e0-103">publicErrorDetail resource type</span></span>

<span data-ttu-id="230e0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="230e0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="230e0-105">Representa os detalhes [de publicError](../resources/publicerror.md) ou [publicInnerError](../resources/publicinnererror.md).</span><span class="sxs-lookup"><span data-stu-id="230e0-105">Represents the details of [publicError](../resources/publicerror.md) or [publicInnerError](../resources/publicinnererror.md).</span></span>

## <a name="properties"></a><span data-ttu-id="230e0-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="230e0-106">Properties</span></span>
|<span data-ttu-id="230e0-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="230e0-107">Property</span></span>|<span data-ttu-id="230e0-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="230e0-108">Type</span></span>|<span data-ttu-id="230e0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="230e0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="230e0-110">código</span><span class="sxs-lookup"><span data-stu-id="230e0-110">code</span></span>|<span data-ttu-id="230e0-111">String</span><span class="sxs-lookup"><span data-stu-id="230e0-111">String</span></span>|<span data-ttu-id="230e0-112">O código de erro.</span><span class="sxs-lookup"><span data-stu-id="230e0-112">The error code.</span></span>|
|<span data-ttu-id="230e0-113">mensagem</span><span class="sxs-lookup"><span data-stu-id="230e0-113">message</span></span>|<span data-ttu-id="230e0-114">String</span><span class="sxs-lookup"><span data-stu-id="230e0-114">String</span></span>|<span data-ttu-id="230e0-115">A mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="230e0-115">The error message.</span></span>|
|<span data-ttu-id="230e0-116">destino</span><span class="sxs-lookup"><span data-stu-id="230e0-116">target</span></span>|<span data-ttu-id="230e0-117">String</span><span class="sxs-lookup"><span data-stu-id="230e0-117">String</span></span>|<span data-ttu-id="230e0-118">O destino do erro.</span><span class="sxs-lookup"><span data-stu-id="230e0-118">The target of the error.</span></span>|

## <a name="relationships"></a><span data-ttu-id="230e0-119">Relações</span><span class="sxs-lookup"><span data-stu-id="230e0-119">Relationships</span></span>
<span data-ttu-id="230e0-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="230e0-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="230e0-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="230e0-121">JSON representation</span></span>
<span data-ttu-id="230e0-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="230e0-122">The following is a JSON representation of the resource.</span></span>
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
