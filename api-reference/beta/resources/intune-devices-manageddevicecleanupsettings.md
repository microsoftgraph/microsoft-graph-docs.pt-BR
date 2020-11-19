---
title: tipo de recurso managedDeviceCleanupSettings
description: Defina a regra quando o administrador quiser que os dispositivos sejam limpos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 062f8a428155a7246e9ac6a372d95aa7ebe42717
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267366"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="d79c9-103">tipo de recurso managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="d79c9-103">managedDeviceCleanupSettings resource type</span></span>

<span data-ttu-id="d79c9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d79c9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d79c9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d79c9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d79c9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d79c9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d79c9-107">Defina a regra quando o administrador quiser que os dispositivos sejam limpos.</span><span class="sxs-lookup"><span data-stu-id="d79c9-107">Define the rule when the admin wants the devices to be cleaned up.</span></span>

## <a name="properties"></a><span data-ttu-id="d79c9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d79c9-108">Properties</span></span>
|<span data-ttu-id="d79c9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d79c9-109">Property</span></span>|<span data-ttu-id="d79c9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d79c9-110">Type</span></span>|<span data-ttu-id="d79c9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d79c9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d79c9-112">deviceInactivityBeforeRetirementInDays</span><span class="sxs-lookup"><span data-stu-id="d79c9-112">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="d79c9-113">String</span><span class="sxs-lookup"><span data-stu-id="d79c9-113">String</span></span>|<span data-ttu-id="d79c9-114">Número de dias em que o dispositivo não entrou no Intune.</span><span class="sxs-lookup"><span data-stu-id="d79c9-114">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d79c9-115">Relações</span><span class="sxs-lookup"><span data-stu-id="d79c9-115">Relationships</span></span>
<span data-ttu-id="d79c9-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d79c9-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d79c9-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d79c9-117">JSON Representation</span></span>
<span data-ttu-id="d79c9-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d79c9-118">Here is a JSON representation of the resource.</span></span>
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




