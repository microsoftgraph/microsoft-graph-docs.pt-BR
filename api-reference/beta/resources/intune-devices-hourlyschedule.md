---
title: tipo de recurso de hourlySchedule
description: Agendamento de execução por hora de um script de gerenciamento de dispositivo recorrente.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cf62c11da0932f5f10b6cc7a76ccecfd1e74ee92
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396823"
---
# <a name="hourlyschedule-resource-type"></a><span data-ttu-id="fe5bc-103">tipo de recurso de hourlySchedule</span><span class="sxs-lookup"><span data-stu-id="fe5bc-103">hourlySchedule resource type</span></span>

> <span data-ttu-id="fe5bc-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="fe5bc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fe5bc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fe5bc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fe5bc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="fe5bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe5bc-107">Agendamento de execução por hora de um script de gerenciamento de dispositivo recorrente.</span><span class="sxs-lookup"><span data-stu-id="fe5bc-107">Hourly run schedule of a recurring device management script.</span></span>


<span data-ttu-id="fe5bc-108">Herda de [runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="fe5bc-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fe5bc-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fe5bc-109">Properties</span></span>
|<span data-ttu-id="fe5bc-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe5bc-110">Property</span></span>|<span data-ttu-id="fe5bc-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe5bc-111">Type</span></span>|<span data-ttu-id="fe5bc-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe5bc-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe5bc-113">interval</span><span class="sxs-lookup"><span data-stu-id="fe5bc-113">interval</span></span>|<span data-ttu-id="fe5bc-114">Int32</span><span class="sxs-lookup"><span data-stu-id="fe5bc-114">Int32</span></span>|<span data-ttu-id="fe5bc-115">Intervalo de número de horas</span><span class="sxs-lookup"><span data-stu-id="fe5bc-115">Interval in number of hours</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe5bc-116">Relações</span><span class="sxs-lookup"><span data-stu-id="fe5bc-116">Relationships</span></span>
<span data-ttu-id="fe5bc-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fe5bc-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe5bc-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fe5bc-118">JSON Representation</span></span>
<span data-ttu-id="fe5bc-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fe5bc-119">Here is a JSON representation of the resource.</span></span>
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




