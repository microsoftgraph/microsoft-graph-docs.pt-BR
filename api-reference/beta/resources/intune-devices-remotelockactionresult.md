---
title: Tipo de recurso remoteLockActionResult
description: Resultado da ação de bloquear com um pin para desbloquear
ms.openlocfilehash: 39791c2e20d39a8fced01a16c6cf0cea0c0db4cd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033212"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="a7c81-103">Tipo de recurso remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="a7c81-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="a7c81-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a7c81-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7c81-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a7c81-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a7c81-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a7c81-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7c81-107">Resultado da ação de bloquear com um pin para desbloquear</span><span class="sxs-lookup"><span data-stu-id="a7c81-107">Lock action result with a pin to unlock</span></span>

<span data-ttu-id="a7c81-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a7c81-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a7c81-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a7c81-109">Properties</span></span>
|<span data-ttu-id="a7c81-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a7c81-110">Property</span></span>|<span data-ttu-id="a7c81-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7c81-111">Type</span></span>|<span data-ttu-id="a7c81-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7c81-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7c81-113">actionName</span><span class="sxs-lookup"><span data-stu-id="a7c81-113">actionName</span></span>|<span data-ttu-id="a7c81-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a7c81-114">String</span></span>|<span data-ttu-id="a7c81-115">Nome da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a7c81-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a7c81-116">actionState</span><span class="sxs-lookup"><span data-stu-id="a7c81-116">actionState</span></span>|[<span data-ttu-id="a7c81-117">actionState</span><span class="sxs-lookup"><span data-stu-id="a7c81-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="a7c81-118">Estado da ação Inherited de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="a7c81-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="a7c81-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="a7c81-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="a7c81-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a7c81-120">startDateTime</span></span>|<span data-ttu-id="a7c81-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7c81-121">DateTimeOffset</span></span>|<span data-ttu-id="a7c81-122">Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a7c81-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a7c81-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="a7c81-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="a7c81-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7c81-124">DateTimeOffset</span></span>|<span data-ttu-id="a7c81-125">Hora em que o estado da ação foi atualizado pela última vez, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a7c81-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a7c81-126">unlockPin</span><span class="sxs-lookup"><span data-stu-id="a7c81-126">unlockPin</span></span>|<span data-ttu-id="a7c81-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a7c81-127">String</span></span>|<span data-ttu-id="a7c81-128">PIN para desbloquear o cliente</span><span class="sxs-lookup"><span data-stu-id="a7c81-128">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7c81-129">Relações</span><span class="sxs-lookup"><span data-stu-id="a7c81-129">Relationships</span></span>
<span data-ttu-id="a7c81-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a7c81-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a7c81-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a7c81-131">JSON Representation</span></span>
<span data-ttu-id="a7c81-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a7c81-132">Here is a JSON representation of the resource.</span></span>
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





