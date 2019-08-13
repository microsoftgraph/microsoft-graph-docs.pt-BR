---
title: tipo de recurso deliveryOptimizationGroupIdCustom
description: Tipo de ID de grupo personalizado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c2e0fa587c312d4e4eef43873f08842ac5c7c79b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333398"
---
# <a name="deliveryoptimizationgroupidcustom-resource-type"></a><span data-ttu-id="797bd-103">tipo de recurso deliveryOptimizationGroupIdCustom</span><span class="sxs-lookup"><span data-stu-id="797bd-103">deliveryOptimizationGroupIdCustom resource type</span></span>

> <span data-ttu-id="797bd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="797bd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="797bd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="797bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="797bd-106">Tipo de ID de grupo personalizado</span><span class="sxs-lookup"><span data-stu-id="797bd-106">Custom group id type</span></span>


<span data-ttu-id="797bd-107">Herda de [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="797bd-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="797bd-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="797bd-108">Properties</span></span>
|<span data-ttu-id="797bd-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="797bd-109">Property</span></span>|<span data-ttu-id="797bd-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="797bd-110">Type</span></span>|<span data-ttu-id="797bd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="797bd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="797bd-112">groupIdCustom</span><span class="sxs-lookup"><span data-stu-id="797bd-112">groupIdCustom</span></span>|<span data-ttu-id="797bd-113">String</span><span class="sxs-lookup"><span data-stu-id="797bd-113">String</span></span>|<span data-ttu-id="797bd-114">Especifica uma ID de grupo arbitrária à qual o dispositivo pertence</span><span class="sxs-lookup"><span data-stu-id="797bd-114">Specifies an arbitrary group ID that the device belongs to</span></span>|

## <a name="relationships"></a><span data-ttu-id="797bd-115">Relações</span><span class="sxs-lookup"><span data-stu-id="797bd-115">Relationships</span></span>
<span data-ttu-id="797bd-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="797bd-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="797bd-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="797bd-117">JSON Representation</span></span>
<span data-ttu-id="797bd-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="797bd-118">Here is a JSON representation of the resource.</span></span>
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



