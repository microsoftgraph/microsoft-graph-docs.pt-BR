---
title: Tipo de recurso teamworkActivityTopic
description: Representa o tópico de uma notificação de feed de atividade.
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: abf2372aca7d58061f609c97521795f328af89f6
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473987"
---
# <a name="teamworkactivitytopic-resource-type"></a><span data-ttu-id="6f138-103">Tipo de recurso teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="6f138-103">teamworkActivityTopic resource type</span></span>

<span data-ttu-id="6f138-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f138-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6f138-105">Representa o tópico de uma notificação de feed de atividade.</span><span class="sxs-lookup"><span data-stu-id="6f138-105">Represents the topic of an activity feed notification.</span></span>

## <a name="properties"></a><span data-ttu-id="6f138-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6f138-106">Properties</span></span>
|<span data-ttu-id="6f138-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f138-107">Property</span></span>|<span data-ttu-id="6f138-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f138-108">Type</span></span>|<span data-ttu-id="6f138-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f138-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f138-110">source</span><span class="sxs-lookup"><span data-stu-id="6f138-110">source</span></span>|<span data-ttu-id="6f138-111">teamworkActivityTopicSource</span><span class="sxs-lookup"><span data-stu-id="6f138-111">teamworkActivityTopicSource</span></span>|<span data-ttu-id="6f138-112">Tipo de fonte.</span><span class="sxs-lookup"><span data-stu-id="6f138-112">Type of source.</span></span> <span data-ttu-id="6f138-113">Os valores possíveis são: `entityUrl` e `text`.</span><span class="sxs-lookup"><span data-stu-id="6f138-113">Possible values are: `entityUrl`, `text`.</span></span> <span data-ttu-id="6f138-114">Para URLs do Microsoft Graph com suporte, use `entityUrl` .</span><span class="sxs-lookup"><span data-stu-id="6f138-114">For supported Microsoft Graph URLs, use `entityUrl`.</span></span> <span data-ttu-id="6f138-115">Para texto personalizado, use `text` .</span><span class="sxs-lookup"><span data-stu-id="6f138-115">For custom text, use `text`.</span></span>|
|<span data-ttu-id="6f138-116">value</span><span class="sxs-lookup"><span data-stu-id="6f138-116">value</span></span>|<span data-ttu-id="6f138-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6f138-117">String</span></span>|<span data-ttu-id="6f138-118">O valor do tópico.</span><span class="sxs-lookup"><span data-stu-id="6f138-118">The topic value.</span></span> <span data-ttu-id="6f138-119">Se o valor da **propriedade de origem** for `entityUrl` , deve ser uma URL do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6f138-119">If the value of the **source** property is `entityUrl`, this must be a Microsoft Graph URL.</span></span> <span data-ttu-id="6f138-120">Se o vaule for `text` , este deve ser um valor de texto simples.</span><span class="sxs-lookup"><span data-stu-id="6f138-120">If the vaule is `text`, this must be a plain text value.</span></span>|
|<span data-ttu-id="6f138-121">webUrl</span><span class="sxs-lookup"><span data-stu-id="6f138-121">webUrl</span></span>|<span data-ttu-id="6f138-122">String</span><span class="sxs-lookup"><span data-stu-id="6f138-122">String</span></span>|<span data-ttu-id="6f138-123">O link que o usuário clica ao selecionar a notificação.</span><span class="sxs-lookup"><span data-stu-id="6f138-123">The link the user clicks when they select the notification.</span></span> <span data-ttu-id="6f138-124">Opcional quando **a origem** `entityUrl` for ; obrigatório quando a **origem** for `text` .</span><span class="sxs-lookup"><span data-stu-id="6f138-124">Optional when **source** is `entityUrl`; required when **source** is `text`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f138-125">Relações</span><span class="sxs-lookup"><span data-stu-id="6f138-125">Relationships</span></span>
<span data-ttu-id="6f138-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6f138-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f138-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6f138-127">JSON representation</span></span>
<span data-ttu-id="6f138-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6f138-128">The following is a JSON representation of the resource.</span></span>
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

