---
title: tipo de recurso de revokeAppleVppLicensesActionResult
description: Revogar o resultado de ação do Apple Vpp licenças
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2cd77bee330e919ab51927af0773d913099cea6e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419223"
---
# <a name="revokeapplevpplicensesactionresult-resource-type"></a><span data-ttu-id="52a83-103">tipo de recurso de revokeAppleVppLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="52a83-103">revokeAppleVppLicensesActionResult resource type</span></span>

> <span data-ttu-id="52a83-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="52a83-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="52a83-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="52a83-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="52a83-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="52a83-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52a83-107">Revogar o resultado de ação do Apple Vpp licenças</span><span class="sxs-lookup"><span data-stu-id="52a83-107">Revoke Apple Vpp licenses action result</span></span>


<span data-ttu-id="52a83-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="52a83-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="52a83-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52a83-109">Properties</span></span>
|<span data-ttu-id="52a83-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52a83-110">Property</span></span>|<span data-ttu-id="52a83-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="52a83-111">Type</span></span>|<span data-ttu-id="52a83-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="52a83-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52a83-113">actionName</span><span class="sxs-lookup"><span data-stu-id="52a83-113">actionName</span></span>|<span data-ttu-id="52a83-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52a83-114">String</span></span>|<span data-ttu-id="52a83-115">Nome da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="52a83-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="52a83-116">actionState</span><span class="sxs-lookup"><span data-stu-id="52a83-116">actionState</span></span>|[<span data-ttu-id="52a83-117">actionState</span><span class="sxs-lookup"><span data-stu-id="52a83-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="52a83-118">Estado da ação Inherited de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="52a83-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="52a83-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="52a83-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="52a83-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="52a83-120">startDateTime</span></span>|<span data-ttu-id="52a83-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52a83-121">DateTimeOffset</span></span>|<span data-ttu-id="52a83-122">Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="52a83-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="52a83-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="52a83-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="52a83-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52a83-124">DateTimeOffset</span></span>|<span data-ttu-id="52a83-125">Hora em que o estado da ação foi atualizado pela última vez, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="52a83-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="52a83-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="52a83-126">totalLicensesCount</span></span>|<span data-ttu-id="52a83-127">Int32</span><span class="sxs-lookup"><span data-stu-id="52a83-127">Int32</span></span>|<span data-ttu-id="52a83-128">Número total de licenças do Apple Vpp associados</span><span class="sxs-lookup"><span data-stu-id="52a83-128">Total number of Apple Vpp licenses associated</span></span>|
|<span data-ttu-id="52a83-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="52a83-129">failedLicensesCount</span></span>|<span data-ttu-id="52a83-130">Int32</span><span class="sxs-lookup"><span data-stu-id="52a83-130">Int32</span></span>|<span data-ttu-id="52a83-131">Número total de licenças Apple Vpp com falha para revogar</span><span class="sxs-lookup"><span data-stu-id="52a83-131">Total number of Apple Vpp licenses that failed to revoke</span></span>|

## <a name="relationships"></a><span data-ttu-id="52a83-132">Relações</span><span class="sxs-lookup"><span data-stu-id="52a83-132">Relationships</span></span>
<span data-ttu-id="52a83-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="52a83-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="52a83-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52a83-134">JSON Representation</span></span>
<span data-ttu-id="52a83-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="52a83-135">Here is a JSON representation of the resource.</span></span>
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




