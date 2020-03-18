---
title: tipo de recurso deliveryOptimizationGroupIdCustom
description: Tipo de ID de grupo personalizado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e3dd542a99a7eace79fbc3318117dbf7c539ee79
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42794365"
---
# <a name="deliveryoptimizationgroupidcustom-resource-type"></a><span data-ttu-id="75a5a-103">tipo de recurso deliveryOptimizationGroupIdCustom</span><span class="sxs-lookup"><span data-stu-id="75a5a-103">deliveryOptimizationGroupIdCustom resource type</span></span>

> <span data-ttu-id="75a5a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="75a5a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75a5a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="75a5a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75a5a-106">Tipo de ID de grupo personalizado</span><span class="sxs-lookup"><span data-stu-id="75a5a-106">Custom group id type</span></span>


<span data-ttu-id="75a5a-107">Herda de [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="75a5a-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="75a5a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="75a5a-108">Properties</span></span>
|<span data-ttu-id="75a5a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75a5a-109">Property</span></span>|<span data-ttu-id="75a5a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="75a5a-110">Type</span></span>|<span data-ttu-id="75a5a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="75a5a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75a5a-112">groupIdCustom</span><span class="sxs-lookup"><span data-stu-id="75a5a-112">groupIdCustom</span></span>|<span data-ttu-id="75a5a-113">String</span><span class="sxs-lookup"><span data-stu-id="75a5a-113">String</span></span>|<span data-ttu-id="75a5a-114">Especifica uma ID de grupo arbitrária à qual o dispositivo pertence</span><span class="sxs-lookup"><span data-stu-id="75a5a-114">Specifies an arbitrary group ID that the device belongs to</span></span>|

## <a name="relationships"></a><span data-ttu-id="75a5a-115">Relações</span><span class="sxs-lookup"><span data-stu-id="75a5a-115">Relationships</span></span>
<span data-ttu-id="75a5a-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="75a5a-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="75a5a-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="75a5a-117">JSON Representation</span></span>
<span data-ttu-id="75a5a-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="75a5a-118">Here is a JSON representation of the resource.</span></span>
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



