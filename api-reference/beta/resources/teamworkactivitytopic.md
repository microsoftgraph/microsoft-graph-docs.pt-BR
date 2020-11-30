---
title: tipo de recurso teamworkActivityTopic
description: Representa o tópico de uma notificação de feed de atividade.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a4425053cf41ebfbad139c6d0ea5fc246f0b1391
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377490"
---
# <a name="teamworkactivitytopic-resource-type"></a><span data-ttu-id="40b16-103">tipo de recurso teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="40b16-103">teamworkActivityTopic resource type</span></span>

<span data-ttu-id="40b16-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40b16-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="40b16-105">Representa o tópico de uma notificação de feed de atividade.</span><span class="sxs-lookup"><span data-stu-id="40b16-105">Represents the topic of an activity feed notification.</span></span>

## <a name="properties"></a><span data-ttu-id="40b16-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="40b16-106">Properties</span></span>
|<span data-ttu-id="40b16-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40b16-107">Property</span></span>|<span data-ttu-id="40b16-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="40b16-108">Type</span></span>|<span data-ttu-id="40b16-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="40b16-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40b16-110">source</span><span class="sxs-lookup"><span data-stu-id="40b16-110">source</span></span>|<span data-ttu-id="40b16-111">teamworkActivityTopicSource</span><span class="sxs-lookup"><span data-stu-id="40b16-111">teamworkActivityTopicSource</span></span>|<span data-ttu-id="40b16-112">Tipo de fonte.</span><span class="sxs-lookup"><span data-stu-id="40b16-112">Type of source.</span></span> <span data-ttu-id="40b16-113">Os valores possíveis são: `entityUrl` e `text`.</span><span class="sxs-lookup"><span data-stu-id="40b16-113">Possible values are: `entityUrl`, `text`.</span></span> <span data-ttu-id="40b16-114">Para obter suporte para URLs do Microsoft Graph, use `entityUrl` .</span><span class="sxs-lookup"><span data-stu-id="40b16-114">For supported Microsoft Graph URLs, use `entityUrl`.</span></span> <span data-ttu-id="40b16-115">Para texto personalizado, use `text` .</span><span class="sxs-lookup"><span data-stu-id="40b16-115">For custom text, use `text`.</span></span>|
|<span data-ttu-id="40b16-116">value</span><span class="sxs-lookup"><span data-stu-id="40b16-116">value</span></span>|<span data-ttu-id="40b16-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40b16-117">String</span></span>|<span data-ttu-id="40b16-118">O valor do tópico.</span><span class="sxs-lookup"><span data-stu-id="40b16-118">The topic value.</span></span> <span data-ttu-id="40b16-119">Se o valor da propriedade **Source** for `entityUrl` , ele deve ser uma URL do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="40b16-119">If the value of the **source** property is `entityUrl`, this must be a Microsoft Graph URL.</span></span> <span data-ttu-id="40b16-120">Se o vaule for `text` , ele deverá ser um valor de texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="40b16-120">If the vaule is `text`, this must be a plain text value.</span></span>|
|<span data-ttu-id="40b16-121">webUrl</span><span class="sxs-lookup"><span data-stu-id="40b16-121">webUrl</span></span>|<span data-ttu-id="40b16-122">String</span><span class="sxs-lookup"><span data-stu-id="40b16-122">String</span></span>|<span data-ttu-id="40b16-123">O link que o usuário clica quando seleciona a notificação.</span><span class="sxs-lookup"><span data-stu-id="40b16-123">The link the user clicks when they select the notification.</span></span> <span data-ttu-id="40b16-124">Opcional quando **Source** é `entityUrl` ; Required quando **Source** é `text` .</span><span class="sxs-lookup"><span data-stu-id="40b16-124">Optional when **source** is `entityUrl`; required when **source** is `text`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40b16-125">Relações</span><span class="sxs-lookup"><span data-stu-id="40b16-125">Relationships</span></span>
<span data-ttu-id="40b16-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="40b16-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="40b16-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="40b16-127">JSON representation</span></span>
<span data-ttu-id="40b16-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="40b16-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkActivityTopic"
}
-->
```json
{
  "@odata.type": "#microsoft.graph.teamworkActivityTopic",
  "source": "String",
  "value": "String",
  "webUrl": "String"
}
```

