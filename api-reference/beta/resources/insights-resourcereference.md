---
title: tipo de recurso de resourceReference
description: Tipo complexo que contém propriedades de ideias.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 23a05a362ea57c84dceecbd9523c2620edc21fbf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966283"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="6549a-103">tipo de recurso de resourceReference</span><span class="sxs-lookup"><span data-stu-id="6549a-103">resourceReference resource type</span></span>

> <span data-ttu-id="6549a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6549a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6549a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6549a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6549a-106">Tipo complexo que contém propriedades de [ideias](insights.md).</span><span class="sxs-lookup"><span data-stu-id="6549a-106">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="6549a-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6549a-107">JSON representation</span></span>

<span data-ttu-id="6549a-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="6549a-108">Here is a JSON representation of the resource</span></span>

```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="6549a-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6549a-109">Properties</span></span>

| <span data-ttu-id="6549a-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6549a-110">Property</span></span>      | <span data-ttu-id="6549a-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="6549a-111">Type</span></span>      | <span data-ttu-id="6549a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="6549a-112">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="6549a-113">webUrl</span><span class="sxs-lookup"><span data-stu-id="6549a-113">webUrl</span></span>        | <span data-ttu-id="6549a-114">String</span><span class="sxs-lookup"><span data-stu-id="6549a-114">String</span></span>    | <span data-ttu-id="6549a-115">Uma URL, levando a item referenciado.</span><span class="sxs-lookup"><span data-stu-id="6549a-115">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="6549a-116">id</span><span class="sxs-lookup"><span data-stu-id="6549a-116">id</span></span>            | <span data-ttu-id="6549a-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6549a-117">String</span></span>    | <span data-ttu-id="6549a-118">Identificador exclusivo do item.</span><span class="sxs-lookup"><span data-stu-id="6549a-118">The item's unique identifier.</span></span>           |
| <span data-ttu-id="6549a-119">type</span><span class="sxs-lookup"><span data-stu-id="6549a-119">type</span></span>          | <span data-ttu-id="6549a-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6549a-120">String</span></span>    | <span data-ttu-id="6549a-121">Um valor de cadeia de caracteres que pode ser usado para classificar o item, como "microsoft.graph.driveItem"</span><span class="sxs-lookup"><span data-stu-id="6549a-121">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
