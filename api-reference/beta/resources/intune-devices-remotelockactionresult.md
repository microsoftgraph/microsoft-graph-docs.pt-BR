---
title: Tipo de recurso remoteLockActionResult
description: Resultado da ação de bloquear com um pin para desbloquear
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7e57949e689f3d8e26c5217acec1a36662145b1a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416465"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="cb84f-103">Tipo de recurso remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="cb84f-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="cb84f-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="cb84f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cb84f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cb84f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cb84f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="cb84f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb84f-107">Resultado da ação de bloquear com um pin para desbloquear</span><span class="sxs-lookup"><span data-stu-id="cb84f-107">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="cb84f-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="cb84f-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cb84f-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cb84f-109">Properties</span></span>
|<span data-ttu-id="cb84f-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb84f-110">Property</span></span>|<span data-ttu-id="cb84f-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb84f-111">Type</span></span>|<span data-ttu-id="cb84f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb84f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb84f-113">actionName</span><span class="sxs-lookup"><span data-stu-id="cb84f-113">actionName</span></span>|<span data-ttu-id="cb84f-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb84f-114">String</span></span>|<span data-ttu-id="cb84f-115">Nome da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="cb84f-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="cb84f-116">actionState</span><span class="sxs-lookup"><span data-stu-id="cb84f-116">actionState</span></span>|[<span data-ttu-id="cb84f-117">actionState</span><span class="sxs-lookup"><span data-stu-id="cb84f-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="cb84f-118">Estado da ação Inherited de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="cb84f-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="cb84f-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="cb84f-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="cb84f-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="cb84f-120">startDateTime</span></span>|<span data-ttu-id="cb84f-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb84f-121">DateTimeOffset</span></span>|<span data-ttu-id="cb84f-122">Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="cb84f-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="cb84f-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb84f-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="cb84f-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb84f-124">DateTimeOffset</span></span>|<span data-ttu-id="cb84f-125">Hora em que o estado da ação foi atualizado pela última vez, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="cb84f-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="cb84f-126">unlockPin</span><span class="sxs-lookup"><span data-stu-id="cb84f-126">unlockPin</span></span>|<span data-ttu-id="cb84f-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cb84f-127">String</span></span>|<span data-ttu-id="cb84f-128">PIN para desbloquear o cliente</span><span class="sxs-lookup"><span data-stu-id="cb84f-128">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb84f-129">Relações</span><span class="sxs-lookup"><span data-stu-id="cb84f-129">Relationships</span></span>
<span data-ttu-id="cb84f-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cb84f-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb84f-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cb84f-131">JSON Representation</span></span>
<span data-ttu-id="cb84f-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cb84f-132">Here is a JSON representation of the resource.</span></span>
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




