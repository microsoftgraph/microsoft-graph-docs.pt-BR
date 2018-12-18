---
title: Tipo de recurso rgbColor
description: Cor em RGB.
author: tfitzmac
ms.openlocfilehash: 0452d8c275e7568df6b304613d8619f04add0548
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307109"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="dd801-103">Tipo de recurso rgbColor</span><span class="sxs-lookup"><span data-stu-id="dd801-103">rgbColor resource type</span></span>

> <span data-ttu-id="dd801-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="dd801-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd801-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dd801-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dd801-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="dd801-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd801-107">Cor em RGB.</span><span class="sxs-lookup"><span data-stu-id="dd801-107">Color in RGB.</span></span>
## <a name="properties"></a><span data-ttu-id="dd801-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dd801-108">Properties</span></span>
|<span data-ttu-id="dd801-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd801-109">Property</span></span>|<span data-ttu-id="dd801-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd801-110">Type</span></span>|<span data-ttu-id="dd801-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd801-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd801-112">r</span><span class="sxs-lookup"><span data-stu-id="dd801-112">r</span></span>|<span data-ttu-id="dd801-113">Byte</span><span class="sxs-lookup"><span data-stu-id="dd801-113">Byte</span></span>|<span data-ttu-id="dd801-114">Valor de vermelho</span><span class="sxs-lookup"><span data-stu-id="dd801-114">Red value</span></span>|
|<span data-ttu-id="dd801-115">g</span><span class="sxs-lookup"><span data-stu-id="dd801-115">g</span></span>|<span data-ttu-id="dd801-116">Byte</span><span class="sxs-lookup"><span data-stu-id="dd801-116">Byte</span></span>|<span data-ttu-id="dd801-117">Valor de verde</span><span class="sxs-lookup"><span data-stu-id="dd801-117">Green value</span></span>|
|<span data-ttu-id="dd801-118">b</span><span class="sxs-lookup"><span data-stu-id="dd801-118">b</span></span>|<span data-ttu-id="dd801-119">Byte</span><span class="sxs-lookup"><span data-stu-id="dd801-119">Byte</span></span>|<span data-ttu-id="dd801-120">Valor de azul</span><span class="sxs-lookup"><span data-stu-id="dd801-120">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd801-121">Relações</span><span class="sxs-lookup"><span data-stu-id="dd801-121">Relationships</span></span>
<span data-ttu-id="dd801-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dd801-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dd801-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dd801-123">JSON Representation</span></span>
<span data-ttu-id="dd801-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dd801-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rgbColor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rgbColor",
  "r": 1024,
  "g": 1024,
  "b": 1024
}
```





