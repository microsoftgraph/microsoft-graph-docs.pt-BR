---
title: tipo de recurso deviceManagementExchangeDeviceClass
description: Classe de dispositivo no Exchange.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4099009c67e2c5b0ce8cc5b3c52dd00b1fd32aec
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448040"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="5e417-103">tipo de recurso deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="5e417-103">deviceManagementExchangeDeviceClass resource type</span></span>

<span data-ttu-id="5e417-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e417-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e417-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5e417-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e417-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5e417-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e417-107">Classe de dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="5e417-107">Device Class in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="5e417-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5e417-108">Properties</span></span>
|<span data-ttu-id="5e417-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e417-109">Property</span></span>|<span data-ttu-id="5e417-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e417-110">Type</span></span>|<span data-ttu-id="5e417-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e417-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e417-112">nome</span><span class="sxs-lookup"><span data-stu-id="5e417-112">name</span></span>|<span data-ttu-id="5e417-113">String</span><span class="sxs-lookup"><span data-stu-id="5e417-113">String</span></span>|<span data-ttu-id="5e417-114">Nome da classe de dispositivo que será afetada por essa regra.</span><span class="sxs-lookup"><span data-stu-id="5e417-114">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="5e417-115">type</span><span class="sxs-lookup"><span data-stu-id="5e417-115">type</span></span>|[<span data-ttu-id="5e417-116">deviceManagementExchangeAccessRuleType</span><span class="sxs-lookup"><span data-stu-id="5e417-116">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="5e417-117">Tipo de dispositivo afetado por essa regra, por exemplo, Family.</span><span class="sxs-lookup"><span data-stu-id="5e417-117">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="5e417-118">Os valores possíveis são: `family`, `model`.</span><span class="sxs-lookup"><span data-stu-id="5e417-118">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e417-119">Relações</span><span class="sxs-lookup"><span data-stu-id="5e417-119">Relationships</span></span>
<span data-ttu-id="5e417-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5e417-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e417-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5e417-121">JSON Representation</span></span>
<span data-ttu-id="5e417-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5e417-122">Here is a JSON representation of the resource.</span></span>
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



