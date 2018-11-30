---
title: Tipo de recurso deviceActionResult
description: Resultado de ação de dispositivo
ms.openlocfilehash: 9d7804b994474778f0f06c52079e09ed5887a09f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006232"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="d2236-103">Tipo de recurso deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="d2236-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="d2236-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d2236-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2236-105">Resultado de ação de dispositivo</span><span class="sxs-lookup"><span data-stu-id="d2236-105">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="d2236-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2236-106">Properties</span></span>
|<span data-ttu-id="d2236-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2236-107">Property</span></span>|<span data-ttu-id="d2236-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2236-108">Type</span></span>|<span data-ttu-id="d2236-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2236-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2236-110">actionName</span><span class="sxs-lookup"><span data-stu-id="d2236-110">actionName</span></span>|<span data-ttu-id="d2236-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d2236-111">String</span></span>|<span data-ttu-id="d2236-112">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="d2236-112">Action name</span></span>|
|<span data-ttu-id="d2236-113">actionState</span><span class="sxs-lookup"><span data-stu-id="d2236-113">actionState</span></span>|[<span data-ttu-id="d2236-114">actionState</span><span class="sxs-lookup"><span data-stu-id="d2236-114">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="d2236-115">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="d2236-115">State of the action.</span></span> <span data-ttu-id="d2236-116">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="d2236-116">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="d2236-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d2236-117">startDateTime</span></span>|<span data-ttu-id="d2236-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2236-118">DateTimeOffset</span></span>|<span data-ttu-id="d2236-119">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="d2236-119">Time the action was initiated</span></span>|
|<span data-ttu-id="d2236-120">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d2236-120">lastUpdatedDateTime</span></span>|<span data-ttu-id="d2236-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2236-121">DateTimeOffset</span></span>|<span data-ttu-id="d2236-122">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="d2236-122">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2236-123">Relações</span><span class="sxs-lookup"><span data-stu-id="d2236-123">Relationships</span></span>
<span data-ttu-id="d2236-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d2236-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d2236-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d2236-125">JSON Representation</span></span>
<span data-ttu-id="d2236-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d2236-126">Here is a JSON representation of the resource.</span></span>
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



