---
title: tipo de recurso deviceManagementExchangeAccessRule
description: Regras de acesso do dispositivo no Exchange.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8ecd6777327defe913818e984ca30d2bc6f47157
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49307420"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="e7301-103">tipo de recurso deviceManagementExchangeAccessRule</span><span class="sxs-lookup"><span data-stu-id="e7301-103">deviceManagementExchangeAccessRule resource type</span></span>

<span data-ttu-id="e7301-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7301-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e7301-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e7301-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7301-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e7301-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7301-107">Regras de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="e7301-107">Device Access Rules in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="e7301-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e7301-108">Properties</span></span>
|<span data-ttu-id="e7301-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e7301-109">Property</span></span>|<span data-ttu-id="e7301-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7301-110">Type</span></span>|<span data-ttu-id="e7301-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7301-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7301-112">deviceClass</span><span class="sxs-lookup"><span data-stu-id="e7301-112">deviceClass</span></span>|[<span data-ttu-id="e7301-113">deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="e7301-113">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="e7301-114">Classe de dispositivo que será afetada por essa regra.</span><span class="sxs-lookup"><span data-stu-id="e7301-114">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="e7301-115">accessLevel</span><span class="sxs-lookup"><span data-stu-id="e7301-115">accessLevel</span></span>|[<span data-ttu-id="e7301-116">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="e7301-116">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="e7301-117">Nível de acesso para o Exchange concedido por esta regra.</span><span class="sxs-lookup"><span data-stu-id="e7301-117">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="e7301-118">Os valores possíveis são: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="e7301-118">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7301-119">Relações</span><span class="sxs-lookup"><span data-stu-id="e7301-119">Relationships</span></span>
<span data-ttu-id="e7301-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e7301-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7301-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e7301-121">JSON Representation</span></span>
<span data-ttu-id="e7301-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e7301-122">Here is a JSON representation of the resource.</span></span>
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




