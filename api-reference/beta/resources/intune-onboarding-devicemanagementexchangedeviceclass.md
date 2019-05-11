---
title: tipo de recurso deviceManagementExchangeDeviceClass
description: Classe de dispositivo no Exchange.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 16ed6730363a8f33eeb9ad430f5d2fb56c518032
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940292"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="a93de-103">tipo de recurso deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="a93de-103">deviceManagementExchangeDeviceClass resource type</span></span>

> <span data-ttu-id="a93de-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a93de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a93de-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a93de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a93de-106">Classe de dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="a93de-106">Device Class in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="a93de-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a93de-107">Properties</span></span>
|<span data-ttu-id="a93de-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a93de-108">Property</span></span>|<span data-ttu-id="a93de-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a93de-109">Type</span></span>|<span data-ttu-id="a93de-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a93de-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a93de-111">nome</span><span class="sxs-lookup"><span data-stu-id="a93de-111">name</span></span>|<span data-ttu-id="a93de-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a93de-112">String</span></span>|<span data-ttu-id="a93de-113">Nome da classe de dispositivo que será afetada por essa regra.</span><span class="sxs-lookup"><span data-stu-id="a93de-113">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="a93de-114">type</span><span class="sxs-lookup"><span data-stu-id="a93de-114">type</span></span>|[<span data-ttu-id="a93de-115">deviceManagementExchangeAccessRuleType</span><span class="sxs-lookup"><span data-stu-id="a93de-115">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="a93de-116">Tipo de dispositivo afetado por essa regra, por exemplo, Family.</span><span class="sxs-lookup"><span data-stu-id="a93de-116">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="a93de-117">Os valores possíveis são: `family`, `model`.</span><span class="sxs-lookup"><span data-stu-id="a93de-117">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a93de-118">Relações</span><span class="sxs-lookup"><span data-stu-id="a93de-118">Relationships</span></span>
<span data-ttu-id="a93de-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a93de-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a93de-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a93de-120">JSON Representation</span></span>
<span data-ttu-id="a93de-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a93de-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeDeviceClass",
  "name": "String",
  "type": "String"
}
```




