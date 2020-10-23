---
title: tipo de recurso managedDeviceModelsAndManufacturers
description: Modela e fabrica meatadata para dispositivos gerenciados na conta
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: afcd9ea210d50bd5778133fcac743ba7bd624118
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725467"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="be8d0-103">tipo de recurso managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="be8d0-103">managedDeviceModelsAndManufacturers resource type</span></span>

<span data-ttu-id="be8d0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be8d0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="be8d0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="be8d0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be8d0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="be8d0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be8d0-107">Modela e fabrica meatadata para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="be8d0-107">Models and Manufactures meatadata for managed devices in the account</span></span>

## <a name="properties"></a><span data-ttu-id="be8d0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="be8d0-108">Properties</span></span>
|<span data-ttu-id="be8d0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="be8d0-109">Property</span></span>|<span data-ttu-id="be8d0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="be8d0-110">Type</span></span>|<span data-ttu-id="be8d0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="be8d0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be8d0-112">deviceModels</span><span class="sxs-lookup"><span data-stu-id="be8d0-112">deviceModels</span></span>|<span data-ttu-id="be8d0-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="be8d0-113">String collection</span></span>|<span data-ttu-id="be8d0-114">Lista de modelos para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="be8d0-114">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="be8d0-115">deviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="be8d0-115">deviceManufacturers</span></span>|<span data-ttu-id="be8d0-116">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="be8d0-116">String collection</span></span>|<span data-ttu-id="be8d0-117">Lista de fabricantes de dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="be8d0-117">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="be8d0-118">Relações</span><span class="sxs-lookup"><span data-stu-id="be8d0-118">Relationships</span></span>
<span data-ttu-id="be8d0-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="be8d0-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="be8d0-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="be8d0-120">JSON Representation</span></span>
<span data-ttu-id="be8d0-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="be8d0-121">Here is a JSON representation of the resource.</span></span>
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





