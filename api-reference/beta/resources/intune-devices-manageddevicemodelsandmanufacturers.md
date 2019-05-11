---
title: tipo de recurso managedDeviceModelsAndManufacturers
description: Modela e fabrica meatadata para dispositivos gerenciados na conta
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d7218e25fc9d1ed0b53bf95cd25ca4b8e3a2e7d8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941937"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="bb03f-103">tipo de recurso managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="bb03f-103">managedDeviceModelsAndManufacturers resource type</span></span>

> <span data-ttu-id="bb03f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bb03f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb03f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bb03f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb03f-106">Modela e fabrica meatadata para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="bb03f-106">Models and Manufactures meatadata for managed devices in the account</span></span>

## <a name="properties"></a><span data-ttu-id="bb03f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bb03f-107">Properties</span></span>
|<span data-ttu-id="bb03f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb03f-108">Property</span></span>|<span data-ttu-id="bb03f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb03f-109">Type</span></span>|<span data-ttu-id="bb03f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb03f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb03f-111">deviceModels</span><span class="sxs-lookup"><span data-stu-id="bb03f-111">deviceModels</span></span>|<span data-ttu-id="bb03f-112">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb03f-112">String collection</span></span>|<span data-ttu-id="bb03f-113">Lista de modelos para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="bb03f-113">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="bb03f-114">deviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="bb03f-114">deviceManufacturers</span></span>|<span data-ttu-id="bb03f-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb03f-115">String collection</span></span>|<span data-ttu-id="bb03f-116">Lista de fabricantes de dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="bb03f-116">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb03f-117">Relações</span><span class="sxs-lookup"><span data-stu-id="bb03f-117">Relationships</span></span>
<span data-ttu-id="bb03f-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bb03f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb03f-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bb03f-119">JSON Representation</span></span>
<span data-ttu-id="bb03f-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bb03f-120">Here is a JSON representation of the resource.</span></span>
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




