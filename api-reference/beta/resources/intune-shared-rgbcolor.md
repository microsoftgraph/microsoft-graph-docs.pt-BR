---
title: Tipo de recurso rgbColor
description: Cor em RGB.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fd734d2cb7c1c03cfdab62b8a8f1acd9acac6814
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846722"
---
# <a name="rgbcolor-resource-type"></a><span data-ttu-id="7f236-103">Tipo de recurso rgbColor</span><span class="sxs-lookup"><span data-stu-id="7f236-103">rgbColor resource type</span></span>

> <span data-ttu-id="7f236-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7f236-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f236-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7f236-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7f236-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7f236-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f236-107">Cor em RGB.</span><span class="sxs-lookup"><span data-stu-id="7f236-107">Color in RGB.</span></span>
## <a name="properties"></a><span data-ttu-id="7f236-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7f236-108">Properties</span></span>
|<span data-ttu-id="7f236-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f236-109">Property</span></span>|<span data-ttu-id="7f236-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f236-110">Type</span></span>|<span data-ttu-id="7f236-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f236-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f236-112">r</span><span class="sxs-lookup"><span data-stu-id="7f236-112">r</span></span>|<span data-ttu-id="7f236-113">Byte</span><span class="sxs-lookup"><span data-stu-id="7f236-113">Byte</span></span>|<span data-ttu-id="7f236-114">Valor de vermelho</span><span class="sxs-lookup"><span data-stu-id="7f236-114">Red value</span></span>|
|<span data-ttu-id="7f236-115">g</span><span class="sxs-lookup"><span data-stu-id="7f236-115">g</span></span>|<span data-ttu-id="7f236-116">Byte</span><span class="sxs-lookup"><span data-stu-id="7f236-116">Byte</span></span>|<span data-ttu-id="7f236-117">Valor de verde</span><span class="sxs-lookup"><span data-stu-id="7f236-117">Green value</span></span>|
|<span data-ttu-id="7f236-118">b</span><span class="sxs-lookup"><span data-stu-id="7f236-118">b</span></span>|<span data-ttu-id="7f236-119">Byte</span><span class="sxs-lookup"><span data-stu-id="7f236-119">Byte</span></span>|<span data-ttu-id="7f236-120">Valor de azul</span><span class="sxs-lookup"><span data-stu-id="7f236-120">Blue value</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f236-121">Relações</span><span class="sxs-lookup"><span data-stu-id="7f236-121">Relationships</span></span>
<span data-ttu-id="7f236-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7f236-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7f236-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7f236-123">JSON Representation</span></span>
<span data-ttu-id="7f236-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7f236-124">Here is a JSON representation of the resource.</span></span>
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





