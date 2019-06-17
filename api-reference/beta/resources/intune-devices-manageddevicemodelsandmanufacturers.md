---
title: tipo de recurso managedDeviceModelsAndManufacturers
description: Modela e fabrica meatadata para dispositivos gerenciados na conta
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 49d470087dcbbab5c8efb4dc9ea47f281f37f746
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995081"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="7d024-103">tipo de recurso managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="7d024-103">managedDeviceModelsAndManufacturers resource type</span></span>

> <span data-ttu-id="7d024-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7d024-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d024-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7d024-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d024-106">Modela e fabrica meatadata para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="7d024-106">Models and Manufactures meatadata for managed devices in the account</span></span>

## <a name="properties"></a><span data-ttu-id="7d024-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7d024-107">Properties</span></span>
|<span data-ttu-id="7d024-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d024-108">Property</span></span>|<span data-ttu-id="7d024-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d024-109">Type</span></span>|<span data-ttu-id="7d024-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d024-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d024-111">deviceModels</span><span class="sxs-lookup"><span data-stu-id="7d024-111">deviceModels</span></span>|<span data-ttu-id="7d024-112">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d024-112">String collection</span></span>|<span data-ttu-id="7d024-113">Lista de modelos para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="7d024-113">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="7d024-114">deviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="7d024-114">deviceManufacturers</span></span>|<span data-ttu-id="7d024-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d024-115">String collection</span></span>|<span data-ttu-id="7d024-116">Lista de fabricantes de dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="7d024-116">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d024-117">Relações</span><span class="sxs-lookup"><span data-stu-id="7d024-117">Relationships</span></span>
<span data-ttu-id="7d024-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7d024-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7d024-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7d024-119">JSON Representation</span></span>
<span data-ttu-id="7d024-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7d024-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceModelsAndManufacturers",
  "deviceModels": [
    "String"
  ],
  "deviceManufacturers": [
    "String"
  ]
}
```





