---
title: Tipo de recurso qualityUpdateReference
description: Representa Windows 10 conteúdo de atualização de qualidade.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: ca416ba5031e4642a073f4796ee27996d22f0f5a
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067790"
---
# <a name="qualityupdatereference-resource-type"></a><span data-ttu-id="29b83-103">Tipo de recurso qualityUpdateReference</span><span class="sxs-lookup"><span data-stu-id="29b83-103">qualityUpdateReference resource type</span></span>

<span data-ttu-id="29b83-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="29b83-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29b83-105">Representa Windows 10 conteúdo de atualização de qualidade.</span><span class="sxs-lookup"><span data-stu-id="29b83-105">Represents Windows 10 quality update content.</span></span>

<span data-ttu-id="29b83-106">Em uma implantação, a mesma referência de atualização de qualidade pode resultar em dispositivos que recebem revisões de atualização diferentes, mas o conteúdo é considerado contextually equivalente para todos os dispositivos na implantação.</span><span class="sxs-lookup"><span data-stu-id="29b83-106">In a deployment, the same quality update reference could result in devices receiving different update revisions, but the content is considered contextually equivalent for all devices in the deployment.</span></span>

<span data-ttu-id="29b83-107">Herda de [windowsUpdateReference](../resources/windowsupdates-windowsupdatereference.md).</span><span class="sxs-lookup"><span data-stu-id="29b83-107">Inherits from [windowsUpdateReference](../resources/windowsupdates-windowsupdatereference.md).</span></span> <span data-ttu-id="29b83-108">Tipo base [de expeditedQualityUpdateReference](../resources/windowsupdates-expeditedqualityupdatereference.md).</span><span class="sxs-lookup"><span data-stu-id="29b83-108">Base type of [expeditedQualityUpdateReference](../resources/windowsupdates-expeditedqualityupdatereference.md).</span></span>

## <a name="properties"></a><span data-ttu-id="29b83-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="29b83-109">Properties</span></span>
|<span data-ttu-id="29b83-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29b83-110">Property</span></span>|<span data-ttu-id="29b83-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="29b83-111">Type</span></span>|<span data-ttu-id="29b83-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="29b83-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29b83-113">classificação</span><span class="sxs-lookup"><span data-stu-id="29b83-113">classification</span></span>|<span data-ttu-id="29b83-114">microsoft.graph.windowsUpdates.qualityUpdateClassification</span><span class="sxs-lookup"><span data-stu-id="29b83-114">microsoft.graph.windowsUpdates.qualityUpdateClassification</span></span>|<span data-ttu-id="29b83-115">Especifica a classificação do conteúdo referenciado.</span><span class="sxs-lookup"><span data-stu-id="29b83-115">Specifies the classification of the referenced content.</span></span> <span data-ttu-id="29b83-116">Oferece suporte a um subconjunto dos valores **para qualityUpdateClassification**.</span><span class="sxs-lookup"><span data-stu-id="29b83-116">Supports a subset of the values for **qualityUpdateClassification**.</span></span> <span data-ttu-id="29b83-117">Os valores possíveis são: `security` .</span><span class="sxs-lookup"><span data-stu-id="29b83-117">Possible values are: `security`.</span></span>|
|<span data-ttu-id="29b83-118">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="29b83-118">releaseDateTime</span></span>|<span data-ttu-id="29b83-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29b83-119">DateTimeOffset</span></span>|<span data-ttu-id="29b83-120">Especifica uma atualização de qualidade no determinado serviçoChannel com a classificação determinada por data (ou seja, a última atualização publicada na data especificada).</span><span class="sxs-lookup"><span data-stu-id="29b83-120">Specifies a quality update in the given servicingChannel with the given classification by date (i.e. the last update published on the specified date).</span></span> <span data-ttu-id="29b83-121">O valor padrão é segurança.</span><span class="sxs-lookup"><span data-stu-id="29b83-121">Default value is security.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29b83-122">Relações</span><span class="sxs-lookup"><span data-stu-id="29b83-122">Relationships</span></span>
<span data-ttu-id="29b83-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="29b83-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="29b83-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="29b83-124">JSON representation</span></span>
<span data-ttu-id="29b83-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="29b83-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.qualityUpdateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateReference",
  "classification": "String",
  "releaseDateTime": "String (timestamp)"
}
```

