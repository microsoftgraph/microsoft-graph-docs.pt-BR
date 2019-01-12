---
title: tipo de recurso de hourlySchedule
description: Agendamento de execução por hora de um script de gerenciamento de dispositivo recorrente.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 004481786fd21ad04e0adbe4e16d3174fc6cc2f4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951884"
---
# <a name="hourlyschedule-resource-type"></a><span data-ttu-id="f2830-103">tipo de recurso de hourlySchedule</span><span class="sxs-lookup"><span data-stu-id="f2830-103">hourlySchedule resource type</span></span>

> <span data-ttu-id="f2830-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f2830-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2830-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f2830-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f2830-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f2830-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f2830-107">Agendamento de execução por hora de um script de gerenciamento de dispositivo recorrente.</span><span class="sxs-lookup"><span data-stu-id="f2830-107">Hourly run schedule of a recurring device management script.</span></span>

<span data-ttu-id="f2830-108">Herda de [runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="f2830-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f2830-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f2830-109">Properties</span></span>
|<span data-ttu-id="f2830-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2830-110">Property</span></span>|<span data-ttu-id="f2830-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2830-111">Type</span></span>|<span data-ttu-id="f2830-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2830-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2830-113">interval</span><span class="sxs-lookup"><span data-stu-id="f2830-113">interval</span></span>|<span data-ttu-id="f2830-114">Int32</span><span class="sxs-lookup"><span data-stu-id="f2830-114">Int32</span></span>|<span data-ttu-id="f2830-115">Intervalo de número de horas</span><span class="sxs-lookup"><span data-stu-id="f2830-115">Interval in number of hours</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2830-116">Relações</span><span class="sxs-lookup"><span data-stu-id="f2830-116">Relationships</span></span>
<span data-ttu-id="f2830-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f2830-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f2830-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f2830-118">JSON Representation</span></span>
<span data-ttu-id="f2830-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f2830-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hourlySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hourlySchedule",
  "interval": 1024
}
```





