---
title: tipo de recurso resetPasscodeActionResult
description: Resultado de ação de redefinir a senha
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4f7d6c3c8f2d339fa499fe09b5b1981833b2f020
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31797673"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="5afa1-103">tipo de recurso resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="5afa1-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="5afa1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5afa1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5afa1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5afa1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5afa1-106">Resultado da ação de redefinir a senha</span><span class="sxs-lookup"><span data-stu-id="5afa1-106">Reset passcode action result</span></span>


<span data-ttu-id="5afa1-107">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="5afa1-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5afa1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5afa1-108">Properties</span></span>
|<span data-ttu-id="5afa1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5afa1-109">Property</span></span>|<span data-ttu-id="5afa1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5afa1-110">Type</span></span>|<span data-ttu-id="5afa1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5afa1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5afa1-112">actionName</span><span class="sxs-lookup"><span data-stu-id="5afa1-112">actionName</span></span>|<span data-ttu-id="5afa1-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5afa1-113">String</span></span>|<span data-ttu-id="5afa1-114">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="5afa1-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="5afa1-115">actionState</span><span class="sxs-lookup"><span data-stu-id="5afa1-115">actionState</span></span>|[<span data-ttu-id="5afa1-116">actionState</span><span class="sxs-lookup"><span data-stu-id="5afa1-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="5afa1-117">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="5afa1-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="5afa1-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="5afa1-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="5afa1-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5afa1-119">startDateTime</span></span>|<span data-ttu-id="5afa1-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5afa1-120">DateTimeOffset</span></span>|<span data-ttu-id="5afa1-121">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="5afa1-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="5afa1-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="5afa1-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="5afa1-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5afa1-123">DateTimeOffset</span></span>|<span data-ttu-id="5afa1-124">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="5afa1-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="5afa1-125">senha</span><span class="sxs-lookup"><span data-stu-id="5afa1-125">passcode</span></span>|<span data-ttu-id="5afa1-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5afa1-126">String</span></span>|<span data-ttu-id="5afa1-127">Senha recentemente gerada para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="5afa1-127">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="5afa1-128">Relações</span><span class="sxs-lookup"><span data-stu-id="5afa1-128">Relationships</span></span>
<span data-ttu-id="5afa1-129">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="5afa1-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5afa1-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5afa1-130">JSON Representation</span></span>
<span data-ttu-id="5afa1-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5afa1-131">Here is a JSON representation of the resource.</span></span>
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





