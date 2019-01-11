---
title: tipo de recurso de dailySchedule
description: Agenda diária de execução de um script de gerenciamento de dispositivo recorrente.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5321bce51f0f682591c6b27a0acec4ed95d0e2e8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840555"
---
# <a name="dailyschedule-resource-type"></a><span data-ttu-id="06e14-103">tipo de recurso de dailySchedule</span><span class="sxs-lookup"><span data-stu-id="06e14-103">dailySchedule resource type</span></span>

> <span data-ttu-id="06e14-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="06e14-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06e14-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="06e14-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06e14-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="06e14-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06e14-107">Agenda diária de execução de um script de gerenciamento de dispositivo recorrente.</span><span class="sxs-lookup"><span data-stu-id="06e14-107">Daily run schedule of a recurring device management script.</span></span>

<span data-ttu-id="06e14-108">Herda de [runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="06e14-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="06e14-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="06e14-109">Properties</span></span>
|<span data-ttu-id="06e14-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06e14-110">Property</span></span>|<span data-ttu-id="06e14-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="06e14-111">Type</span></span>|<span data-ttu-id="06e14-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="06e14-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06e14-113">interval</span><span class="sxs-lookup"><span data-stu-id="06e14-113">interval</span></span>|<span data-ttu-id="06e14-114">Int32</span><span class="sxs-lookup"><span data-stu-id="06e14-114">Int32</span></span>|<span data-ttu-id="06e14-115">Intervalo de número de dias</span><span class="sxs-lookup"><span data-stu-id="06e14-115">Interval in number of days</span></span>|

## <a name="relationships"></a><span data-ttu-id="06e14-116">Relações</span><span class="sxs-lookup"><span data-stu-id="06e14-116">Relationships</span></span>
<span data-ttu-id="06e14-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="06e14-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="06e14-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="06e14-118">JSON Representation</span></span>
<span data-ttu-id="06e14-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="06e14-119">Here is a JSON representation of the resource.</span></span>
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





