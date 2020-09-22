---
title: tipo de recurso useranalytics
description: As configurações do usuário e as estatísticas de atividade.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: ac4024fff534bd89e369f1f8048ca274ccfd157a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057896"
---
# <a name="useranalytics-resource-type"></a><span data-ttu-id="2568e-103">tipo de recurso useranalytics</span><span class="sxs-lookup"><span data-stu-id="2568e-103">userAnalytics resource type</span></span>

<span data-ttu-id="2568e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2568e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2568e-105">As configurações do usuário e as estatísticas de atividade.</span><span class="sxs-lookup"><span data-stu-id="2568e-105">The user's settings and activity statistics.</span></span>

## <a name="methods"></a><span data-ttu-id="2568e-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="2568e-106">Methods</span></span>

| <span data-ttu-id="2568e-107">Método</span><span class="sxs-lookup"><span data-stu-id="2568e-107">Method</span></span>       | <span data-ttu-id="2568e-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2568e-108">Return Type</span></span> | <span data-ttu-id="2568e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2568e-109">Description</span></span> |
|:-------------|:------------|:------------|
[<span data-ttu-id="2568e-110">Obter configurações</span><span class="sxs-lookup"><span data-stu-id="2568e-110">Get settings</span></span>](../api/useranalytics-get-settings.md) | [<span data-ttu-id="2568e-111">configurações</span><span class="sxs-lookup"><span data-stu-id="2568e-111">settings</span></span>](settings.md) | <span data-ttu-id="2568e-112">Obter as configurações do usuário para usar a API de análise.</span><span class="sxs-lookup"><span data-stu-id="2568e-112">Get the user's settings for using the analytics API.</span></span>|

## <a name="properties"></a><span data-ttu-id="2568e-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2568e-113">Properties</span></span>

| <span data-ttu-id="2568e-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2568e-114">Property</span></span>     | <span data-ttu-id="2568e-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="2568e-115">Type</span></span>        | <span data-ttu-id="2568e-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="2568e-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2568e-117">configurações</span><span class="sxs-lookup"><span data-stu-id="2568e-117">settings</span></span>|[<span data-ttu-id="2568e-118">configurações</span><span class="sxs-lookup"><span data-stu-id="2568e-118">settings</span></span>](settings.md)|<span data-ttu-id="2568e-119">As configurações atuais de um usuário para usar a API de análise.</span><span class="sxs-lookup"><span data-stu-id="2568e-119">The current settings for a user to use the analytics API.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2568e-120">Relações</span><span class="sxs-lookup"><span data-stu-id="2568e-120">Relationships</span></span>

| <span data-ttu-id="2568e-121">Relação</span><span class="sxs-lookup"><span data-stu-id="2568e-121">Relationship</span></span> | <span data-ttu-id="2568e-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="2568e-122">Type</span></span>        | <span data-ttu-id="2568e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2568e-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2568e-124">activityStatistics</span><span class="sxs-lookup"><span data-stu-id="2568e-124">activityStatistics</span></span>|<span data-ttu-id="2568e-125">coleção [activityStatistics](activitystatistics.md)</span><span class="sxs-lookup"><span data-stu-id="2568e-125">[activityStatistics](activitystatistics.md) collection</span></span>| <span data-ttu-id="2568e-126">O conjunto de atividades de trabalho que um usuário gastou enquanto está fora do horário de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2568e-126">The collection of work activities that a user spent time on during and outside of working hours.</span></span> <span data-ttu-id="2568e-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2568e-127">Read-only.</span></span> <span data-ttu-id="2568e-128">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2568e-128">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2568e-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2568e-129">JSON representation</span></span>

<span data-ttu-id="2568e-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2568e-130">The following is a JSON representation of the resource.</span></span>

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


