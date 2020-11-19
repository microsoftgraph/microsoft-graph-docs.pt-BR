---
title: tipo de recurso deviceManagementExchangeDeviceClass
description: Classe de dispositivo no Exchange.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 86b26f41e756471b416686cf7443b6280341097b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49272238"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="f78b1-103">tipo de recurso deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="f78b1-103">deviceManagementExchangeDeviceClass resource type</span></span>

<span data-ttu-id="f78b1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f78b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f78b1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f78b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f78b1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f78b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f78b1-107">Classe de dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="f78b1-107">Device Class in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="f78b1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f78b1-108">Properties</span></span>
|<span data-ttu-id="f78b1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f78b1-109">Property</span></span>|<span data-ttu-id="f78b1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f78b1-110">Type</span></span>|<span data-ttu-id="f78b1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f78b1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f78b1-112">nome</span><span class="sxs-lookup"><span data-stu-id="f78b1-112">name</span></span>|<span data-ttu-id="f78b1-113">String</span><span class="sxs-lookup"><span data-stu-id="f78b1-113">String</span></span>|<span data-ttu-id="f78b1-114">Nome da classe de dispositivo que será afetada por essa regra.</span><span class="sxs-lookup"><span data-stu-id="f78b1-114">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="f78b1-115">tipo</span><span class="sxs-lookup"><span data-stu-id="f78b1-115">type</span></span>|[<span data-ttu-id="f78b1-116">deviceManagementExchangeAccessRuleType</span><span class="sxs-lookup"><span data-stu-id="f78b1-116">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="f78b1-117">Tipo de dispositivo afetado por essa regra, por exemplo, Family.</span><span class="sxs-lookup"><span data-stu-id="f78b1-117">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="f78b1-118">Os valores possíveis são: `family`, `model`.</span><span class="sxs-lookup"><span data-stu-id="f78b1-118">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f78b1-119">Relações</span><span class="sxs-lookup"><span data-stu-id="f78b1-119">Relationships</span></span>
<span data-ttu-id="f78b1-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f78b1-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f78b1-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f78b1-121">JSON Representation</span></span>
<span data-ttu-id="f78b1-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f78b1-122">Here is a JSON representation of the resource.</span></span>
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




