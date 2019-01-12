---
title: tipo de recurso de deviceManagementExchangeAccessRule
description: Regras de acesso de dispositivo no Exchange.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a03fb9f56361cc72bd0321a3b2bd548571740b34
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927811"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="77899-103">tipo de recurso de deviceManagementExchangeAccessRule</span><span class="sxs-lookup"><span data-stu-id="77899-103">deviceManagementExchangeAccessRule resource type</span></span>

> <span data-ttu-id="77899-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="77899-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77899-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="77899-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="77899-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="77899-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="77899-107">Regras de acesso de dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="77899-107">Device Access Rules in Exchange.</span></span>
## <a name="properties"></a><span data-ttu-id="77899-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="77899-108">Properties</span></span>
|<span data-ttu-id="77899-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="77899-109">Property</span></span>|<span data-ttu-id="77899-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="77899-110">Type</span></span>|<span data-ttu-id="77899-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="77899-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77899-112">deviceClass</span><span class="sxs-lookup"><span data-stu-id="77899-112">deviceClass</span></span>|[<span data-ttu-id="77899-113">deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="77899-113">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="77899-114">Classe de dispositivo que será afetado por essa regra.</span><span class="sxs-lookup"><span data-stu-id="77899-114">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="77899-115">accessLevel</span><span class="sxs-lookup"><span data-stu-id="77899-115">accessLevel</span></span>|[<span data-ttu-id="77899-116">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="77899-116">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="77899-117">Nível de acesso para o Exchange concedida por esta regra.</span><span class="sxs-lookup"><span data-stu-id="77899-117">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="77899-118">Os valores possíveis são: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="77899-118">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="77899-119">Relações</span><span class="sxs-lookup"><span data-stu-id="77899-119">Relationships</span></span>
<span data-ttu-id="77899-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="77899-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="77899-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="77899-121">JSON Representation</span></span>
<span data-ttu-id="77899-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="77899-122">Here is a JSON representation of the resource.</span></span>
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





