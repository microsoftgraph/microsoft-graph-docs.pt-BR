---
title: tipo de recurso resetPasscodeActionResult
description: Resultado de ação de redefinir a senha
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 07b7728677f639fefabd2954f74ff006ff76ef40
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356893"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="4da31-103">tipo de recurso resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="4da31-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="4da31-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4da31-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4da31-105">Resultado da ação de redefinir a senha</span><span class="sxs-lookup"><span data-stu-id="4da31-105">Reset passcode action result</span></span>


<span data-ttu-id="4da31-106">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4da31-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4da31-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4da31-107">Properties</span></span>
|<span data-ttu-id="4da31-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4da31-108">Property</span></span>|<span data-ttu-id="4da31-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4da31-109">Type</span></span>|<span data-ttu-id="4da31-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4da31-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4da31-111">actionName</span><span class="sxs-lookup"><span data-stu-id="4da31-111">actionName</span></span>|<span data-ttu-id="4da31-112">String</span><span class="sxs-lookup"><span data-stu-id="4da31-112">String</span></span>|<span data-ttu-id="4da31-113">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4da31-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4da31-114">actionState</span><span class="sxs-lookup"><span data-stu-id="4da31-114">actionState</span></span>|[<span data-ttu-id="4da31-115">actionState</span><span class="sxs-lookup"><span data-stu-id="4da31-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="4da31-116">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="4da31-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="4da31-117">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="4da31-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="4da31-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4da31-118">startDateTime</span></span>|<span data-ttu-id="4da31-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4da31-119">DateTimeOffset</span></span>|<span data-ttu-id="4da31-120">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4da31-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4da31-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="4da31-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="4da31-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4da31-122">DateTimeOffset</span></span>|<span data-ttu-id="4da31-123">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4da31-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4da31-124">senha</span><span class="sxs-lookup"><span data-stu-id="4da31-124">passcode</span></span>|<span data-ttu-id="4da31-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4da31-125">String</span></span>|<span data-ttu-id="4da31-126">Senha recentemente gerada para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="4da31-126">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="4da31-127">Relações</span><span class="sxs-lookup"><span data-stu-id="4da31-127">Relationships</span></span>
<span data-ttu-id="4da31-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4da31-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4da31-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4da31-129">JSON Representation</span></span>
<span data-ttu-id="4da31-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4da31-130">Here is a JSON representation of the resource.</span></span>
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




