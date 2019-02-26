---
title: tipo de recurso macOsVppAppRevokeLicensesActionResult
description: Define os resultados de ações em aplicativos de conteúdo do MacOS, que contém as propriedades herdadas de ActionResult.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7cf8390dc2c1541525e288b81defd073144f4132
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166504"
---
# <a name="macosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="e42b9-103">tipo de recurso macOsVppAppRevokeLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="e42b9-103">macOsVppAppRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="e42b9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e42b9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e42b9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e42b9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e42b9-106">Define os resultados de ações em aplicativos de conteúdo do MacOS, que contém as propriedades herdadas de ActionResult.</span><span class="sxs-lookup"><span data-stu-id="e42b9-106">Defines results for actions on MacOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="e42b9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e42b9-107">Properties</span></span>
|<span data-ttu-id="e42b9-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e42b9-108">Property</span></span>|<span data-ttu-id="e42b9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e42b9-109">Type</span></span>|<span data-ttu-id="e42b9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e42b9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e42b9-111">userId</span><span class="sxs-lookup"><span data-stu-id="e42b9-111">userId</span></span>|<span data-ttu-id="e42b9-112">String</span><span class="sxs-lookup"><span data-stu-id="e42b9-112">String</span></span>|<span data-ttu-id="e42b9-113">UserId associado à ação.</span><span class="sxs-lookup"><span data-stu-id="e42b9-113">UserId associated with the action.</span></span>|
|<span data-ttu-id="e42b9-114">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="e42b9-114">managedDeviceId</span></span>|<span data-ttu-id="e42b9-115">String</span><span class="sxs-lookup"><span data-stu-id="e42b9-115">String</span></span>|<span data-ttu-id="e42b9-116">DeViceid associado à ação.</span><span class="sxs-lookup"><span data-stu-id="e42b9-116">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="e42b9-117">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="e42b9-117">totalLicensesCount</span></span>|<span data-ttu-id="e42b9-118">Int32</span><span class="sxs-lookup"><span data-stu-id="e42b9-118">Int32</span></span>|<span data-ttu-id="e42b9-119">Uma contagem do número de licenças para as quais houve uma tentativa de revogação.</span><span class="sxs-lookup"><span data-stu-id="e42b9-119">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="e42b9-120">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="e42b9-120">failedLicensesCount</span></span>|<span data-ttu-id="e42b9-121">Int32</span><span class="sxs-lookup"><span data-stu-id="e42b9-121">Int32</span></span>|<span data-ttu-id="e42b9-122">Uma contagem do número de licenças para as quais houve falha na revogação.</span><span class="sxs-lookup"><span data-stu-id="e42b9-122">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="e42b9-123">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="e42b9-123">actionFailureReason</span></span>|[<span data-ttu-id="e42b9-124">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="e42b9-124">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="e42b9-125">O motivo da falha na ação de revogação de licenças.</span><span class="sxs-lookup"><span data-stu-id="e42b9-125">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="e42b9-126">Os valores possíveis são: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="e42b9-126">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="e42b9-127">actionName</span><span class="sxs-lookup"><span data-stu-id="e42b9-127">actionName</span></span>|<span data-ttu-id="e42b9-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e42b9-128">String</span></span>|<span data-ttu-id="e42b9-129">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="e42b9-129">Action name</span></span>|
|<span data-ttu-id="e42b9-130">actionState</span><span class="sxs-lookup"><span data-stu-id="e42b9-130">actionState</span></span>|[<span data-ttu-id="e42b9-131">actionState</span><span class="sxs-lookup"><span data-stu-id="e42b9-131">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="e42b9-132">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="e42b9-132">State of the action.</span></span> <span data-ttu-id="e42b9-133">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="e42b9-133">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="e42b9-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e42b9-134">startDateTime</span></span>|<span data-ttu-id="e42b9-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e42b9-135">DateTimeOffset</span></span>|<span data-ttu-id="e42b9-136">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="e42b9-136">Time the action was initiated</span></span>|
|<span data-ttu-id="e42b9-137">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="e42b9-137">lastUpdatedDateTime</span></span>|<span data-ttu-id="e42b9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e42b9-138">DateTimeOffset</span></span>|<span data-ttu-id="e42b9-139">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="e42b9-139">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="e42b9-140">Relações</span><span class="sxs-lookup"><span data-stu-id="e42b9-140">Relationships</span></span>
<span data-ttu-id="e42b9-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e42b9-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e42b9-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e42b9-142">JSON Representation</span></span>
<span data-ttu-id="e42b9-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e42b9-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsVppAppRevokeLicensesActionResult",
  "userId": "String",
  "managedDeviceId": "String",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024,
  "actionFailureReason": "String",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```




