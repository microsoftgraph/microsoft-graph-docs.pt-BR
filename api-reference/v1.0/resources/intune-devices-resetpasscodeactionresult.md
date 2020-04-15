---
title: tipo de recurso resetPasscodeActionResult
description: Resultado de ação de redefinir a senha
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d8510dcb20fa0af50df1db24927b97c32afb1188
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439439"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="b857d-103">tipo de recurso resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="b857d-103">resetPasscodeActionResult resource type</span></span>

<span data-ttu-id="b857d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b857d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b857d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b857d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b857d-106">Resultado da ação de redefinir a senha</span><span class="sxs-lookup"><span data-stu-id="b857d-106">Reset passcode action result</span></span>


<span data-ttu-id="b857d-107">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b857d-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b857d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b857d-108">Properties</span></span>
|<span data-ttu-id="b857d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b857d-109">Property</span></span>|<span data-ttu-id="b857d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b857d-110">Type</span></span>|<span data-ttu-id="b857d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b857d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b857d-112">actionName</span><span class="sxs-lookup"><span data-stu-id="b857d-112">actionName</span></span>|<span data-ttu-id="b857d-113">String</span><span class="sxs-lookup"><span data-stu-id="b857d-113">String</span></span>|<span data-ttu-id="b857d-114">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b857d-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b857d-115">actionState</span><span class="sxs-lookup"><span data-stu-id="b857d-115">actionState</span></span>|[<span data-ttu-id="b857d-116">actionState</span><span class="sxs-lookup"><span data-stu-id="b857d-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="b857d-117">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="b857d-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="b857d-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="b857d-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="b857d-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b857d-119">startDateTime</span></span>|<span data-ttu-id="b857d-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b857d-120">DateTimeOffset</span></span>|<span data-ttu-id="b857d-121">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b857d-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b857d-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b857d-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="b857d-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b857d-123">DateTimeOffset</span></span>|<span data-ttu-id="b857d-124">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b857d-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b857d-125">senha</span><span class="sxs-lookup"><span data-stu-id="b857d-125">passcode</span></span>|<span data-ttu-id="b857d-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b857d-126">String</span></span>|<span data-ttu-id="b857d-127">Senha recentemente gerada para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="b857d-127">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="b857d-128">Relações</span><span class="sxs-lookup"><span data-stu-id="b857d-128">Relationships</span></span>
<span data-ttu-id="b857d-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b857d-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b857d-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b857d-130">JSON Representation</span></span>
<span data-ttu-id="b857d-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b857d-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resetPasscodeActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resetPasscodeActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "passcode": "String"
}
```







