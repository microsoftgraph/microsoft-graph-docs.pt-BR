---
title: tipo de recurso deliveryOptimizationGroupIdCustom
description: Tipo de ID de grupo personalizado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d4f369c9a3b62480549f19d4a7c1d7b1d0bb196
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31796588"
---
# <a name="deliveryoptimizationgroupidcustom-resource-type"></a><span data-ttu-id="942ba-103">tipo de recurso deliveryOptimizationGroupIdCustom</span><span class="sxs-lookup"><span data-stu-id="942ba-103">deliveryOptimizationGroupIdCustom resource type</span></span>

> <span data-ttu-id="942ba-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="942ba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="942ba-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="942ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="942ba-106">Tipo de ID de grupo personalizado</span><span class="sxs-lookup"><span data-stu-id="942ba-106">Custom group id type</span></span>


<span data-ttu-id="942ba-107">Herda de [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="942ba-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="942ba-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="942ba-108">Properties</span></span>
|<span data-ttu-id="942ba-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="942ba-109">Property</span></span>|<span data-ttu-id="942ba-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="942ba-110">Type</span></span>|<span data-ttu-id="942ba-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="942ba-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="942ba-112">groupIdCustom</span><span class="sxs-lookup"><span data-stu-id="942ba-112">groupIdCustom</span></span>|<span data-ttu-id="942ba-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="942ba-113">String</span></span>|<span data-ttu-id="942ba-114">Especifica uma ID de grupo arbitrária à qual o dispositivo pertence</span><span class="sxs-lookup"><span data-stu-id="942ba-114">Specifies an arbitrary group ID that the device belongs to</span></span>|

## <a name="relationships"></a><span data-ttu-id="942ba-115">Relações</span><span class="sxs-lookup"><span data-stu-id="942ba-115">Relationships</span></span>
<span data-ttu-id="942ba-116">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="942ba-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="942ba-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="942ba-117">JSON Representation</span></span>
<span data-ttu-id="942ba-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="942ba-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdCustom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationGroupIdCustom",
  "groupIdCustom": "String"
}
```





