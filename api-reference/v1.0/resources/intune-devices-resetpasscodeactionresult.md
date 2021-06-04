---
title: tipo de recurso resetPasscodeActionResult
description: Resultado de ação de redefinir a senha
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c2cb26a208c09449c732aeed621ed05c59cd4450
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754550"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="cef01-103">tipo de recurso resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="cef01-103">resetPasscodeActionResult resource type</span></span>

<span data-ttu-id="cef01-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cef01-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cef01-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cef01-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cef01-106">Resultado da ação de redefinir a senha</span><span class="sxs-lookup"><span data-stu-id="cef01-106">Reset passcode action result</span></span>


<span data-ttu-id="cef01-107">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="cef01-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cef01-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cef01-108">Properties</span></span>
|<span data-ttu-id="cef01-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cef01-109">Property</span></span>|<span data-ttu-id="cef01-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="cef01-110">Type</span></span>|<span data-ttu-id="cef01-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cef01-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cef01-112">actionName</span><span class="sxs-lookup"><span data-stu-id="cef01-112">actionName</span></span>|<span data-ttu-id="cef01-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cef01-113">String</span></span>|<span data-ttu-id="cef01-114">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="cef01-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="cef01-115">actionState</span><span class="sxs-lookup"><span data-stu-id="cef01-115">actionState</span></span>|[<span data-ttu-id="cef01-116">actionState</span><span class="sxs-lookup"><span data-stu-id="cef01-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="cef01-117">Estado da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="cef01-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="cef01-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="cef01-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="cef01-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="cef01-119">startDateTime</span></span>|<span data-ttu-id="cef01-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cef01-120">DateTimeOffset</span></span>|<span data-ttu-id="cef01-121">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="cef01-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="cef01-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="cef01-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="cef01-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cef01-123">DateTimeOffset</span></span>|<span data-ttu-id="cef01-124">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="cef01-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="cef01-125">senha</span><span class="sxs-lookup"><span data-stu-id="cef01-125">passcode</span></span>|<span data-ttu-id="cef01-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cef01-126">String</span></span>|<span data-ttu-id="cef01-127">Senha recentemente gerada para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="cef01-127">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="cef01-128">Relações</span><span class="sxs-lookup"><span data-stu-id="cef01-128">Relationships</span></span>
<span data-ttu-id="cef01-129">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="cef01-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cef01-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cef01-130">JSON Representation</span></span>
<span data-ttu-id="cef01-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cef01-131">Here is a JSON representation of the resource.</span></span>
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




