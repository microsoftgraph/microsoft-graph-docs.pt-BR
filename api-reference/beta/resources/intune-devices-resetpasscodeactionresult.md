---
title: tipo de recurso resetPasscodeActionResult
description: Resultado de ação de redefinir a senha
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4e7ff89fb85192a873595cb362c3e6031b834a7b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524932"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="4ba1c-103">tipo de recurso resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="4ba1c-103">resetPasscodeActionResult resource type</span></span>

<span data-ttu-id="4ba1c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4ba1c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ba1c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4ba1c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ba1c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4ba1c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ba1c-107">Resultado da ação de redefinir a senha</span><span class="sxs-lookup"><span data-stu-id="4ba1c-107">Reset passcode action result</span></span>


<span data-ttu-id="4ba1c-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4ba1c-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4ba1c-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4ba1c-109">Properties</span></span>
|<span data-ttu-id="4ba1c-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ba1c-110">Property</span></span>|<span data-ttu-id="4ba1c-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ba1c-111">Type</span></span>|<span data-ttu-id="4ba1c-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ba1c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ba1c-113">actionName</span><span class="sxs-lookup"><span data-stu-id="4ba1c-113">actionName</span></span>|<span data-ttu-id="4ba1c-114">String</span><span class="sxs-lookup"><span data-stu-id="4ba1c-114">String</span></span>|<span data-ttu-id="4ba1c-115">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4ba1c-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4ba1c-116">actionState</span><span class="sxs-lookup"><span data-stu-id="4ba1c-116">actionState</span></span>|[<span data-ttu-id="4ba1c-117">actionState</span><span class="sxs-lookup"><span data-stu-id="4ba1c-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="4ba1c-118">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="4ba1c-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="4ba1c-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="4ba1c-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="4ba1c-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4ba1c-120">startDateTime</span></span>|<span data-ttu-id="4ba1c-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ba1c-121">DateTimeOffset</span></span>|<span data-ttu-id="4ba1c-122">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4ba1c-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4ba1c-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="4ba1c-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="4ba1c-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ba1c-124">DateTimeOffset</span></span>|<span data-ttu-id="4ba1c-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4ba1c-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4ba1c-126">senha</span><span class="sxs-lookup"><span data-stu-id="4ba1c-126">passcode</span></span>|<span data-ttu-id="4ba1c-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ba1c-127">String</span></span>|<span data-ttu-id="4ba1c-128">Senha recentemente gerada para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="4ba1c-128">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="4ba1c-129">Relações</span><span class="sxs-lookup"><span data-stu-id="4ba1c-129">Relationships</span></span>
<span data-ttu-id="4ba1c-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4ba1c-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ba1c-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4ba1c-131">JSON Representation</span></span>
<span data-ttu-id="4ba1c-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4ba1c-132">Here is a JSON representation of the resource.</span></span>
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



