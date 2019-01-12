---
title: tipo de recurso de deviceManagementExchangeDeviceClass
description: Classe de dispositivo no Exchange.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fcc46cf2744563108a7f063faf5fffbfda172394
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986618"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="0c20d-103">tipo de recurso de deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="0c20d-103">deviceManagementExchangeDeviceClass resource type</span></span>

> <span data-ttu-id="0c20d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0c20d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c20d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0c20d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c20d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0c20d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c20d-107">Classe de dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="0c20d-107">Device Class in Exchange.</span></span>
## <a name="properties"></a><span data-ttu-id="0c20d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0c20d-108">Properties</span></span>
|<span data-ttu-id="0c20d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c20d-109">Property</span></span>|<span data-ttu-id="0c20d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c20d-110">Type</span></span>|<span data-ttu-id="0c20d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c20d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c20d-112">name</span><span class="sxs-lookup"><span data-stu-id="0c20d-112">name</span></span>|<span data-ttu-id="0c20d-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c20d-113">String</span></span>|<span data-ttu-id="0c20d-114">Nome da classe do dispositivo que será afetada por essa regra.</span><span class="sxs-lookup"><span data-stu-id="0c20d-114">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="0c20d-115">type</span><span class="sxs-lookup"><span data-stu-id="0c20d-115">type</span></span>|[<span data-ttu-id="0c20d-116">deviceManagementExchangeAccessRuleType</span><span class="sxs-lookup"><span data-stu-id="0c20d-116">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="0c20d-117">Tipo de dispositivo que é afetado por esta regra modelar p. ex., família.</span><span class="sxs-lookup"><span data-stu-id="0c20d-117">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="0c20d-118">Os valores possíveis são: `family`, `model`.</span><span class="sxs-lookup"><span data-stu-id="0c20d-118">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c20d-119">Relações</span><span class="sxs-lookup"><span data-stu-id="0c20d-119">Relationships</span></span>
<span data-ttu-id="0c20d-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0c20d-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0c20d-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0c20d-121">JSON Representation</span></span>
<span data-ttu-id="0c20d-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0c20d-122">Here is a JSON representation of the resource.</span></span>
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





