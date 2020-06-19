---
title: tipo de recurso resetPasscodeActionResult
description: Resultado de ação de redefinir a senha
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 35ffae18d564ccda9d54599833195ea845d654f4
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44788056"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="d1b8e-103">tipo de recurso resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="d1b8e-103">resetPasscodeActionResult resource type</span></span>

<span data-ttu-id="d1b8e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1b8e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1b8e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d1b8e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1b8e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d1b8e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1b8e-107">Resultado da ação de redefinir a senha</span><span class="sxs-lookup"><span data-stu-id="d1b8e-107">Reset passcode action result</span></span>


<span data-ttu-id="d1b8e-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d1b8e-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d1b8e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d1b8e-109">Properties</span></span>
|<span data-ttu-id="d1b8e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d1b8e-110">Property</span></span>|<span data-ttu-id="d1b8e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1b8e-111">Type</span></span>|<span data-ttu-id="d1b8e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1b8e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1b8e-113">actionName</span><span class="sxs-lookup"><span data-stu-id="d1b8e-113">actionName</span></span>|<span data-ttu-id="d1b8e-114">String</span><span class="sxs-lookup"><span data-stu-id="d1b8e-114">String</span></span>|<span data-ttu-id="d1b8e-115">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d1b8e-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d1b8e-116">actionState</span><span class="sxs-lookup"><span data-stu-id="d1b8e-116">actionState</span></span>|[<span data-ttu-id="d1b8e-117">actionState</span><span class="sxs-lookup"><span data-stu-id="d1b8e-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="d1b8e-118">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="d1b8e-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="d1b8e-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="d1b8e-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="d1b8e-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d1b8e-120">startDateTime</span></span>|<span data-ttu-id="d1b8e-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1b8e-121">DateTimeOffset</span></span>|<span data-ttu-id="d1b8e-122">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d1b8e-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d1b8e-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d1b8e-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="d1b8e-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1b8e-124">DateTimeOffset</span></span>|<span data-ttu-id="d1b8e-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d1b8e-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d1b8e-126">senha</span><span class="sxs-lookup"><span data-stu-id="d1b8e-126">passcode</span></span>|<span data-ttu-id="d1b8e-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1b8e-127">String</span></span>|<span data-ttu-id="d1b8e-128">Senha recentemente gerada para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="d1b8e-128">Newly generated passcode for the device</span></span> |
|<span data-ttu-id="d1b8e-129">errorCode</span><span class="sxs-lookup"><span data-stu-id="d1b8e-129">errorCode</span></span>|<span data-ttu-id="d1b8e-130">Int32</span><span class="sxs-lookup"><span data-stu-id="d1b8e-130">Int32</span></span>|<span data-ttu-id="d1b8e-131">Código de erro de ação RotateBitLockerKeys.</span><span class="sxs-lookup"><span data-stu-id="d1b8e-131">RotateBitLockerKeys action error code.</span></span> <span data-ttu-id="d1b8e-132">Valores válidos de 0 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="d1b8e-132">Valid values 0 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1b8e-133">Relações</span><span class="sxs-lookup"><span data-stu-id="d1b8e-133">Relationships</span></span>
<span data-ttu-id="d1b8e-134">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d1b8e-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1b8e-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d1b8e-135">JSON Representation</span></span>
<span data-ttu-id="d1b8e-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d1b8e-136">Here is a JSON representation of the resource.</span></span>
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
  "passcode": "String",
  "errorCode": 1024
}
```



