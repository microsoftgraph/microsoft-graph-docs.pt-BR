---
title: tipo de recurso managedDeviceCleanupSettings
description: Defina a regra quando o administrador quiser que os dispositivos sejam limpos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 67e911cb5e1b31e3be2cc20378ebe77ff305204a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725481"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="198e8-103">tipo de recurso managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="198e8-103">managedDeviceCleanupSettings resource type</span></span>

<span data-ttu-id="198e8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="198e8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="198e8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="198e8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="198e8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="198e8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="198e8-107">Defina a regra quando o administrador quiser que os dispositivos sejam limpos.</span><span class="sxs-lookup"><span data-stu-id="198e8-107">Define the rule when the admin wants the devices to be cleaned up.</span></span>

## <a name="properties"></a><span data-ttu-id="198e8-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="198e8-108">Properties</span></span>
|<span data-ttu-id="198e8-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="198e8-109">Property</span></span>|<span data-ttu-id="198e8-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="198e8-110">Type</span></span>|<span data-ttu-id="198e8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="198e8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="198e8-112">deviceInactivityBeforeRetirementInDays</span><span class="sxs-lookup"><span data-stu-id="198e8-112">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="198e8-113">String</span><span class="sxs-lookup"><span data-stu-id="198e8-113">String</span></span>|<span data-ttu-id="198e8-114">Número de dias em que o dispositivo não entrou no Intune.</span><span class="sxs-lookup"><span data-stu-id="198e8-114">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="198e8-115">Relações</span><span class="sxs-lookup"><span data-stu-id="198e8-115">Relationships</span></span>
<span data-ttu-id="198e8-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="198e8-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="198e8-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="198e8-117">JSON Representation</span></span>
<span data-ttu-id="198e8-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="198e8-118">Here is a JSON representation of the resource.</span></span>
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





