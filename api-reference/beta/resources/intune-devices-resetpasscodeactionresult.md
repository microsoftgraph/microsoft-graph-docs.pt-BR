---
title: tipo de recurso resetPasscodeActionResult
description: Resultado da ação de redefinir a senha
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ead49e3c73dc65ebbc139fc7d1fd37743fe98be3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844706"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="31ef1-103">tipo de recurso resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="31ef1-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="31ef1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="31ef1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31ef1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="31ef1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="31ef1-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="31ef1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31ef1-107">Resultado da ação de redefinir a senha</span><span class="sxs-lookup"><span data-stu-id="31ef1-107">Reset passcode action result</span></span>

<span data-ttu-id="31ef1-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="31ef1-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="31ef1-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="31ef1-109">Properties</span></span>
|<span data-ttu-id="31ef1-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31ef1-110">Property</span></span>|<span data-ttu-id="31ef1-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="31ef1-111">Type</span></span>|<span data-ttu-id="31ef1-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="31ef1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31ef1-113">actionName</span><span class="sxs-lookup"><span data-stu-id="31ef1-113">actionName</span></span>|<span data-ttu-id="31ef1-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31ef1-114">String</span></span>|<span data-ttu-id="31ef1-115">Nome da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="31ef1-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="31ef1-116">actionState</span><span class="sxs-lookup"><span data-stu-id="31ef1-116">actionState</span></span>|[<span data-ttu-id="31ef1-117">actionState</span><span class="sxs-lookup"><span data-stu-id="31ef1-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="31ef1-118">Estado da ação Inherited de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="31ef1-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="31ef1-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="31ef1-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="31ef1-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="31ef1-120">startDateTime</span></span>|<span data-ttu-id="31ef1-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31ef1-121">DateTimeOffset</span></span>|<span data-ttu-id="31ef1-122">Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="31ef1-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="31ef1-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="31ef1-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="31ef1-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31ef1-124">DateTimeOffset</span></span>|<span data-ttu-id="31ef1-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="31ef1-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="31ef1-126">senha</span><span class="sxs-lookup"><span data-stu-id="31ef1-126">passcode</span></span>|<span data-ttu-id="31ef1-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31ef1-127">String</span></span>|<span data-ttu-id="31ef1-128">Senha recentemente gerada para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="31ef1-128">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="31ef1-129">Relações</span><span class="sxs-lookup"><span data-stu-id="31ef1-129">Relationships</span></span>
<span data-ttu-id="31ef1-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="31ef1-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="31ef1-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="31ef1-131">JSON Representation</span></span>
<span data-ttu-id="31ef1-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="31ef1-132">Here is a JSON representation of the resource.</span></span>
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





