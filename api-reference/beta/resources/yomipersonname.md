---
title: tipo de recurso yomiPersonName
description: tipo de recurso yomiPersonName
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 8117dd71947fea41508ccbe7d50d49a4f78b335d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939765"
---
# <a name="yomipersonname-resource-type"></a><span data-ttu-id="0a313-103">tipo de recurso yomiPersonName</span><span class="sxs-lookup"><span data-stu-id="0a313-103">yomiPersonName resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a313-104">Fornece um mecanismo para que um usuário armazene informações sobre como pronunciar um nome para alto-falantes não nativos do idioma no qual o recurso [PersonName](personname.md) é representado.</span><span class="sxs-lookup"><span data-stu-id="0a313-104">Provides a mechanism for a user to store information about how to pronounce a name for non-native speakers of the language that the [personName](personname.md) resource is represented in.</span></span>

## <a name="properties"></a><span data-ttu-id="0a313-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0a313-105">Properties</span></span>

| <span data-ttu-id="0a313-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0a313-106">Property</span></span>     | <span data-ttu-id="0a313-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a313-107">Type</span></span>        | <span data-ttu-id="0a313-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a313-108">Description</span></span>                                             |
|:-------------|:------------|:--------------------------------------------------------|
|<span data-ttu-id="0a313-109">displayName</span><span class="sxs-lookup"><span data-stu-id="0a313-109">displayName</span></span>   |<span data-ttu-id="0a313-110">String</span><span class="sxs-lookup"><span data-stu-id="0a313-110">String</span></span>       | <span data-ttu-id="0a313-111">Composto de guias de pronúncia de nome e de sobrenome.</span><span class="sxs-lookup"><span data-stu-id="0a313-111">Composite of first and last name pronunciation guides.</span></span>  |
|<span data-ttu-id="0a313-112">primeiro</span><span class="sxs-lookup"><span data-stu-id="0a313-112">first</span></span>         |<span data-ttu-id="0a313-113">String</span><span class="sxs-lookup"><span data-stu-id="0a313-113">String</span></span>       | <span data-ttu-id="0a313-114">Guia de pronúncia para o primeiro nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="0a313-114">Pronunciation guide for the first name of the user.</span></span>     |
|<span data-ttu-id="0a313-115">durar</span><span class="sxs-lookup"><span data-stu-id="0a313-115">last</span></span>          |<span data-ttu-id="0a313-116">String</span><span class="sxs-lookup"><span data-stu-id="0a313-116">String</span></span>       | <span data-ttu-id="0a313-117">Guia de pronúncia para o sobrenome do usuário.</span><span class="sxs-lookup"><span data-stu-id="0a313-117">Pronunciation guide for the last name of the user.</span></span>      |
|<span data-ttu-id="0a313-118">Virgem</span><span class="sxs-lookup"><span data-stu-id="0a313-118">maiden</span></span>        |<span data-ttu-id="0a313-119">String</span><span class="sxs-lookup"><span data-stu-id="0a313-119">String</span></span>       | <span data-ttu-id="0a313-120">Guia de pronúncia para o nome de solteira do usuário.</span><span class="sxs-lookup"><span data-stu-id="0a313-120">Pronunciation guide for the maiden name of the user.</span></span>    |
|<span data-ttu-id="0a313-121">middleware</span><span class="sxs-lookup"><span data-stu-id="0a313-121">middle</span></span>        |<span data-ttu-id="0a313-122">String</span><span class="sxs-lookup"><span data-stu-id="0a313-122">String</span></span>       | <span data-ttu-id="0a313-123">Guia de pronúncia para o nome do meio do usuário.</span><span class="sxs-lookup"><span data-stu-id="0a313-123">Pronunciation guide for the middle name of the user.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="0a313-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0a313-124">JSON representation</span></span>

<span data-ttu-id="0a313-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0a313-125">The following is a JSON representation of the resource.</span></span>

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
