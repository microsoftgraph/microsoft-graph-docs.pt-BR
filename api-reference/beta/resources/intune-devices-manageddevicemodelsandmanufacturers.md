---
title: tipo de recurso managedDeviceModelsAndManufacturers
description: Modela e fabrica meatadata para dispositivos gerenciados na conta
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 99291829bfa672a9ade85a0a015061e4f6ec8e10
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31782559"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="b0be9-103">tipo de recurso managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="b0be9-103">managedDeviceModelsAndManufacturers resource type</span></span>

> <span data-ttu-id="b0be9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b0be9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0be9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b0be9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0be9-106">Modela e fabrica meatadata para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="b0be9-106">Models and Manufactures meatadata for managed devices in the account</span></span>

## <a name="properties"></a><span data-ttu-id="b0be9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0be9-107">Properties</span></span>
|<span data-ttu-id="b0be9-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0be9-108">Property</span></span>|<span data-ttu-id="b0be9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0be9-109">Type</span></span>|<span data-ttu-id="b0be9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0be9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0be9-111">deviceModels</span><span class="sxs-lookup"><span data-stu-id="b0be9-111">deviceModels</span></span>|<span data-ttu-id="b0be9-112">Coleção String</span><span class="sxs-lookup"><span data-stu-id="b0be9-112">String collection</span></span>|<span data-ttu-id="b0be9-113">Lista de modelos para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="b0be9-113">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="b0be9-114">deviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="b0be9-114">deviceManufacturers</span></span>|<span data-ttu-id="b0be9-115">Coleção String</span><span class="sxs-lookup"><span data-stu-id="b0be9-115">String collection</span></span>|<span data-ttu-id="b0be9-116">Lista de fabricantes de dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="b0be9-116">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0be9-117">Relações</span><span class="sxs-lookup"><span data-stu-id="b0be9-117">Relationships</span></span>
<span data-ttu-id="b0be9-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="b0be9-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0be9-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0be9-119">JSON Representation</span></span>
<span data-ttu-id="b0be9-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0be9-120">Here is a JSON representation of the resource.</span></span>
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





