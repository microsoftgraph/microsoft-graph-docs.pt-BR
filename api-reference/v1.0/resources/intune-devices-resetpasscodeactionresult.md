---
title: tipo de recurso resetPasscodeActionResult
description: Resultado da ação de redefinir a senha
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e526370ca86792ed30a5f5e24a4be244d73441b6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920839"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="48ecb-103">tipo de recurso resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="48ecb-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="48ecb-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="48ecb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="48ecb-105">Resultado da ação de redefinir a senha</span><span class="sxs-lookup"><span data-stu-id="48ecb-105">Reset passcode action result</span></span>

<span data-ttu-id="48ecb-106">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="48ecb-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="48ecb-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="48ecb-107">Properties</span></span>
|<span data-ttu-id="48ecb-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48ecb-108">Property</span></span>|<span data-ttu-id="48ecb-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="48ecb-109">Type</span></span>|<span data-ttu-id="48ecb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="48ecb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48ecb-111">actionName</span><span class="sxs-lookup"><span data-stu-id="48ecb-111">actionName</span></span>|<span data-ttu-id="48ecb-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="48ecb-112">String</span></span>|<span data-ttu-id="48ecb-113">Nome da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="48ecb-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="48ecb-114">actionState</span><span class="sxs-lookup"><span data-stu-id="48ecb-114">actionState</span></span>|[<span data-ttu-id="48ecb-115">actionState</span><span class="sxs-lookup"><span data-stu-id="48ecb-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="48ecb-116">Estado da ação Inherited de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="48ecb-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="48ecb-117">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="48ecb-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="48ecb-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="48ecb-118">startDateTime</span></span>|<span data-ttu-id="48ecb-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48ecb-119">DateTimeOffset</span></span>|<span data-ttu-id="48ecb-120">Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="48ecb-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="48ecb-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="48ecb-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="48ecb-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48ecb-122">DateTimeOffset</span></span>|<span data-ttu-id="48ecb-123">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="48ecb-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="48ecb-124">senha</span><span class="sxs-lookup"><span data-stu-id="48ecb-124">passcode</span></span>|<span data-ttu-id="48ecb-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="48ecb-125">String</span></span>|<span data-ttu-id="48ecb-126">Senha recentemente gerada para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="48ecb-126">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="48ecb-127">Relações</span><span class="sxs-lookup"><span data-stu-id="48ecb-127">Relationships</span></span>
<span data-ttu-id="48ecb-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="48ecb-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="48ecb-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="48ecb-129">JSON Representation</span></span>
<span data-ttu-id="48ecb-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="48ecb-130">Here is a JSON representation of the resource.</span></span>
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



