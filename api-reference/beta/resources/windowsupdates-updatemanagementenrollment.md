---
title: Tipo de recurso updateManagementEnrollment
description: Representa o registro no gerenciamento pelo serviço de uma determinada categoria de atualização.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 1d00bc152d5fc3b7b4be267cd3ea56fab52b8b38
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067232"
---
# <a name="updatemanagementenrollment-resource-type"></a><span data-ttu-id="ff47a-103">Tipo de recurso updateManagementEnrollment</span><span class="sxs-lookup"><span data-stu-id="ff47a-103">updateManagementEnrollment resource type</span></span>

<span data-ttu-id="ff47a-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="ff47a-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff47a-105">Representa o registro no gerenciamento pelo serviço de uma determinada categoria de atualização.</span><span class="sxs-lookup"><span data-stu-id="ff47a-105">Represents enrollment into management by the service of a certain update category.</span></span>

<span data-ttu-id="ff47a-106">Herda [de updatableAssetEnrollment](../resources/windowsupdates-updatableassetenrollment.md).</span><span class="sxs-lookup"><span data-stu-id="ff47a-106">Inherits from [updatableAssetEnrollment](../resources/windowsupdates-updatableassetenrollment.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ff47a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ff47a-107">Properties</span></span>
|<span data-ttu-id="ff47a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff47a-108">Property</span></span>|<span data-ttu-id="ff47a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff47a-109">Type</span></span>|<span data-ttu-id="ff47a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff47a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff47a-111">updateCategory</span><span class="sxs-lookup"><span data-stu-id="ff47a-111">updateCategory</span></span>|<span data-ttu-id="ff47a-112">microsoft.graph.windowsUpdates.updateCategory</span><span class="sxs-lookup"><span data-stu-id="ff47a-112">microsoft.graph.windowsUpdates.updateCategory</span></span>|<span data-ttu-id="ff47a-113">A categoria de atualizações que o serviço gerencia.</span><span class="sxs-lookup"><span data-stu-id="ff47a-113">The category of updates that the service manages.</span></span> <span data-ttu-id="ff47a-114">Oferece suporte a um subconjunto dos valores **para updateCategory**.</span><span class="sxs-lookup"><span data-stu-id="ff47a-114">Supports a subset of the values for **updateCategory**.</span></span> <span data-ttu-id="ff47a-115">Os valores possíveis são: `feature` .</span><span class="sxs-lookup"><span data-stu-id="ff47a-115">Possible values are: `feature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff47a-116">Relações</span><span class="sxs-lookup"><span data-stu-id="ff47a-116">Relationships</span></span>
<span data-ttu-id="ff47a-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ff47a-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff47a-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ff47a-118">JSON representation</span></span>
<span data-ttu-id="ff47a-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ff47a-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.updateManagementEnrollment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.updateManagementEnrollment",
  "updateCategory": "String"
}
```

