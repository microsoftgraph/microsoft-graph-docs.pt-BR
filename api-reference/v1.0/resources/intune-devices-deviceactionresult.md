---
title: Tipo de recurso deviceActionResult
description: Resultado de ação de dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: be8519adc44f7bb63379b0bfa821a067f3eee947
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985879"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="2c036-103">Tipo de recurso deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="2c036-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="2c036-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2c036-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2c036-105">Resultado de ação de dispositivo</span><span class="sxs-lookup"><span data-stu-id="2c036-105">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="2c036-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2c036-106">Properties</span></span>
|<span data-ttu-id="2c036-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c036-107">Property</span></span>|<span data-ttu-id="2c036-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c036-108">Type</span></span>|<span data-ttu-id="2c036-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c036-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c036-110">actionName</span><span class="sxs-lookup"><span data-stu-id="2c036-110">actionName</span></span>|<span data-ttu-id="2c036-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2c036-111">String</span></span>|<span data-ttu-id="2c036-112">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="2c036-112">Action name</span></span>|
|<span data-ttu-id="2c036-113">actionState</span><span class="sxs-lookup"><span data-stu-id="2c036-113">actionState</span></span>|[<span data-ttu-id="2c036-114">actionState</span><span class="sxs-lookup"><span data-stu-id="2c036-114">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="2c036-115">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="2c036-115">State of the action.</span></span> <span data-ttu-id="2c036-116">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="2c036-116">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="2c036-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2c036-117">startDateTime</span></span>|<span data-ttu-id="2c036-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c036-118">DateTimeOffset</span></span>|<span data-ttu-id="2c036-119">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="2c036-119">Time the action was initiated</span></span>|
|<span data-ttu-id="2c036-120">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c036-120">lastUpdatedDateTime</span></span>|<span data-ttu-id="2c036-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c036-121">DateTimeOffset</span></span>|<span data-ttu-id="2c036-122">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="2c036-122">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c036-123">Relações</span><span class="sxs-lookup"><span data-stu-id="2c036-123">Relationships</span></span>
<span data-ttu-id="2c036-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2c036-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2c036-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2c036-125">JSON Representation</span></span>
<span data-ttu-id="2c036-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2c036-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```



