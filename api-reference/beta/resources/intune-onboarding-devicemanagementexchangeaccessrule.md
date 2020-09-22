---
title: tipo de recurso deviceManagementExchangeAccessRule
description: Regras de acesso do dispositivo no Exchange.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 62d5dac75116278eac6f3d1764dbb8f8865434f4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029649"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="39f97-103">tipo de recurso deviceManagementExchangeAccessRule</span><span class="sxs-lookup"><span data-stu-id="39f97-103">deviceManagementExchangeAccessRule resource type</span></span>

<span data-ttu-id="39f97-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39f97-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="39f97-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="39f97-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39f97-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="39f97-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39f97-107">Regras de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="39f97-107">Device Access Rules in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="39f97-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="39f97-108">Properties</span></span>
|<span data-ttu-id="39f97-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="39f97-109">Property</span></span>|<span data-ttu-id="39f97-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="39f97-110">Type</span></span>|<span data-ttu-id="39f97-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="39f97-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39f97-112">deviceClass</span><span class="sxs-lookup"><span data-stu-id="39f97-112">deviceClass</span></span>|[<span data-ttu-id="39f97-113">deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="39f97-113">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="39f97-114">Classe de dispositivo que será afetada por essa regra.</span><span class="sxs-lookup"><span data-stu-id="39f97-114">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="39f97-115">accessLevel</span><span class="sxs-lookup"><span data-stu-id="39f97-115">accessLevel</span></span>|[<span data-ttu-id="39f97-116">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="39f97-116">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="39f97-117">Nível de acesso para o Exchange concedido por esta regra.</span><span class="sxs-lookup"><span data-stu-id="39f97-117">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="39f97-118">Os valores possíveis são: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="39f97-118">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39f97-119">Relações</span><span class="sxs-lookup"><span data-stu-id="39f97-119">Relationships</span></span>
<span data-ttu-id="39f97-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="39f97-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="39f97-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="39f97-121">JSON Representation</span></span>
<span data-ttu-id="39f97-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="39f97-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeAccessRule",
  "deviceClass": {
    "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
    "name": "String",
    "type": "String"
  },
  "accessLevel": "String"
}
```






