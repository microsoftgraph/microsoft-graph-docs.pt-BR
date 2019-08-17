---
title: tipo de recurso useranalytics
description: As configurações do usuário e as estatísticas de atividade.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 51e72d21cfb0e26e46a7d247f4ede59b112893ea
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450691"
---
# <a name="useranalytics-resource-type"></a><span data-ttu-id="c407c-103">tipo de recurso useranalytics</span><span class="sxs-lookup"><span data-stu-id="c407c-103">userAnalytics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c407c-104">As configurações do usuário e as estatísticas de atividade.</span><span class="sxs-lookup"><span data-stu-id="c407c-104">The user's settings and activity statistics.</span></span>

## <a name="methods"></a><span data-ttu-id="c407c-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="c407c-105">Methods</span></span>

| <span data-ttu-id="c407c-106">Método</span><span class="sxs-lookup"><span data-stu-id="c407c-106">Method</span></span>       | <span data-ttu-id="c407c-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c407c-107">Return Type</span></span> | <span data-ttu-id="c407c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c407c-108">Description</span></span> |
|:-------------|:------------|:------------|
[<span data-ttu-id="c407c-109">Obter configurações</span><span class="sxs-lookup"><span data-stu-id="c407c-109">Get settings</span></span>](../api/useranalytics-get-settings.md) | [<span data-ttu-id="c407c-110">configurações</span><span class="sxs-lookup"><span data-stu-id="c407c-110">settings</span></span>](settings.md) | <span data-ttu-id="c407c-111">Obter as configurações do usuário para usar a API de análise.</span><span class="sxs-lookup"><span data-stu-id="c407c-111">Get the user's settings for using the analytics API.</span></span>|

## <a name="properties"></a><span data-ttu-id="c407c-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c407c-112">Properties</span></span>

| <span data-ttu-id="c407c-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c407c-113">Property</span></span>     | <span data-ttu-id="c407c-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="c407c-114">Type</span></span>        | <span data-ttu-id="c407c-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="c407c-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c407c-116">settings</span><span class="sxs-lookup"><span data-stu-id="c407c-116">settings</span></span>|[<span data-ttu-id="c407c-117">configurações</span><span class="sxs-lookup"><span data-stu-id="c407c-117">settings</span></span>](settings.md)|<span data-ttu-id="c407c-118">As configurações atuais de um usuário para usar a API de análise.</span><span class="sxs-lookup"><span data-stu-id="c407c-118">The current settings for a user to use the analytics API.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c407c-119">Relações</span><span class="sxs-lookup"><span data-stu-id="c407c-119">Relationships</span></span>

| <span data-ttu-id="c407c-120">Relação</span><span class="sxs-lookup"><span data-stu-id="c407c-120">Relationship</span></span> | <span data-ttu-id="c407c-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c407c-121">Type</span></span>        | <span data-ttu-id="c407c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c407c-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c407c-123">activityStatistics</span><span class="sxs-lookup"><span data-stu-id="c407c-123">activityStatistics</span></span>|<span data-ttu-id="c407c-124">coleção [activityStatistics](activitystatistics.md)</span><span class="sxs-lookup"><span data-stu-id="c407c-124">[activityStatistics](activitystatistics.md) collection</span></span>| <span data-ttu-id="c407c-125">O conjunto de atividades de trabalho que um usuário gastou enquanto está fora do horário de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c407c-125">The collection of work activities that a user spent time on during and outside of working hours.</span></span> <span data-ttu-id="c407c-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c407c-126">Read-only.</span></span> <span data-ttu-id="c407c-127">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c407c-127">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c407c-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c407c-128">JSON representation</span></span>

<span data-ttu-id="c407c-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c407c-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [
    "activityStatistics"
  ],
  "@odata.type": "microsoft.graph.userAnalytics"
}-->

```json
{
  "id": "string",
  "settings": {"@odata.type": "microsoft.graph.settings"},
  "activityStatistics": [{"@odata.type": "microsoft.graph.activityStatistics"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userAnalytics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
