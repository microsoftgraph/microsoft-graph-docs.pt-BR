---
title: tipo de recurso de deviceManagementExchangeDeviceClass
description: Classe de dispositivo no Exchange.
ms.openlocfilehash: 53234a97ffd2581eea1a4c480161ec9243a710d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039894"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="0bb30-103">tipo de recurso de deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="0bb30-103">deviceManagementExchangeDeviceClass resource type</span></span>

> <span data-ttu-id="0bb30-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0bb30-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0bb30-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0bb30-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0bb30-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0bb30-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0bb30-107">Classe de dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="0bb30-107">Device Class in Exchange.</span></span>
## <a name="properties"></a><span data-ttu-id="0bb30-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0bb30-108">Properties</span></span>
|<span data-ttu-id="0bb30-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0bb30-109">Property</span></span>|<span data-ttu-id="0bb30-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0bb30-110">Type</span></span>|<span data-ttu-id="0bb30-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bb30-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bb30-112">name</span><span class="sxs-lookup"><span data-stu-id="0bb30-112">name</span></span>|<span data-ttu-id="0bb30-113">String</span><span class="sxs-lookup"><span data-stu-id="0bb30-113">String</span></span>|<span data-ttu-id="0bb30-114">Nome da classe do dispositivo que será afetada por essa regra.</span><span class="sxs-lookup"><span data-stu-id="0bb30-114">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="0bb30-115">type</span><span class="sxs-lookup"><span data-stu-id="0bb30-115">type</span></span>|[<span data-ttu-id="0bb30-116">deviceManagementExchangeAccessRuleType</span><span class="sxs-lookup"><span data-stu-id="0bb30-116">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="0bb30-117">Tipo de dispositivo que é afetado por esta regra modelar p. ex., família.</span><span class="sxs-lookup"><span data-stu-id="0bb30-117">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="0bb30-118">Os valores possíveis são: `family`, `model`.</span><span class="sxs-lookup"><span data-stu-id="0bb30-118">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0bb30-119">Relações</span><span class="sxs-lookup"><span data-stu-id="0bb30-119">Relationships</span></span>
<span data-ttu-id="0bb30-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0bb30-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0bb30-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0bb30-121">JSON Representation</span></span>
<span data-ttu-id="0bb30-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0bb30-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeDeviceClass",
  "name": "String",
  "type": "String"
}
```





