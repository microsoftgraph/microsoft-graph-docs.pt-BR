---
title: tipo de recurso deviceManagementExchangeAccessRule
description: Regras de acesso do dispositivo no Exchange.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: afe7cde845bfff01100f5e8fabea22d6ce863f63
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455036"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="46d36-103">tipo de recurso deviceManagementExchangeAccessRule</span><span class="sxs-lookup"><span data-stu-id="46d36-103">deviceManagementExchangeAccessRule resource type</span></span>

<span data-ttu-id="46d36-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46d36-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="46d36-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="46d36-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46d36-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="46d36-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46d36-107">Regras de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="46d36-107">Device Access Rules in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="46d36-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="46d36-108">Properties</span></span>
|<span data-ttu-id="46d36-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46d36-109">Property</span></span>|<span data-ttu-id="46d36-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="46d36-110">Type</span></span>|<span data-ttu-id="46d36-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="46d36-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46d36-112">deviceClass</span><span class="sxs-lookup"><span data-stu-id="46d36-112">deviceClass</span></span>|[<span data-ttu-id="46d36-113">deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="46d36-113">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="46d36-114">Classe de dispositivo que será afetada por essa regra.</span><span class="sxs-lookup"><span data-stu-id="46d36-114">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="46d36-115">accessLevel</span><span class="sxs-lookup"><span data-stu-id="46d36-115">accessLevel</span></span>|[<span data-ttu-id="46d36-116">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="46d36-116">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="46d36-117">Nível de acesso para o Exchange concedido por esta regra.</span><span class="sxs-lookup"><span data-stu-id="46d36-117">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="46d36-118">Os valores possíveis são: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="46d36-118">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="46d36-119">Relações</span><span class="sxs-lookup"><span data-stu-id="46d36-119">Relationships</span></span>
<span data-ttu-id="46d36-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="46d36-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="46d36-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="46d36-121">JSON Representation</span></span>
<span data-ttu-id="46d36-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="46d36-122">Here is a JSON representation of the resource.</span></span>
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



