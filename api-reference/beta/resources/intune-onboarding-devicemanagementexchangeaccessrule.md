---
title: tipo de recurso deviceManagementExchangeAccessRule
description: Regras de acesso do dispositivo no Exchange.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3a09d1fdea20583c7f80036ae54ca518df92bd5c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524164"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="b9e43-103">tipo de recurso deviceManagementExchangeAccessRule</span><span class="sxs-lookup"><span data-stu-id="b9e43-103">deviceManagementExchangeAccessRule resource type</span></span>

<span data-ttu-id="b9e43-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b9e43-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9e43-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b9e43-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9e43-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b9e43-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9e43-107">Regras de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="b9e43-107">Device Access Rules in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="b9e43-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b9e43-108">Properties</span></span>
|<span data-ttu-id="b9e43-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b9e43-109">Property</span></span>|<span data-ttu-id="b9e43-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9e43-110">Type</span></span>|<span data-ttu-id="b9e43-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9e43-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9e43-112">deviceClass</span><span class="sxs-lookup"><span data-stu-id="b9e43-112">deviceClass</span></span>|[<span data-ttu-id="b9e43-113">deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="b9e43-113">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="b9e43-114">Classe de dispositivo que será afetada por essa regra.</span><span class="sxs-lookup"><span data-stu-id="b9e43-114">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="b9e43-115">accessLevel</span><span class="sxs-lookup"><span data-stu-id="b9e43-115">accessLevel</span></span>|[<span data-ttu-id="b9e43-116">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="b9e43-116">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="b9e43-117">Nível de acesso para o Exchange concedido por esta regra.</span><span class="sxs-lookup"><span data-stu-id="b9e43-117">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="b9e43-118">Os valores possíveis são: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="b9e43-118">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9e43-119">Relações</span><span class="sxs-lookup"><span data-stu-id="b9e43-119">Relationships</span></span>
<span data-ttu-id="b9e43-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b9e43-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9e43-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b9e43-121">JSON Representation</span></span>
<span data-ttu-id="b9e43-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b9e43-122">Here is a JSON representation of the resource.</span></span>
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



