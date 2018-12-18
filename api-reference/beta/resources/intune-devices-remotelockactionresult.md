---
title: Tipo de recurso remoteLockActionResult
description: Resultado da ação de bloquear com um pin para desbloquear
author: tfitzmac
ms.openlocfilehash: 9cde6019329be909e688bbc1b7a568aa3a9e7781
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324889"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="bac62-103">Tipo de recurso remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="bac62-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="bac62-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bac62-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bac62-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bac62-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bac62-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bac62-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bac62-107">Resultado da ação de bloquear com um pin para desbloquear</span><span class="sxs-lookup"><span data-stu-id="bac62-107">Lock action result with a pin to unlock</span></span>

<span data-ttu-id="bac62-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bac62-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bac62-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bac62-109">Properties</span></span>
|<span data-ttu-id="bac62-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bac62-110">Property</span></span>|<span data-ttu-id="bac62-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="bac62-111">Type</span></span>|<span data-ttu-id="bac62-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="bac62-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bac62-113">actionName</span><span class="sxs-lookup"><span data-stu-id="bac62-113">actionName</span></span>|<span data-ttu-id="bac62-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bac62-114">String</span></span>|<span data-ttu-id="bac62-115">Nome da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bac62-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="bac62-116">actionState</span><span class="sxs-lookup"><span data-stu-id="bac62-116">actionState</span></span>|[<span data-ttu-id="bac62-117">actionState</span><span class="sxs-lookup"><span data-stu-id="bac62-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="bac62-118">Estado da ação Inherited de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="bac62-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="bac62-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="bac62-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="bac62-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bac62-120">startDateTime</span></span>|<span data-ttu-id="bac62-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bac62-121">DateTimeOffset</span></span>|<span data-ttu-id="bac62-122">Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bac62-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="bac62-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="bac62-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="bac62-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bac62-124">DateTimeOffset</span></span>|<span data-ttu-id="bac62-125">Hora em que o estado da ação foi atualizado pela última vez, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bac62-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="bac62-126">unlockPin</span><span class="sxs-lookup"><span data-stu-id="bac62-126">unlockPin</span></span>|<span data-ttu-id="bac62-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bac62-127">String</span></span>|<span data-ttu-id="bac62-128">PIN para desbloquear o cliente</span><span class="sxs-lookup"><span data-stu-id="bac62-128">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="bac62-129">Relações</span><span class="sxs-lookup"><span data-stu-id="bac62-129">Relationships</span></span>
<span data-ttu-id="bac62-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bac62-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bac62-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bac62-131">JSON Representation</span></span>
<span data-ttu-id="bac62-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bac62-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.remoteLockActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteLockActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "unlockPin": "String"
}
```





