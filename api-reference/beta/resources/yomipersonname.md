---
title: tipo de recurso yomiPersonName
description: tipo de recurso yomiPersonName
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 6e112d97f67b260c19de9fe0ab104e9dc1ed1d74
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810332"
---
# <a name="yomipersonname-resource-type"></a><span data-ttu-id="92868-103">tipo de recurso yomiPersonName</span><span class="sxs-lookup"><span data-stu-id="92868-103">yomiPersonName resource type</span></span>

<span data-ttu-id="92868-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92868-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92868-105">Fornece um mecanismo para que um usuário armazene informações sobre como pronunciar um nome para alto-falantes não nativos do idioma no qual o recurso [PersonName](personname.md) é representado.</span><span class="sxs-lookup"><span data-stu-id="92868-105">Provides a mechanism for a user to store information about how to pronounce a name for non-native speakers of the language that the [personName](personname.md) resource is represented in.</span></span>

## <a name="properties"></a><span data-ttu-id="92868-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="92868-106">Properties</span></span>

| <span data-ttu-id="92868-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92868-107">Property</span></span>     | <span data-ttu-id="92868-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="92868-108">Type</span></span>        | <span data-ttu-id="92868-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="92868-109">Description</span></span>                                             |
|:-------------|:------------|:--------------------------------------------------------|
|<span data-ttu-id="92868-110">displayName</span><span class="sxs-lookup"><span data-stu-id="92868-110">displayName</span></span>   |<span data-ttu-id="92868-111">String</span><span class="sxs-lookup"><span data-stu-id="92868-111">String</span></span>       | <span data-ttu-id="92868-112">Composto de guias de pronúncia de nome e de sobrenome.</span><span class="sxs-lookup"><span data-stu-id="92868-112">Composite of first and last name pronunciation guides.</span></span>  |
|<span data-ttu-id="92868-113">primeiro</span><span class="sxs-lookup"><span data-stu-id="92868-113">first</span></span>         |<span data-ttu-id="92868-114">String</span><span class="sxs-lookup"><span data-stu-id="92868-114">String</span></span>       | <span data-ttu-id="92868-115">Guia de pronúncia para o primeiro nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="92868-115">Pronunciation guide for the first name of the user.</span></span>     |
|<span data-ttu-id="92868-116">durar</span><span class="sxs-lookup"><span data-stu-id="92868-116">last</span></span>          |<span data-ttu-id="92868-117">String</span><span class="sxs-lookup"><span data-stu-id="92868-117">String</span></span>       | <span data-ttu-id="92868-118">Guia de pronúncia para o sobrenome do usuário.</span><span class="sxs-lookup"><span data-stu-id="92868-118">Pronunciation guide for the last name of the user.</span></span>      |
|<span data-ttu-id="92868-119">Virgem</span><span class="sxs-lookup"><span data-stu-id="92868-119">maiden</span></span>        |<span data-ttu-id="92868-120">String</span><span class="sxs-lookup"><span data-stu-id="92868-120">String</span></span>       | <span data-ttu-id="92868-121">Guia de pronúncia para o nome de solteira do usuário.</span><span class="sxs-lookup"><span data-stu-id="92868-121">Pronunciation guide for the maiden name of the user.</span></span>    |
|<span data-ttu-id="92868-122">middleware</span><span class="sxs-lookup"><span data-stu-id="92868-122">middle</span></span>        |<span data-ttu-id="92868-123">String</span><span class="sxs-lookup"><span data-stu-id="92868-123">String</span></span>       | <span data-ttu-id="92868-124">Guia de pronúncia para o nome do meio do usuário.</span><span class="sxs-lookup"><span data-stu-id="92868-124">Pronunciation guide for the middle name of the user.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="92868-125">Relações</span><span class="sxs-lookup"><span data-stu-id="92868-125">Relationships</span></span>

<span data-ttu-id="92868-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="92868-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="92868-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="92868-127">JSON representation</span></span>

<span data-ttu-id="92868-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="92868-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yomiPersonName"
}
-->

``` json

{
  "displayName": "String",
  "first": "String",
  "maiden": "String",
  "middle": "String",
  "last": "String"
}
```
