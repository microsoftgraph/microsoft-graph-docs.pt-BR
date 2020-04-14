---
title: tipo de recurso resetPasscodeActionResult
description: Resultado de ação de redefinir a senha
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 65ec840aaab89ee3558ee2882c5c3ed048f4c65a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43383179"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="f17fe-103">tipo de recurso resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="f17fe-103">resetPasscodeActionResult resource type</span></span>

<span data-ttu-id="f17fe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f17fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f17fe-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f17fe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f17fe-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f17fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f17fe-107">Resultado da ação de redefinir a senha</span><span class="sxs-lookup"><span data-stu-id="f17fe-107">Reset passcode action result</span></span>


<span data-ttu-id="f17fe-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f17fe-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f17fe-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f17fe-109">Properties</span></span>
|<span data-ttu-id="f17fe-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f17fe-110">Property</span></span>|<span data-ttu-id="f17fe-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="f17fe-111">Type</span></span>|<span data-ttu-id="f17fe-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="f17fe-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f17fe-113">actionName</span><span class="sxs-lookup"><span data-stu-id="f17fe-113">actionName</span></span>|<span data-ttu-id="f17fe-114">String</span><span class="sxs-lookup"><span data-stu-id="f17fe-114">String</span></span>|<span data-ttu-id="f17fe-115">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f17fe-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="f17fe-116">actionState</span><span class="sxs-lookup"><span data-stu-id="f17fe-116">actionState</span></span>|[<span data-ttu-id="f17fe-117">actionState</span><span class="sxs-lookup"><span data-stu-id="f17fe-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="f17fe-118">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="f17fe-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="f17fe-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="f17fe-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="f17fe-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f17fe-120">startDateTime</span></span>|<span data-ttu-id="f17fe-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f17fe-121">DateTimeOffset</span></span>|<span data-ttu-id="f17fe-122">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f17fe-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="f17fe-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="f17fe-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="f17fe-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f17fe-124">DateTimeOffset</span></span>|<span data-ttu-id="f17fe-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f17fe-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="f17fe-126">senha</span><span class="sxs-lookup"><span data-stu-id="f17fe-126">passcode</span></span>|<span data-ttu-id="f17fe-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f17fe-127">String</span></span>|<span data-ttu-id="f17fe-128">Senha recentemente gerada para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="f17fe-128">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="f17fe-129">Relações</span><span class="sxs-lookup"><span data-stu-id="f17fe-129">Relationships</span></span>
<span data-ttu-id="f17fe-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f17fe-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f17fe-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f17fe-131">JSON Representation</span></span>
<span data-ttu-id="f17fe-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f17fe-132">Here is a JSON representation of the resource.</span></span>
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



