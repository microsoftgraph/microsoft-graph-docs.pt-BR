---
title: Tipo de recurso cloudPcSourceDeviceImage
description: 'A imagem de origem associada à sua assinatura do Azure. '
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 1b0c656142ddad5af3d0af7778d0ae04f0c5d7b4
ms.sourcegitcommit: de175a11806f9e9ba3c916384e897aee1cc7f75c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/09/2021
ms.locfileid: "49790738"
---
# <a name="cloudpcsourcedeviceimage-resource-type"></a><span data-ttu-id="c58f8-103">Tipo de recurso cloudPcSourceDeviceImage</span><span class="sxs-lookup"><span data-stu-id="c58f8-103">cloudPcSourceDeviceImage resource type</span></span>

<span data-ttu-id="c58f8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c58f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c58f8-105">A imagem de origem associada à sua assinatura do Azure.</span><span class="sxs-lookup"><span data-stu-id="c58f8-105">The source image associated with your Azure subscription.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="c58f8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c58f8-106">Properties</span></span>

|<span data-ttu-id="c58f8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c58f8-107">Property</span></span>|<span data-ttu-id="c58f8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c58f8-108">Type</span></span>|<span data-ttu-id="c58f8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c58f8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c58f8-110">id</span><span class="sxs-lookup"><span data-stu-id="c58f8-110">id</span></span>|<span data-ttu-id="c58f8-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c58f8-111">String</span></span>|<span data-ttu-id="c58f8-112">A ID da imagem de origem.</span><span class="sxs-lookup"><span data-stu-id="c58f8-112">The ID of the source image.</span></span>|
|<span data-ttu-id="c58f8-113">displayName</span><span class="sxs-lookup"><span data-stu-id="c58f8-113">displayName</span></span>|<span data-ttu-id="c58f8-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c58f8-114">String</span></span>|<span data-ttu-id="c58f8-115">O nome de exibição da imagem de origem.</span><span class="sxs-lookup"><span data-stu-id="c58f8-115">The display name for the source image.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c58f8-116">Relações</span><span class="sxs-lookup"><span data-stu-id="c58f8-116">Relationships</span></span>

<span data-ttu-id="c58f8-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c58f8-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c58f8-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c58f8-118">JSON representation</span></span>

<span data-ttu-id="c58f8-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c58f8-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcSourceDeviceImage"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcSourceDeviceImage",
  "id": "String (identifier)",
  "displayName": "String"
}
```
