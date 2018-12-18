---
title: tipo de recurso de resourceReference
description: Tipo complexo que contém propriedades de ideias.
author: simonhult
ms.openlocfilehash: 2f1a44412eebbb7a74895c12db9a07696d6ee409
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27363617"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="c57b1-103">tipo de recurso de resourceReference</span><span class="sxs-lookup"><span data-stu-id="c57b1-103">resourceReference resource type</span></span>

> <span data-ttu-id="c57b1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c57b1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c57b1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c57b1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c57b1-106">Tipo complexo que contém propriedades de [ideias](insights.md).</span><span class="sxs-lookup"><span data-stu-id="c57b1-106">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="c57b1-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c57b1-107">JSON representation</span></span>

<span data-ttu-id="c57b1-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="c57b1-108">Here is a JSON representation of the resource</span></span>

```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="c57b1-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c57b1-109">Properties</span></span>

| <span data-ttu-id="c57b1-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c57b1-110">Property</span></span>      | <span data-ttu-id="c57b1-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c57b1-111">Type</span></span>      | <span data-ttu-id="c57b1-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c57b1-112">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="c57b1-113">webUrl</span><span class="sxs-lookup"><span data-stu-id="c57b1-113">webUrl</span></span>        | <span data-ttu-id="c57b1-114">String</span><span class="sxs-lookup"><span data-stu-id="c57b1-114">String</span></span>    | <span data-ttu-id="c57b1-115">Uma URL, levando a item referenciado.</span><span class="sxs-lookup"><span data-stu-id="c57b1-115">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="c57b1-116">id</span><span class="sxs-lookup"><span data-stu-id="c57b1-116">id</span></span>            | <span data-ttu-id="c57b1-117">String</span><span class="sxs-lookup"><span data-stu-id="c57b1-117">String</span></span>    | <span data-ttu-id="c57b1-118">Identificador exclusivo do item.</span><span class="sxs-lookup"><span data-stu-id="c57b1-118">The item's unique identifier.</span></span>           |
| <span data-ttu-id="c57b1-119">type</span><span class="sxs-lookup"><span data-stu-id="c57b1-119">type</span></span>          | <span data-ttu-id="c57b1-120">String</span><span class="sxs-lookup"><span data-stu-id="c57b1-120">String</span></span>    | <span data-ttu-id="c57b1-121">Um valor de cadeia de caracteres que pode ser usado para classificar o item, como "microsoft.graph.driveItem"</span><span class="sxs-lookup"><span data-stu-id="c57b1-121">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |