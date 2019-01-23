---
title: tipo de recurso de managedDeviceCleanupSettings
description: Defina a regra quando o administrador deseja que os dispositivos devem ser limpos.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4bf756072dcc3cd13bda2fda59b8688b63f3cd43
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424564"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="348c6-103">tipo de recurso de managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="348c6-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="348c6-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="348c6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="348c6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="348c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="348c6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="348c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="348c6-107">Defina a regra quando o administrador deseja que os dispositivos devem ser limpos.</span><span class="sxs-lookup"><span data-stu-id="348c6-107">Define the rule when the admin wants the devices to be cleaned up.</span></span>

## <a name="properties"></a><span data-ttu-id="348c6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="348c6-108">Properties</span></span>
|<span data-ttu-id="348c6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="348c6-109">Property</span></span>|<span data-ttu-id="348c6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="348c6-110">Type</span></span>|<span data-ttu-id="348c6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="348c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="348c6-112">deviceInactivityBeforeRetirementInDays</span><span class="sxs-lookup"><span data-stu-id="348c6-112">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="348c6-113">String</span><span class="sxs-lookup"><span data-stu-id="348c6-113">String</span></span>|<span data-ttu-id="348c6-114">Número de dias quando o dispositivo não foi contatado Intune.</span><span class="sxs-lookup"><span data-stu-id="348c6-114">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="348c6-115">Relações</span><span class="sxs-lookup"><span data-stu-id="348c6-115">Relationships</span></span>
<span data-ttu-id="348c6-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="348c6-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="348c6-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="348c6-117">JSON Representation</span></span>
<span data-ttu-id="348c6-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="348c6-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceCleanupSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceCleanupSettings",
  "deviceInactivityBeforeRetirementInDays": "String"
}
```




