---
title: tipo de recurso deviceManagementExchangeAccessRule
description: Regras de acesso do dispositivo no Exchange.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 832e11829300ccd1ac4e1d4e6b08acafb908f3b2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566602"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="f6ba4-103">tipo de recurso deviceManagementExchangeAccessRule</span><span class="sxs-lookup"><span data-stu-id="f6ba4-103">deviceManagementExchangeAccessRule resource type</span></span>

> <span data-ttu-id="f6ba4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f6ba4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6ba4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f6ba4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6ba4-106">Regras de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6ba4-106">Device Access Rules in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="f6ba4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f6ba4-107">Properties</span></span>
|<span data-ttu-id="f6ba4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f6ba4-108">Property</span></span>|<span data-ttu-id="f6ba4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6ba4-109">Type</span></span>|<span data-ttu-id="f6ba4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6ba4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6ba4-111">deviceClass</span><span class="sxs-lookup"><span data-stu-id="f6ba4-111">deviceClass</span></span>|[<span data-ttu-id="f6ba4-112">deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="f6ba4-112">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="f6ba4-113">Classe de dispositivo que será afetada por essa regra.</span><span class="sxs-lookup"><span data-stu-id="f6ba4-113">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="f6ba4-114">accessLevel</span><span class="sxs-lookup"><span data-stu-id="f6ba4-114">accessLevel</span></span>|[<span data-ttu-id="f6ba4-115">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="f6ba4-115">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="f6ba4-116">Nível de acesso para o Exchange concedido por esta regra.</span><span class="sxs-lookup"><span data-stu-id="f6ba4-116">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="f6ba4-117">Os valores possíveis são: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="f6ba4-117">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6ba4-118">Relações</span><span class="sxs-lookup"><span data-stu-id="f6ba4-118">Relationships</span></span>
<span data-ttu-id="f6ba4-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f6ba4-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6ba4-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f6ba4-120">JSON Representation</span></span>
<span data-ttu-id="f6ba4-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f6ba4-121">Here is a JSON representation of the resource.</span></span>
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





