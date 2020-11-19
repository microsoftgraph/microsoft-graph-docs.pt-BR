---
title: tipo de recurso managedDeviceModelsAndManufacturers
description: Modela e fabrica meatadata para dispositivos gerenciados na conta
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6ed8f1d2bc55e05edc54c3ec19d84c5d7fc46e96
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49208818"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="35987-103">tipo de recurso managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="35987-103">managedDeviceModelsAndManufacturers resource type</span></span>

<span data-ttu-id="35987-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35987-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="35987-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="35987-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35987-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="35987-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35987-107">Modela e fabrica meatadata para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="35987-107">Models and Manufactures meatadata for managed devices in the account</span></span>

## <a name="properties"></a><span data-ttu-id="35987-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="35987-108">Properties</span></span>
|<span data-ttu-id="35987-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35987-109">Property</span></span>|<span data-ttu-id="35987-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="35987-110">Type</span></span>|<span data-ttu-id="35987-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="35987-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35987-112">deviceModels</span><span class="sxs-lookup"><span data-stu-id="35987-112">deviceModels</span></span>|<span data-ttu-id="35987-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="35987-113">String collection</span></span>|<span data-ttu-id="35987-114">Lista de modelos para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="35987-114">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="35987-115">deviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="35987-115">deviceManufacturers</span></span>|<span data-ttu-id="35987-116">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="35987-116">String collection</span></span>|<span data-ttu-id="35987-117">Lista de fabricantes de dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="35987-117">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="35987-118">Relações</span><span class="sxs-lookup"><span data-stu-id="35987-118">Relationships</span></span>
<span data-ttu-id="35987-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="35987-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35987-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="35987-120">JSON Representation</span></span>
<span data-ttu-id="35987-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="35987-121">Here is a JSON representation of the resource.</span></span>
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




