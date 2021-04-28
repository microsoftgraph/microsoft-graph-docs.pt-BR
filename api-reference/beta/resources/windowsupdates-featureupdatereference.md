---
title: Tipo de recurso featureUpdateReference
description: Representa Windows 10 conteúdo de atualização de recursos.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 69eda05a94982429035999bd914c6f0c9847fa67
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067267"
---
# <a name="featureupdatereference-resource-type"></a><span data-ttu-id="04206-103">Tipo de recurso featureUpdateReference</span><span class="sxs-lookup"><span data-stu-id="04206-103">featureUpdateReference resource type</span></span>

<span data-ttu-id="04206-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="04206-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04206-105">Representa Windows 10 conteúdo de atualização de recursos.</span><span class="sxs-lookup"><span data-stu-id="04206-105">Represents Windows 10 feature update content.</span></span>

<span data-ttu-id="04206-106">Em uma implantação, a mesma referência de atualização de recurso pode resultar em dispositivos que recebem revisões de atualização diferentes, mas o conteúdo é considerado contextually equivalente para todos os dispositivos na implantação.</span><span class="sxs-lookup"><span data-stu-id="04206-106">In a deployment, the same feature update reference could result in devices receiving different update revisions, but the content is considered contextually equivalent for all devices in the deployment.</span></span>

<span data-ttu-id="04206-107">Herda de [windowsUpdateReference](../resources/windowsupdates-windowsupdatereference.md).</span><span class="sxs-lookup"><span data-stu-id="04206-107">Inherits from [windowsUpdateReference](../resources/windowsupdates-windowsupdatereference.md).</span></span>

## <a name="properties"></a><span data-ttu-id="04206-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="04206-108">Properties</span></span>
|<span data-ttu-id="04206-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04206-109">Property</span></span>|<span data-ttu-id="04206-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="04206-110">Type</span></span>|<span data-ttu-id="04206-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="04206-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04206-112">versão</span><span class="sxs-lookup"><span data-stu-id="04206-112">version</span></span>|<span data-ttu-id="04206-113">String</span><span class="sxs-lookup"><span data-stu-id="04206-113">String</span></span>|<span data-ttu-id="04206-114">Especifica uma atualização de recurso por versão.</span><span class="sxs-lookup"><span data-stu-id="04206-114">Specifies a feature update by version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04206-115">Relações</span><span class="sxs-lookup"><span data-stu-id="04206-115">Relationships</span></span>
<span data-ttu-id="04206-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="04206-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="04206-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="04206-117">JSON representation</span></span>
<span data-ttu-id="04206-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="04206-118">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.featureUpdateReference",
  "version": "String"
}
```

