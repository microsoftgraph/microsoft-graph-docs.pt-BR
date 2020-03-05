---
title: tipo de recurso managedDeviceModelsAndManufacturers
description: Modela e fabrica meatadata para dispositivos gerenciados na conta
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: aa241bd17ad8c42074ed74d2d2548777ea8bf3ba
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528533"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="282e2-103">tipo de recurso managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="282e2-103">managedDeviceModelsAndManufacturers resource type</span></span>

<span data-ttu-id="282e2-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="282e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="282e2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="282e2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="282e2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="282e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="282e2-107">Modela e fabrica meatadata para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="282e2-107">Models and Manufactures meatadata for managed devices in the account</span></span>

## <a name="properties"></a><span data-ttu-id="282e2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="282e2-108">Properties</span></span>
|<span data-ttu-id="282e2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="282e2-109">Property</span></span>|<span data-ttu-id="282e2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="282e2-110">Type</span></span>|<span data-ttu-id="282e2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="282e2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="282e2-112">deviceModels</span><span class="sxs-lookup"><span data-stu-id="282e2-112">deviceModels</span></span>|<span data-ttu-id="282e2-113">String collection</span><span class="sxs-lookup"><span data-stu-id="282e2-113">String collection</span></span>|<span data-ttu-id="282e2-114">Lista de modelos para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="282e2-114">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="282e2-115">deviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="282e2-115">deviceManufacturers</span></span>|<span data-ttu-id="282e2-116">String collection</span><span class="sxs-lookup"><span data-stu-id="282e2-116">String collection</span></span>|<span data-ttu-id="282e2-117">Lista de fabricantes de dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="282e2-117">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="282e2-118">Relações</span><span class="sxs-lookup"><span data-stu-id="282e2-118">Relationships</span></span>
<span data-ttu-id="282e2-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="282e2-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="282e2-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="282e2-120">JSON Representation</span></span>
<span data-ttu-id="282e2-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="282e2-121">Here is a JSON representation of the resource.</span></span>
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



