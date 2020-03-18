---
title: tipo de recurso deviceManagementExchangeAccessRule
description: Regras de acesso do dispositivo no Exchange.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a6d32744d2fd3cb48f52c85b314e72d50983dffc
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42779188"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="c2ac2-103">tipo de recurso deviceManagementExchangeAccessRule</span><span class="sxs-lookup"><span data-stu-id="c2ac2-103">deviceManagementExchangeAccessRule resource type</span></span>

> <span data-ttu-id="c2ac2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c2ac2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2ac2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c2ac2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2ac2-106">Regras de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="c2ac2-106">Device Access Rules in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="c2ac2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c2ac2-107">Properties</span></span>
|<span data-ttu-id="c2ac2-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c2ac2-108">Property</span></span>|<span data-ttu-id="c2ac2-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c2ac2-109">Type</span></span>|<span data-ttu-id="c2ac2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2ac2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2ac2-111">deviceClass</span><span class="sxs-lookup"><span data-stu-id="c2ac2-111">deviceClass</span></span>|[<span data-ttu-id="c2ac2-112">deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="c2ac2-112">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="c2ac2-113">Classe de dispositivo que será afetada por essa regra.</span><span class="sxs-lookup"><span data-stu-id="c2ac2-113">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="c2ac2-114">accessLevel</span><span class="sxs-lookup"><span data-stu-id="c2ac2-114">accessLevel</span></span>|[<span data-ttu-id="c2ac2-115">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="c2ac2-115">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="c2ac2-116">Nível de acesso para o Exchange concedido por esta regra.</span><span class="sxs-lookup"><span data-stu-id="c2ac2-116">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="c2ac2-117">Os valores possíveis são: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="c2ac2-117">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2ac2-118">Relações</span><span class="sxs-lookup"><span data-stu-id="c2ac2-118">Relationships</span></span>
<span data-ttu-id="c2ac2-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c2ac2-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2ac2-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c2ac2-120">JSON Representation</span></span>
<span data-ttu-id="c2ac2-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c2ac2-121">Here is a JSON representation of the resource.</span></span>
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



