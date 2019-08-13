---
title: tipo de recurso deviceManagementExchangeAccessRule
description: Regras de acesso do dispositivo no Exchange.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9577ba5acf826598b0cefa6cf884bcc25dc50107
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374201"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="7bfc2-103">tipo de recurso deviceManagementExchangeAccessRule</span><span class="sxs-lookup"><span data-stu-id="7bfc2-103">deviceManagementExchangeAccessRule resource type</span></span>

> <span data-ttu-id="7bfc2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7bfc2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7bfc2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7bfc2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bfc2-106">Regras de acesso do dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="7bfc2-106">Device Access Rules in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="7bfc2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7bfc2-107">Properties</span></span>
|<span data-ttu-id="7bfc2-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7bfc2-108">Property</span></span>|<span data-ttu-id="7bfc2-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bfc2-109">Type</span></span>|<span data-ttu-id="7bfc2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bfc2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bfc2-111">deviceClass</span><span class="sxs-lookup"><span data-stu-id="7bfc2-111">deviceClass</span></span>|[<span data-ttu-id="7bfc2-112">deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="7bfc2-112">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="7bfc2-113">Classe de dispositivo que será afetada por essa regra.</span><span class="sxs-lookup"><span data-stu-id="7bfc2-113">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="7bfc2-114">accessLevel</span><span class="sxs-lookup"><span data-stu-id="7bfc2-114">accessLevel</span></span>|[<span data-ttu-id="7bfc2-115">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="7bfc2-115">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="7bfc2-116">Nível de acesso para o Exchange concedido por esta regra.</span><span class="sxs-lookup"><span data-stu-id="7bfc2-116">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="7bfc2-117">Os valores possíveis são: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="7bfc2-117">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7bfc2-118">Relações</span><span class="sxs-lookup"><span data-stu-id="7bfc2-118">Relationships</span></span>
<span data-ttu-id="7bfc2-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7bfc2-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7bfc2-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7bfc2-120">JSON Representation</span></span>
<span data-ttu-id="7bfc2-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7bfc2-121">Here is a JSON representation of the resource.</span></span>
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



