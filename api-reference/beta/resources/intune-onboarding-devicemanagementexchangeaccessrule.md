---
title: tipo de recurso deviceManagementExchangeAccessRule
description: Regras de acesso do dispositivo no Exchange.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1a9a7fe3474f53b7107fb7fe35c1a80f743cfb7b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697228"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="4ff9a-103">tipo de recurso deviceManagementExchangeAccessRule</span><span class="sxs-lookup"><span data-stu-id="4ff9a-103">deviceManagementExchangeAccessRule resource type</span></span>

<span data-ttu-id="4ff9a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ff9a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ff9a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4ff9a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ff9a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4ff9a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ff9a-107">Regras de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="4ff9a-107">Device Access Rules in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="4ff9a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4ff9a-108">Properties</span></span>
|<span data-ttu-id="4ff9a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ff9a-109">Property</span></span>|<span data-ttu-id="4ff9a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ff9a-110">Type</span></span>|<span data-ttu-id="4ff9a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ff9a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ff9a-112">deviceClass</span><span class="sxs-lookup"><span data-stu-id="4ff9a-112">deviceClass</span></span>|[<span data-ttu-id="4ff9a-113">deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="4ff9a-113">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="4ff9a-114">Classe de dispositivo que será afetada por essa regra.</span><span class="sxs-lookup"><span data-stu-id="4ff9a-114">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="4ff9a-115">accessLevel</span><span class="sxs-lookup"><span data-stu-id="4ff9a-115">accessLevel</span></span>|[<span data-ttu-id="4ff9a-116">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="4ff9a-116">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="4ff9a-117">Nível de acesso para o Exchange concedido por esta regra.</span><span class="sxs-lookup"><span data-stu-id="4ff9a-117">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="4ff9a-118">Os valores possíveis são: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="4ff9a-118">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ff9a-119">Relações</span><span class="sxs-lookup"><span data-stu-id="4ff9a-119">Relationships</span></span>
<span data-ttu-id="4ff9a-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4ff9a-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ff9a-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4ff9a-121">JSON Representation</span></span>
<span data-ttu-id="4ff9a-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4ff9a-122">Here is a JSON representation of the resource.</span></span>
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





