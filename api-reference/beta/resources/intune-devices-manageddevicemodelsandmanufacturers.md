---
title: tipo de recurso managedDeviceModelsAndManufacturers
description: Modela e fabrica meatadata para dispositivos gerenciados na conta
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 99291829bfa672a9ade85a0a015061e4f6ec8e10
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522101"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="20c33-103">tipo de recurso managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="20c33-103">managedDeviceModelsAndManufacturers resource type</span></span>

> <span data-ttu-id="20c33-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="20c33-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20c33-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="20c33-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20c33-106">Modela e fabrica meatadata para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="20c33-106">Models and Manufactures meatadata for managed devices in the account</span></span>

## <a name="properties"></a><span data-ttu-id="20c33-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="20c33-107">Properties</span></span>
|<span data-ttu-id="20c33-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20c33-108">Property</span></span>|<span data-ttu-id="20c33-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="20c33-109">Type</span></span>|<span data-ttu-id="20c33-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="20c33-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20c33-111">deviceModels</span><span class="sxs-lookup"><span data-stu-id="20c33-111">deviceModels</span></span>|<span data-ttu-id="20c33-112">String collection</span><span class="sxs-lookup"><span data-stu-id="20c33-112">String collection</span></span>|<span data-ttu-id="20c33-113">Lista de modelos para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="20c33-113">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="20c33-114">deviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="20c33-114">deviceManufacturers</span></span>|<span data-ttu-id="20c33-115">String collection</span><span class="sxs-lookup"><span data-stu-id="20c33-115">String collection</span></span>|<span data-ttu-id="20c33-116">Lista de fabricantes de dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="20c33-116">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="20c33-117">Relações</span><span class="sxs-lookup"><span data-stu-id="20c33-117">Relationships</span></span>
<span data-ttu-id="20c33-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="20c33-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="20c33-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="20c33-119">JSON Representation</span></span>
<span data-ttu-id="20c33-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="20c33-120">Here is a JSON representation of the resource.</span></span>
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





