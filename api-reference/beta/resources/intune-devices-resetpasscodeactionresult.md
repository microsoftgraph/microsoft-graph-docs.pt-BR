---
title: tipo de recurso resetPasscodeActionResult
description: Resultado de ação de redefinir a senha
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f4dde2b89f186580e1c01e63a9a2dd718b3ecf32
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267310"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="0b281-103">tipo de recurso resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="0b281-103">resetPasscodeActionResult resource type</span></span>

<span data-ttu-id="0b281-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b281-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0b281-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0b281-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b281-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0b281-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b281-107">Resultado da ação de redefinir a senha</span><span class="sxs-lookup"><span data-stu-id="0b281-107">Reset passcode action result</span></span>


<span data-ttu-id="0b281-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0b281-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0b281-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b281-109">Properties</span></span>
|<span data-ttu-id="0b281-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b281-110">Property</span></span>|<span data-ttu-id="0b281-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b281-111">Type</span></span>|<span data-ttu-id="0b281-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b281-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b281-113">actionName</span><span class="sxs-lookup"><span data-stu-id="0b281-113">actionName</span></span>|<span data-ttu-id="0b281-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b281-114">String</span></span>|<span data-ttu-id="0b281-115">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0b281-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="0b281-116">actionState</span><span class="sxs-lookup"><span data-stu-id="0b281-116">actionState</span></span>|[<span data-ttu-id="0b281-117">actionState</span><span class="sxs-lookup"><span data-stu-id="0b281-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="0b281-118">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="0b281-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="0b281-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="0b281-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="0b281-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0b281-120">startDateTime</span></span>|<span data-ttu-id="0b281-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b281-121">DateTimeOffset</span></span>|<span data-ttu-id="0b281-122">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0b281-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="0b281-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="0b281-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="0b281-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b281-124">DateTimeOffset</span></span>|<span data-ttu-id="0b281-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0b281-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="0b281-126">senha</span><span class="sxs-lookup"><span data-stu-id="0b281-126">passcode</span></span>|<span data-ttu-id="0b281-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b281-127">String</span></span>|<span data-ttu-id="0b281-128">Senha recentemente gerada para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="0b281-128">Newly generated passcode for the device</span></span> |
|<span data-ttu-id="0b281-129">errorCode</span><span class="sxs-lookup"><span data-stu-id="0b281-129">errorCode</span></span>|<span data-ttu-id="0b281-130">Int32</span><span class="sxs-lookup"><span data-stu-id="0b281-130">Int32</span></span>|<span data-ttu-id="0b281-131">Código de erro de ação RotateBitLockerKeys.</span><span class="sxs-lookup"><span data-stu-id="0b281-131">RotateBitLockerKeys action error code.</span></span> <span data-ttu-id="0b281-132">Valores válidos de 0 a 2147483647</span><span class="sxs-lookup"><span data-stu-id="0b281-132">Valid values 0 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b281-133">Relações</span><span class="sxs-lookup"><span data-stu-id="0b281-133">Relationships</span></span>
<span data-ttu-id="0b281-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0b281-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b281-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b281-135">JSON Representation</span></span>
<span data-ttu-id="0b281-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0b281-136">Here is a JSON representation of the resource.</span></span>
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




