---
title: tipo de recurso numberRange
description: Definição do intervalo de números.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 772ffc59bc9ac4848b6b34eee8c62f8006468784
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958715"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="e5621-103">tipo de recurso numberRange</span><span class="sxs-lookup"><span data-stu-id="e5621-103">numberRange resource type</span></span>

> <span data-ttu-id="e5621-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e5621-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5621-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e5621-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5621-106">Definição do intervalo de números.</span><span class="sxs-lookup"><span data-stu-id="e5621-106">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="e5621-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e5621-107">Properties</span></span>
|<span data-ttu-id="e5621-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5621-108">Property</span></span>|<span data-ttu-id="e5621-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5621-109">Type</span></span>|<span data-ttu-id="e5621-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5621-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5621-111">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="e5621-111">lowerNumber</span></span>|<span data-ttu-id="e5621-112">Int32</span><span class="sxs-lookup"><span data-stu-id="e5621-112">Int32</span></span>|<span data-ttu-id="e5621-113">Número menor.</span><span class="sxs-lookup"><span data-stu-id="e5621-113">Lower number.</span></span>|
|<span data-ttu-id="e5621-114">upperNumber</span><span class="sxs-lookup"><span data-stu-id="e5621-114">upperNumber</span></span>|<span data-ttu-id="e5621-115">Int32</span><span class="sxs-lookup"><span data-stu-id="e5621-115">Int32</span></span>|<span data-ttu-id="e5621-116">Número superior.</span><span class="sxs-lookup"><span data-stu-id="e5621-116">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5621-117">Relações</span><span class="sxs-lookup"><span data-stu-id="e5621-117">Relationships</span></span>
<span data-ttu-id="e5621-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e5621-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5621-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e5621-119">JSON Representation</span></span>
<span data-ttu-id="e5621-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e5621-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.numberRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.numberRange",
  "lowerNumber": 1024,
  "upperNumber": 1024
}
```





