---
title: tipo de recurso resetPasscodeActionResult
description: Resultado de ação de redefinir a senha
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 90a9011f0b55ee38191fc2fc9c445583fe89f4b7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081080"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="3e9c3-103">tipo de recurso resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="3e9c3-103">resetPasscodeActionResult resource type</span></span>

<span data-ttu-id="3e9c3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e9c3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3e9c3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3e9c3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e9c3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3e9c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e9c3-107">Resultado da ação de redefinir a senha</span><span class="sxs-lookup"><span data-stu-id="3e9c3-107">Reset passcode action result</span></span>


<span data-ttu-id="3e9c3-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3e9c3-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3e9c3-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3e9c3-109">Properties</span></span>
|<span data-ttu-id="3e9c3-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e9c3-110">Property</span></span>|<span data-ttu-id="3e9c3-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e9c3-111">Type</span></span>|<span data-ttu-id="3e9c3-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e9c3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e9c3-113">actionName</span><span class="sxs-lookup"><span data-stu-id="3e9c3-113">actionName</span></span>|<span data-ttu-id="3e9c3-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e9c3-114">String</span></span>|<span data-ttu-id="3e9c3-115">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3e9c3-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3e9c3-116">actionState</span><span class="sxs-lookup"><span data-stu-id="3e9c3-116">actionState</span></span>|[<span data-ttu-id="3e9c3-117">actionState</span><span class="sxs-lookup"><span data-stu-id="3e9c3-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="3e9c3-118">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="3e9c3-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="3e9c3-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="3e9c3-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="3e9c3-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3e9c3-120">startDateTime</span></span>|<span data-ttu-id="3e9c3-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e9c3-121">DateTimeOffset</span></span>|<span data-ttu-id="3e9c3-122">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3e9c3-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3e9c3-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e9c3-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="3e9c3-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e9c3-124">DateTimeOffset</span></span>|<span data-ttu-id="3e9c3-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3e9c3-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3e9c3-126">senha</span><span class="sxs-lookup"><span data-stu-id="3e9c3-126">passcode</span></span>|<span data-ttu-id="3e9c3-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e9c3-127">String</span></span>|<span data-ttu-id="3e9c3-128">Senha recentemente gerada para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="3e9c3-128">Newly generated passcode for the device</span></span> |
|<span data-ttu-id="3e9c3-129">errorCode</span><span class="sxs-lookup"><span data-stu-id="3e9c3-129">errorCode</span></span>|<span data-ttu-id="3e9c3-130">Int32</span><span class="sxs-lookup"><span data-stu-id="3e9c3-130">Int32</span></span>|<span data-ttu-id="3e9c3-131">Código de erro de ação RotateBitLockerKeys.</span><span class="sxs-lookup"><span data-stu-id="3e9c3-131">RotateBitLockerKeys action error code.</span></span> <span data-ttu-id="3e9c3-132">Valores válidos de 0 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="3e9c3-132">Valid values 0 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e9c3-133">Relações</span><span class="sxs-lookup"><span data-stu-id="3e9c3-133">Relationships</span></span>
<span data-ttu-id="3e9c3-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3e9c3-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e9c3-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3e9c3-135">JSON Representation</span></span>
<span data-ttu-id="3e9c3-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3e9c3-136">Here is a JSON representation of the resource.</span></span>
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






