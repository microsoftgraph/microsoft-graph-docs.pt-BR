---
title: tipo de recurso resetPasscodeActionResult
description: Resultado de ação de redefinir a senha
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c30c204699f7fdc277aab56848fb109a32ab8ec4
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783883"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="24e5b-103">tipo de recurso resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="24e5b-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="24e5b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="24e5b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24e5b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="24e5b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24e5b-106">Resultado da ação de redefinir a senha</span><span class="sxs-lookup"><span data-stu-id="24e5b-106">Reset passcode action result</span></span>


<span data-ttu-id="24e5b-107">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="24e5b-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="24e5b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="24e5b-108">Properties</span></span>
|<span data-ttu-id="24e5b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="24e5b-109">Property</span></span>|<span data-ttu-id="24e5b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="24e5b-110">Type</span></span>|<span data-ttu-id="24e5b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="24e5b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24e5b-112">actionName</span><span class="sxs-lookup"><span data-stu-id="24e5b-112">actionName</span></span>|<span data-ttu-id="24e5b-113">String</span><span class="sxs-lookup"><span data-stu-id="24e5b-113">String</span></span>|<span data-ttu-id="24e5b-114">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="24e5b-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="24e5b-115">actionState</span><span class="sxs-lookup"><span data-stu-id="24e5b-115">actionState</span></span>|[<span data-ttu-id="24e5b-116">actionState</span><span class="sxs-lookup"><span data-stu-id="24e5b-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="24e5b-117">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="24e5b-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="24e5b-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="24e5b-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="24e5b-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="24e5b-119">startDateTime</span></span>|<span data-ttu-id="24e5b-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24e5b-120">DateTimeOffset</span></span>|<span data-ttu-id="24e5b-121">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="24e5b-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="24e5b-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="24e5b-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="24e5b-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24e5b-123">DateTimeOffset</span></span>|<span data-ttu-id="24e5b-124">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="24e5b-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="24e5b-125">senha</span><span class="sxs-lookup"><span data-stu-id="24e5b-125">passcode</span></span>|<span data-ttu-id="24e5b-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="24e5b-126">String</span></span>|<span data-ttu-id="24e5b-127">Senha recentemente gerada para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="24e5b-127">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="24e5b-128">Relações</span><span class="sxs-lookup"><span data-stu-id="24e5b-128">Relationships</span></span>
<span data-ttu-id="24e5b-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="24e5b-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="24e5b-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="24e5b-130">JSON Representation</span></span>
<span data-ttu-id="24e5b-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="24e5b-131">Here is a JSON representation of the resource.</span></span>
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



