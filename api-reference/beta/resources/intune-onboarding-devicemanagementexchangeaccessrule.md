---
title: tipo de recurso de deviceManagementExchangeAccessRule
description: Regras de acesso de dispositivo no Exchange.
ms.openlocfilehash: e59c81fdfe6cb6a0a7f7f952e6bfc8929bbc2633
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036104"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="eeee1-103">tipo de recurso de deviceManagementExchangeAccessRule</span><span class="sxs-lookup"><span data-stu-id="eeee1-103">deviceManagementExchangeAccessRule resource type</span></span>

> <span data-ttu-id="eeee1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="eeee1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eeee1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="eeee1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eeee1-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="eeee1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eeee1-107">Regras de acesso de dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="eeee1-107">Device Access Rules in Exchange.</span></span>
## <a name="properties"></a><span data-ttu-id="eeee1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eeee1-108">Properties</span></span>
|<span data-ttu-id="eeee1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eeee1-109">Property</span></span>|<span data-ttu-id="eeee1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="eeee1-110">Type</span></span>|<span data-ttu-id="eeee1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="eeee1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eeee1-112">deviceClass</span><span class="sxs-lookup"><span data-stu-id="eeee1-112">deviceClass</span></span>|[<span data-ttu-id="eeee1-113">deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="eeee1-113">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="eeee1-114">Classe de dispositivo que será afetado por essa regra.</span><span class="sxs-lookup"><span data-stu-id="eeee1-114">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="eeee1-115">accessLevel</span><span class="sxs-lookup"><span data-stu-id="eeee1-115">accessLevel</span></span>|[<span data-ttu-id="eeee1-116">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="eeee1-116">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="eeee1-117">Nível de acesso para o Exchange concedida por esta regra.</span><span class="sxs-lookup"><span data-stu-id="eeee1-117">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="eeee1-118">Os valores possíveis são: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="eeee1-118">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eeee1-119">Relações</span><span class="sxs-lookup"><span data-stu-id="eeee1-119">Relationships</span></span>
<span data-ttu-id="eeee1-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eeee1-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="eeee1-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eeee1-121">JSON Representation</span></span>
<span data-ttu-id="eeee1-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eeee1-122">Here is a JSON representation of the resource.</span></span>
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





