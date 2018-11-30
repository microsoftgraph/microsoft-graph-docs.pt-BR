---
title: tipo de recurso resetPasscodeActionResult
description: Resultado da ação de redefinir a senha
ms.openlocfilehash: 6b951a75b93b4e625fb61110ba909632c051b0f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004888"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="3129a-103">tipo de recurso resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="3129a-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="3129a-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3129a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3129a-105">Resultado da ação de redefinir a senha</span><span class="sxs-lookup"><span data-stu-id="3129a-105">Reset passcode action result</span></span>

<span data-ttu-id="3129a-106">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3129a-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3129a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3129a-107">Properties</span></span>
|<span data-ttu-id="3129a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3129a-108">Property</span></span>|<span data-ttu-id="3129a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3129a-109">Type</span></span>|<span data-ttu-id="3129a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3129a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3129a-111">actionName</span><span class="sxs-lookup"><span data-stu-id="3129a-111">actionName</span></span>|<span data-ttu-id="3129a-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3129a-112">String</span></span>|<span data-ttu-id="3129a-113">Nome da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3129a-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3129a-114">actionState</span><span class="sxs-lookup"><span data-stu-id="3129a-114">actionState</span></span>|[<span data-ttu-id="3129a-115">actionState</span><span class="sxs-lookup"><span data-stu-id="3129a-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="3129a-116">Estado da ação Inherited de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="3129a-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="3129a-117">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="3129a-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="3129a-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3129a-118">startDateTime</span></span>|<span data-ttu-id="3129a-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3129a-119">DateTimeOffset</span></span>|<span data-ttu-id="3129a-120">Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3129a-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3129a-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="3129a-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="3129a-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3129a-122">DateTimeOffset</span></span>|<span data-ttu-id="3129a-123">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3129a-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3129a-124">senha</span><span class="sxs-lookup"><span data-stu-id="3129a-124">passcode</span></span>|<span data-ttu-id="3129a-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3129a-125">String</span></span>|<span data-ttu-id="3129a-126">Senha recentemente gerada para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="3129a-126">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="3129a-127">Relações</span><span class="sxs-lookup"><span data-stu-id="3129a-127">Relationships</span></span>
<span data-ttu-id="3129a-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3129a-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3129a-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3129a-129">JSON Representation</span></span>
<span data-ttu-id="3129a-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3129a-130">Here is a JSON representation of the resource.</span></span>
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



