---
title: tipo de recurso managedDeviceModelsAndManufacturers
description: Modela e fabrica meatadata para dispositivos gerenciados na conta
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: db6d5a59a748f5e8befbe662a0b317a185437665
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443951"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="46d82-103">tipo de recurso managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="46d82-103">managedDeviceModelsAndManufacturers resource type</span></span>

<span data-ttu-id="46d82-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46d82-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="46d82-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="46d82-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46d82-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="46d82-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46d82-107">Modela e fabrica meatadata para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="46d82-107">Models and Manufactures meatadata for managed devices in the account</span></span>

## <a name="properties"></a><span data-ttu-id="46d82-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="46d82-108">Properties</span></span>
|<span data-ttu-id="46d82-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46d82-109">Property</span></span>|<span data-ttu-id="46d82-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="46d82-110">Type</span></span>|<span data-ttu-id="46d82-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="46d82-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46d82-112">deviceModels</span><span class="sxs-lookup"><span data-stu-id="46d82-112">deviceModels</span></span>|<span data-ttu-id="46d82-113">Coleção String</span><span class="sxs-lookup"><span data-stu-id="46d82-113">String collection</span></span>|<span data-ttu-id="46d82-114">Lista de modelos para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="46d82-114">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="46d82-115">deviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="46d82-115">deviceManufacturers</span></span>|<span data-ttu-id="46d82-116">Coleção String</span><span class="sxs-lookup"><span data-stu-id="46d82-116">String collection</span></span>|<span data-ttu-id="46d82-117">Lista de fabricantes de dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="46d82-117">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="46d82-118">Relações</span><span class="sxs-lookup"><span data-stu-id="46d82-118">Relationships</span></span>
<span data-ttu-id="46d82-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="46d82-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="46d82-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="46d82-120">JSON Representation</span></span>
<span data-ttu-id="46d82-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="46d82-121">Here is a JSON representation of the resource.</span></span>
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



