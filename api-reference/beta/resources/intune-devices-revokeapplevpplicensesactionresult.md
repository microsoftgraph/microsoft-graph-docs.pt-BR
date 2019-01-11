---
title: tipo de recurso de revokeAppleVppLicensesActionResult
description: Revogar o resultado de ação do Apple Vpp licenças
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b7e578ee695e171a1a91167b61e47af717dd82c0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879097"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a><span data-ttu-id="38565-103">tipo de recurso de revokeAppleVppLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="38565-103">revokeAppleVppLicensesActionResult resource type</span></span>

> <span data-ttu-id="38565-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="38565-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="38565-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="38565-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="38565-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="38565-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="38565-107">Revogar o resultado de ação do Apple Vpp licenças</span><span class="sxs-lookup"><span data-stu-id="38565-107">Revoke Apple Vpp licenses action result</span></span>

<span data-ttu-id="38565-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="38565-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="38565-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="38565-109">Properties</span></span>
|<span data-ttu-id="38565-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38565-110">Property</span></span>|<span data-ttu-id="38565-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="38565-111">Type</span></span>|<span data-ttu-id="38565-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="38565-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38565-113">actionName</span><span class="sxs-lookup"><span data-stu-id="38565-113">actionName</span></span>|<span data-ttu-id="38565-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38565-114">String</span></span>|<span data-ttu-id="38565-115">Nome da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="38565-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="38565-116">actionState</span><span class="sxs-lookup"><span data-stu-id="38565-116">actionState</span></span>|[<span data-ttu-id="38565-117">actionState</span><span class="sxs-lookup"><span data-stu-id="38565-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="38565-118">Estado da ação Inherited de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="38565-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="38565-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="38565-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="38565-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="38565-120">startDateTime</span></span>|<span data-ttu-id="38565-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38565-121">DateTimeOffset</span></span>|<span data-ttu-id="38565-122">Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="38565-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="38565-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="38565-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="38565-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38565-124">DateTimeOffset</span></span>|<span data-ttu-id="38565-125">Hora em que o estado da ação foi atualizado pela última vez, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="38565-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="38565-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="38565-126">totalLicensesCount</span></span>|<span data-ttu-id="38565-127">Int32</span><span class="sxs-lookup"><span data-stu-id="38565-127">Int32</span></span>|<span data-ttu-id="38565-128">Número total de licenças do Apple Vpp associados</span><span class="sxs-lookup"><span data-stu-id="38565-128">Total number of Apple Vpp licenses associated</span></span>|
|<span data-ttu-id="38565-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="38565-129">failedLicensesCount</span></span>|<span data-ttu-id="38565-130">Int32</span><span class="sxs-lookup"><span data-stu-id="38565-130">Int32</span></span>|<span data-ttu-id="38565-131">Número total de licenças Apple Vpp com falha para revogar</span><span class="sxs-lookup"><span data-stu-id="38565-131">Total number of Apple Vpp licenses that failed to revoke</span></span>|

## <a name="relationships"></a><span data-ttu-id="38565-132">Relações</span><span class="sxs-lookup"><span data-stu-id="38565-132">Relationships</span></span>
<span data-ttu-id="38565-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="38565-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="38565-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="38565-134">JSON Representation</span></span>
<span data-ttu-id="38565-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="38565-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.revokeAppleVppLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.revokeAppleVppLicensesActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024
}
```





