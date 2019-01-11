---
title: tipo de recurso de deviceManagementExchangeDeviceClass
description: Classe de dispositivo no Exchange.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 80142f4e05752a37c324cd20ce96e4c8e6668c03
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839022"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="60aff-103">tipo de recurso de deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="60aff-103">deviceManagementExchangeDeviceClass resource type</span></span>

> <span data-ttu-id="60aff-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="60aff-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60aff-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="60aff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="60aff-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="60aff-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="60aff-107">Classe de dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="60aff-107">Device Class in Exchange.</span></span>
## <a name="properties"></a><span data-ttu-id="60aff-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="60aff-108">Properties</span></span>
|<span data-ttu-id="60aff-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60aff-109">Property</span></span>|<span data-ttu-id="60aff-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="60aff-110">Type</span></span>|<span data-ttu-id="60aff-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="60aff-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60aff-112">name</span><span class="sxs-lookup"><span data-stu-id="60aff-112">name</span></span>|<span data-ttu-id="60aff-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="60aff-113">String</span></span>|<span data-ttu-id="60aff-114">Nome da classe do dispositivo que será afetada por essa regra.</span><span class="sxs-lookup"><span data-stu-id="60aff-114">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="60aff-115">type</span><span class="sxs-lookup"><span data-stu-id="60aff-115">type</span></span>|[<span data-ttu-id="60aff-116">deviceManagementExchangeAccessRuleType</span><span class="sxs-lookup"><span data-stu-id="60aff-116">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="60aff-117">Tipo de dispositivo que é afetado por esta regra modelar p. ex., família.</span><span class="sxs-lookup"><span data-stu-id="60aff-117">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="60aff-118">Os valores possíveis são: `family`, `model`.</span><span class="sxs-lookup"><span data-stu-id="60aff-118">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60aff-119">Relações</span><span class="sxs-lookup"><span data-stu-id="60aff-119">Relationships</span></span>
<span data-ttu-id="60aff-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="60aff-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="60aff-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="60aff-121">JSON Representation</span></span>
<span data-ttu-id="60aff-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="60aff-122">Here is a JSON representation of the resource.</span></span>
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





