---
title: tipo de recurso cloudPcSourceDeviceImage
description: 'A imagem de origem associada à sua assinatura do Azure. '
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: c944ab1a634d10e978c6ce1620ebe1accc5e4359
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563741"
---
# <a name="cloudpcsourcedeviceimage-resource-type"></a><span data-ttu-id="62c87-103">tipo de recurso cloudPcSourceDeviceImage</span><span class="sxs-lookup"><span data-stu-id="62c87-103">cloudPcSourceDeviceImage resource type</span></span>

<span data-ttu-id="62c87-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62c87-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62c87-105">A imagem de origem associada à sua assinatura do Azure.</span><span class="sxs-lookup"><span data-stu-id="62c87-105">The source image associated with your Azure subscription.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="62c87-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="62c87-106">Properties</span></span>

|<span data-ttu-id="62c87-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62c87-107">Property</span></span>|<span data-ttu-id="62c87-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="62c87-108">Type</span></span>|<span data-ttu-id="62c87-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="62c87-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62c87-110">id</span><span class="sxs-lookup"><span data-stu-id="62c87-110">id</span></span>|<span data-ttu-id="62c87-111">String</span><span class="sxs-lookup"><span data-stu-id="62c87-111">String</span></span>|<span data-ttu-id="62c87-112">A ID da imagem de origem.</span><span class="sxs-lookup"><span data-stu-id="62c87-112">The ID of the source image.</span></span>|
|<span data-ttu-id="62c87-113">displayName</span><span class="sxs-lookup"><span data-stu-id="62c87-113">displayName</span></span>|<span data-ttu-id="62c87-114">String</span><span class="sxs-lookup"><span data-stu-id="62c87-114">String</span></span>|<span data-ttu-id="62c87-115">O nome de exibição da imagem de origem.</span><span class="sxs-lookup"><span data-stu-id="62c87-115">The display name for the source image.</span></span>|

## <a name="relationships"></a><span data-ttu-id="62c87-116">Relações</span><span class="sxs-lookup"><span data-stu-id="62c87-116">Relationships</span></span>

<span data-ttu-id="62c87-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="62c87-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="62c87-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="62c87-118">JSON representation</span></span>

<span data-ttu-id="62c87-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="62c87-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcSourceDeviceImage",
  "baseType": "microsoft.graph.entity"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcSourceDeviceImage",
  "id": "String (identifier)",
  "displayName": "String"
}
```
