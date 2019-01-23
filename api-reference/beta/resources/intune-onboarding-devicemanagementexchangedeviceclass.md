---
title: tipo de recurso de deviceManagementExchangeDeviceClass
description: Classe de dispositivo no Exchange.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3e512253a9b9bc4228d41c369501bec1e7a5e031
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413728"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="dd8c6-103">tipo de recurso de deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="dd8c6-103">deviceManagementExchangeDeviceClass resource type</span></span>

> <span data-ttu-id="dd8c6-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="dd8c6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="dd8c6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dd8c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dd8c6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="dd8c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd8c6-107">Classe de dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="dd8c6-107">Device Class in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="dd8c6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dd8c6-108">Properties</span></span>
|<span data-ttu-id="dd8c6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd8c6-109">Property</span></span>|<span data-ttu-id="dd8c6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd8c6-110">Type</span></span>|<span data-ttu-id="dd8c6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd8c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd8c6-112">name</span><span class="sxs-lookup"><span data-stu-id="dd8c6-112">name</span></span>|<span data-ttu-id="dd8c6-113">String</span><span class="sxs-lookup"><span data-stu-id="dd8c6-113">String</span></span>|<span data-ttu-id="dd8c6-114">Nome da classe do dispositivo que será afetada por essa regra.</span><span class="sxs-lookup"><span data-stu-id="dd8c6-114">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="dd8c6-115">type</span><span class="sxs-lookup"><span data-stu-id="dd8c6-115">type</span></span>|[<span data-ttu-id="dd8c6-116">deviceManagementExchangeAccessRuleType</span><span class="sxs-lookup"><span data-stu-id="dd8c6-116">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="dd8c6-117">Tipo de dispositivo que é afetado por esta regra modelar p. ex., família.</span><span class="sxs-lookup"><span data-stu-id="dd8c6-117">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="dd8c6-118">Os valores possíveis são: `family`, `model`.</span><span class="sxs-lookup"><span data-stu-id="dd8c6-118">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd8c6-119">Relações</span><span class="sxs-lookup"><span data-stu-id="dd8c6-119">Relationships</span></span>
<span data-ttu-id="dd8c6-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dd8c6-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd8c6-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dd8c6-121">JSON Representation</span></span>
<span data-ttu-id="dd8c6-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dd8c6-122">Here is a JSON representation of the resource.</span></span>
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




