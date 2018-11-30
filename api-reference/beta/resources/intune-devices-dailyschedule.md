---
title: tipo de recurso de dailySchedule
description: Agenda diária de execução de um script de gerenciamento de dispositivo recorrente.
ms.openlocfilehash: 5d517b0bcd15f041b934a0ca936075bc6d3d3741
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038809"
---
# <a name="dailyschedule-resource-type"></a><span data-ttu-id="a8494-103">tipo de recurso de dailySchedule</span><span class="sxs-lookup"><span data-stu-id="a8494-103">dailySchedule resource type</span></span>

> <span data-ttu-id="a8494-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a8494-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8494-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a8494-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8494-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a8494-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8494-107">Agenda diária de execução de um script de gerenciamento de dispositivo recorrente.</span><span class="sxs-lookup"><span data-stu-id="a8494-107">Daily run schedule of a recurring device management script.</span></span>

<span data-ttu-id="a8494-108">Herda de [runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="a8494-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a8494-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8494-109">Properties</span></span>
|<span data-ttu-id="a8494-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8494-110">Property</span></span>|<span data-ttu-id="a8494-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8494-111">Type</span></span>|<span data-ttu-id="a8494-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8494-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8494-113">interval</span><span class="sxs-lookup"><span data-stu-id="a8494-113">interval</span></span>|<span data-ttu-id="a8494-114">Int32</span><span class="sxs-lookup"><span data-stu-id="a8494-114">Int32</span></span>|<span data-ttu-id="a8494-115">Intervalo de número de dias</span><span class="sxs-lookup"><span data-stu-id="a8494-115">Interval in number of days</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8494-116">Relações</span><span class="sxs-lookup"><span data-stu-id="a8494-116">Relationships</span></span>
<span data-ttu-id="a8494-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a8494-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a8494-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8494-118">JSON Representation</span></span>
<span data-ttu-id="a8494-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a8494-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.dailySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dailySchedule",
  "interval": 1024
}
```





