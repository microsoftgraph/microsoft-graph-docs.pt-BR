---
title: tipo de recurso resetPasscodeActionResult
description: Resultado de ação de redefinir a senha
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 456bbc92dba168501fe3114e831665f8e2efce50
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530288"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="36be7-103">tipo de recurso resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="36be7-103">resetPasscodeActionResult resource type</span></span>

<span data-ttu-id="36be7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36be7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="36be7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="36be7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36be7-106">Resultado da ação de redefinir a senha</span><span class="sxs-lookup"><span data-stu-id="36be7-106">Reset passcode action result</span></span>


<span data-ttu-id="36be7-107">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="36be7-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="36be7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="36be7-108">Properties</span></span>
|<span data-ttu-id="36be7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36be7-109">Property</span></span>|<span data-ttu-id="36be7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="36be7-110">Type</span></span>|<span data-ttu-id="36be7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="36be7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36be7-112">actionName</span><span class="sxs-lookup"><span data-stu-id="36be7-112">actionName</span></span>|<span data-ttu-id="36be7-113">String</span><span class="sxs-lookup"><span data-stu-id="36be7-113">String</span></span>|<span data-ttu-id="36be7-114">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="36be7-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="36be7-115">actionState</span><span class="sxs-lookup"><span data-stu-id="36be7-115">actionState</span></span>|[<span data-ttu-id="36be7-116">actionState</span><span class="sxs-lookup"><span data-stu-id="36be7-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="36be7-117">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="36be7-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="36be7-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="36be7-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="36be7-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="36be7-119">startDateTime</span></span>|<span data-ttu-id="36be7-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36be7-120">DateTimeOffset</span></span>|<span data-ttu-id="36be7-121">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="36be7-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="36be7-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="36be7-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="36be7-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36be7-123">DateTimeOffset</span></span>|<span data-ttu-id="36be7-124">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="36be7-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="36be7-125">senha</span><span class="sxs-lookup"><span data-stu-id="36be7-125">passcode</span></span>|<span data-ttu-id="36be7-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="36be7-126">String</span></span>|<span data-ttu-id="36be7-127">Senha recentemente gerada para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="36be7-127">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="36be7-128">Relações</span><span class="sxs-lookup"><span data-stu-id="36be7-128">Relationships</span></span>
<span data-ttu-id="36be7-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="36be7-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="36be7-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="36be7-130">JSON Representation</span></span>
<span data-ttu-id="36be7-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="36be7-131">Here is a JSON representation of the resource.</span></span>
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




