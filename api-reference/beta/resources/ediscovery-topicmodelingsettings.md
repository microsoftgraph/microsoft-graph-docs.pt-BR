---
title: tipo de recurso topicModelingSettings
description: Configurações de modelagem de tópicos para um caso de Descoberta E
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: bd433de0aa88298961366f50425706e1af4bffde
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080711"
---
# <a name="topicmodelingsettings-resource-type"></a><span data-ttu-id="11f2d-103">tipo de recurso topicModelingSettings</span><span class="sxs-lookup"><span data-stu-id="11f2d-103">topicModelingSettings resource type</span></span>

<span data-ttu-id="11f2d-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="11f2d-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11f2d-105">Configurações de modelagem de tópicos (Temas) para um caso de Descoberta e.</span><span class="sxs-lookup"><span data-stu-id="11f2d-105">Topic modeling (Themes) settings for an eDiscovery case.</span></span> <span data-ttu-id="11f2d-106">Para saber mais, consulte [Configure search and analytics settings in Advanced eDiscovery](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery).</span><span class="sxs-lookup"><span data-stu-id="11f2d-106">To learn more, see [Configure search and analytics settings in Advanced eDiscovery](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery).</span></span>

## <a name="properties"></a><span data-ttu-id="11f2d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11f2d-107">Properties</span></span>

|<span data-ttu-id="11f2d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11f2d-108">Property</span></span>|<span data-ttu-id="11f2d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="11f2d-109">Type</span></span>|<span data-ttu-id="11f2d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="11f2d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11f2d-111">dinamicamenteAdjustTopicCount</span><span class="sxs-lookup"><span data-stu-id="11f2d-111">dynamicallyAdjustTopicCount</span></span>|<span data-ttu-id="11f2d-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="11f2d-112">Boolean</span></span>|<span data-ttu-id="11f2d-113">Para saber mais, confira [Ajustar o número máximo de temas dinamicamente](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes).</span><span class="sxs-lookup"><span data-stu-id="11f2d-113">To learn more, see [Adjust maximum number of themes dynamically](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes).</span></span>|
|<span data-ttu-id="11f2d-114">ignoreNumbers</span><span class="sxs-lookup"><span data-stu-id="11f2d-114">ignoreNumbers</span></span>|<span data-ttu-id="11f2d-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="11f2d-115">Boolean</span></span>|<span data-ttu-id="11f2d-116">Para saber mais, confira [Incluir números em temas](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes).</span><span class="sxs-lookup"><span data-stu-id="11f2d-116">To learn more, see [Include numbers in themes](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes).</span></span>|
|<span data-ttu-id="11f2d-117">isEnabled</span><span class="sxs-lookup"><span data-stu-id="11f2d-117">isEnabled</span></span>|<span data-ttu-id="11f2d-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="11f2d-118">Boolean</span></span>|<span data-ttu-id="11f2d-119">Indica se os temas estão habilitados para o caso.</span><span class="sxs-lookup"><span data-stu-id="11f2d-119">Indicates whether themes is enabled for the case.</span></span>|
|<span data-ttu-id="11f2d-120">topicCount</span><span class="sxs-lookup"><span data-stu-id="11f2d-120">topicCount</span></span>|<span data-ttu-id="11f2d-121">Int32</span><span class="sxs-lookup"><span data-stu-id="11f2d-121">Int32</span></span>|<span data-ttu-id="11f2d-122">Para saber mais, confira [Número máximo de temas](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes).</span><span class="sxs-lookup"><span data-stu-id="11f2d-122">To learn more, see [Maximum number of themes](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes).</span></span>|

## <a name="relationships"></a><span data-ttu-id="11f2d-123">Relações</span><span class="sxs-lookup"><span data-stu-id="11f2d-123">Relationships</span></span>

<span data-ttu-id="11f2d-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="11f2d-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="11f2d-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11f2d-125">JSON representation</span></span>

<span data-ttu-id="11f2d-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="11f2d-126">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.ediscovery.topicModelingSettings"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.topicModelingSettings",
  "isEnabled": "Boolean",
  "ignoreNumbers": "Boolean",
  "topicCount": "Integer",
  "dynamicallyAdjustTopicCount": "Boolean"
}
```
