---
title: tipo de recurso deviceManagementExchangeDeviceClass
description: Classe de dispositivo no Exchange.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 79c1e7cf50bc0cc87f620ad0b875704005b90435
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029607"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="9a335-103">tipo de recurso deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="9a335-103">deviceManagementExchangeDeviceClass resource type</span></span>

<span data-ttu-id="9a335-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a335-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a335-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9a335-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a335-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9a335-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a335-107">Classe de dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="9a335-107">Device Class in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="9a335-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9a335-108">Properties</span></span>
|<span data-ttu-id="9a335-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a335-109">Property</span></span>|<span data-ttu-id="9a335-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a335-110">Type</span></span>|<span data-ttu-id="9a335-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a335-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a335-112">nome</span><span class="sxs-lookup"><span data-stu-id="9a335-112">name</span></span>|<span data-ttu-id="9a335-113">String</span><span class="sxs-lookup"><span data-stu-id="9a335-113">String</span></span>|<span data-ttu-id="9a335-114">Nome da classe de dispositivo que será afetada por essa regra.</span><span class="sxs-lookup"><span data-stu-id="9a335-114">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="9a335-115">tipo</span><span class="sxs-lookup"><span data-stu-id="9a335-115">type</span></span>|[<span data-ttu-id="9a335-116">deviceManagementExchangeAccessRuleType</span><span class="sxs-lookup"><span data-stu-id="9a335-116">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="9a335-117">Tipo de dispositivo afetado por essa regra, por exemplo, Family.</span><span class="sxs-lookup"><span data-stu-id="9a335-117">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="9a335-118">Os valores possíveis são: `family`, `model`.</span><span class="sxs-lookup"><span data-stu-id="9a335-118">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a335-119">Relações</span><span class="sxs-lookup"><span data-stu-id="9a335-119">Relationships</span></span>
<span data-ttu-id="9a335-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9a335-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a335-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9a335-121">JSON Representation</span></span>
<span data-ttu-id="9a335-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9a335-122">Here is a JSON representation of the resource.</span></span>
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






