---
title: tipo de recurso yomiPersonName
description: tipo de recurso yomiPersonName
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0a598c4b5e999b03aeb7201c6eae3a230d3160a7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518970"
---
# <a name="yomipersonname-resource-type"></a><span data-ttu-id="0347a-103">tipo de recurso yomiPersonName</span><span class="sxs-lookup"><span data-stu-id="0347a-103">yomiPersonName resource type</span></span>

<span data-ttu-id="0347a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0347a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0347a-105">Fornece um mecanismo para que um usuário armazene informações sobre como pronunciar um nome para alto-falantes não nativos do idioma no qual o recurso [PersonName](personname.md) é representado.</span><span class="sxs-lookup"><span data-stu-id="0347a-105">Provides a mechanism for a user to store information about how to pronounce a name for non-native speakers of the language that the [personName](personname.md) resource is represented in.</span></span>

## <a name="properties"></a><span data-ttu-id="0347a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0347a-106">Properties</span></span>

| <span data-ttu-id="0347a-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0347a-107">Property</span></span>     | <span data-ttu-id="0347a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0347a-108">Type</span></span>        | <span data-ttu-id="0347a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0347a-109">Description</span></span>                                             |
|:-------------|:------------|:--------------------------------------------------------|
|<span data-ttu-id="0347a-110">displayName</span><span class="sxs-lookup"><span data-stu-id="0347a-110">displayName</span></span>   |<span data-ttu-id="0347a-111">String</span><span class="sxs-lookup"><span data-stu-id="0347a-111">String</span></span>       | <span data-ttu-id="0347a-112">Composto de guias de pronúncia de nome e de sobrenome.</span><span class="sxs-lookup"><span data-stu-id="0347a-112">Composite of first and last name pronunciation guides.</span></span>  |
|<span data-ttu-id="0347a-113">primeiro</span><span class="sxs-lookup"><span data-stu-id="0347a-113">first</span></span>         |<span data-ttu-id="0347a-114">String</span><span class="sxs-lookup"><span data-stu-id="0347a-114">String</span></span>       | <span data-ttu-id="0347a-115">Guia de pronúncia para o primeiro nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="0347a-115">Pronunciation guide for the first name of the user.</span></span>     |
|<span data-ttu-id="0347a-116">durar</span><span class="sxs-lookup"><span data-stu-id="0347a-116">last</span></span>          |<span data-ttu-id="0347a-117">String</span><span class="sxs-lookup"><span data-stu-id="0347a-117">String</span></span>       | <span data-ttu-id="0347a-118">Guia de pronúncia para o sobrenome do usuário.</span><span class="sxs-lookup"><span data-stu-id="0347a-118">Pronunciation guide for the last name of the user.</span></span>      |
|<span data-ttu-id="0347a-119">Virgem</span><span class="sxs-lookup"><span data-stu-id="0347a-119">maiden</span></span>        |<span data-ttu-id="0347a-120">String</span><span class="sxs-lookup"><span data-stu-id="0347a-120">String</span></span>       | <span data-ttu-id="0347a-121">Guia de pronúncia para o nome de solteira do usuário.</span><span class="sxs-lookup"><span data-stu-id="0347a-121">Pronunciation guide for the maiden name of the user.</span></span>    |
|<span data-ttu-id="0347a-122">middleware</span><span class="sxs-lookup"><span data-stu-id="0347a-122">middle</span></span>        |<span data-ttu-id="0347a-123">String</span><span class="sxs-lookup"><span data-stu-id="0347a-123">String</span></span>       | <span data-ttu-id="0347a-124">Guia de pronúncia para o nome do meio do usuário.</span><span class="sxs-lookup"><span data-stu-id="0347a-124">Pronunciation guide for the middle name of the user.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="0347a-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0347a-125">JSON representation</span></span>

<span data-ttu-id="0347a-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0347a-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.yomiPersonName",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "first": "String",
  "last": "String",
  "maiden": "String",
  "middle": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "yomiPersonName resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
