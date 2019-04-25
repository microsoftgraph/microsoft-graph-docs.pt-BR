---
title: tipo de recurso deviceManagementExchangeDeviceClass
description: Classe de dispositivo no Exchange.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7ec9f0242521bf23b4ed5f1c9f002211d542e48c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566560"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="94112-103">tipo de recurso deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="94112-103">deviceManagementExchangeDeviceClass resource type</span></span>

> <span data-ttu-id="94112-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="94112-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94112-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="94112-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94112-106">Classe de dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="94112-106">Device Class in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="94112-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="94112-107">Properties</span></span>
|<span data-ttu-id="94112-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94112-108">Property</span></span>|<span data-ttu-id="94112-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="94112-109">Type</span></span>|<span data-ttu-id="94112-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="94112-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94112-111">name</span><span class="sxs-lookup"><span data-stu-id="94112-111">name</span></span>|<span data-ttu-id="94112-112">String</span><span class="sxs-lookup"><span data-stu-id="94112-112">String</span></span>|<span data-ttu-id="94112-113">Nome da classe de dispositivo que será afetada por essa regra.</span><span class="sxs-lookup"><span data-stu-id="94112-113">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="94112-114">type</span><span class="sxs-lookup"><span data-stu-id="94112-114">type</span></span>|[<span data-ttu-id="94112-115">deviceManagementExchangeAccessRuleType</span><span class="sxs-lookup"><span data-stu-id="94112-115">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="94112-116">Tipo de dispositivo afetado por essa regra, por exemplo, Family.</span><span class="sxs-lookup"><span data-stu-id="94112-116">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="94112-117">Os valores possíveis são: `family`, `model`.</span><span class="sxs-lookup"><span data-stu-id="94112-117">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94112-118">Relações</span><span class="sxs-lookup"><span data-stu-id="94112-118">Relationships</span></span>
<span data-ttu-id="94112-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="94112-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="94112-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="94112-120">JSON Representation</span></span>
<span data-ttu-id="94112-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="94112-121">Here is a JSON representation of the resource.</span></span>
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





