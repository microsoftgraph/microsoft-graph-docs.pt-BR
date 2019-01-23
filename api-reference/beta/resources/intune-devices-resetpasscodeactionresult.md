---
title: tipo de recurso resetPasscodeActionResult
description: Resultado da ação de redefinir a senha
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5c022d2531bd1576ab7e336193d2f488f5f89f98
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407043"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="2435d-103">tipo de recurso resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="2435d-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="2435d-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="2435d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2435d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2435d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2435d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="2435d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2435d-107">Resultado da ação de redefinir a senha</span><span class="sxs-lookup"><span data-stu-id="2435d-107">Reset passcode action result</span></span>


<span data-ttu-id="2435d-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2435d-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2435d-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2435d-109">Properties</span></span>
|<span data-ttu-id="2435d-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2435d-110">Property</span></span>|<span data-ttu-id="2435d-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="2435d-111">Type</span></span>|<span data-ttu-id="2435d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2435d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2435d-113">actionName</span><span class="sxs-lookup"><span data-stu-id="2435d-113">actionName</span></span>|<span data-ttu-id="2435d-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2435d-114">String</span></span>|<span data-ttu-id="2435d-115">Nome da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2435d-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2435d-116">actionState</span><span class="sxs-lookup"><span data-stu-id="2435d-116">actionState</span></span>|[<span data-ttu-id="2435d-117">actionState</span><span class="sxs-lookup"><span data-stu-id="2435d-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="2435d-118">Estado da ação Inherited de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="2435d-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="2435d-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="2435d-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="2435d-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2435d-120">startDateTime</span></span>|<span data-ttu-id="2435d-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2435d-121">DateTimeOffset</span></span>|<span data-ttu-id="2435d-122">Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2435d-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2435d-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="2435d-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="2435d-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2435d-124">DateTimeOffset</span></span>|<span data-ttu-id="2435d-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2435d-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2435d-126">senha</span><span class="sxs-lookup"><span data-stu-id="2435d-126">passcode</span></span>|<span data-ttu-id="2435d-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2435d-127">String</span></span>|<span data-ttu-id="2435d-128">Senha recentemente gerada para o dispositivo</span><span class="sxs-lookup"><span data-stu-id="2435d-128">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="2435d-129">Relações</span><span class="sxs-lookup"><span data-stu-id="2435d-129">Relationships</span></span>
<span data-ttu-id="2435d-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2435d-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2435d-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2435d-131">JSON Representation</span></span>
<span data-ttu-id="2435d-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2435d-132">Here is a JSON representation of the resource.</span></span>
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




