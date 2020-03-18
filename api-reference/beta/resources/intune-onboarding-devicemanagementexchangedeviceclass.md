---
title: tipo de recurso deviceManagementExchangeDeviceClass
description: Classe de dispositivo no Exchange.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 384fa172c255ec3f21ec0088c2b9f4ab025768ce
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42779027"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="070aa-103">tipo de recurso deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="070aa-103">deviceManagementExchangeDeviceClass resource type</span></span>

> <span data-ttu-id="070aa-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="070aa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="070aa-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="070aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="070aa-106">Classe de dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="070aa-106">Device Class in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="070aa-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="070aa-107">Properties</span></span>
|<span data-ttu-id="070aa-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="070aa-108">Property</span></span>|<span data-ttu-id="070aa-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="070aa-109">Type</span></span>|<span data-ttu-id="070aa-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="070aa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="070aa-111">nome</span><span class="sxs-lookup"><span data-stu-id="070aa-111">name</span></span>|<span data-ttu-id="070aa-112">String</span><span class="sxs-lookup"><span data-stu-id="070aa-112">String</span></span>|<span data-ttu-id="070aa-113">Nome da classe de dispositivo que será afetada por essa regra.</span><span class="sxs-lookup"><span data-stu-id="070aa-113">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="070aa-114">type</span><span class="sxs-lookup"><span data-stu-id="070aa-114">type</span></span>|[<span data-ttu-id="070aa-115">deviceManagementExchangeAccessRuleType</span><span class="sxs-lookup"><span data-stu-id="070aa-115">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="070aa-116">Tipo de dispositivo afetado por essa regra, por exemplo, Family.</span><span class="sxs-lookup"><span data-stu-id="070aa-116">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="070aa-117">Os valores possíveis são: `family`, `model`.</span><span class="sxs-lookup"><span data-stu-id="070aa-117">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="070aa-118">Relações</span><span class="sxs-lookup"><span data-stu-id="070aa-118">Relationships</span></span>
<span data-ttu-id="070aa-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="070aa-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="070aa-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="070aa-120">JSON Representation</span></span>
<span data-ttu-id="070aa-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="070aa-121">Here is a JSON representation of the resource.</span></span>
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



