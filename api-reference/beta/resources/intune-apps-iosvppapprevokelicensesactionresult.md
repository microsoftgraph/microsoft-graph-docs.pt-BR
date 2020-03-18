---
title: tipo de recurso iosVppAppRevokeLicensesActionResult
description: Define resultados para ações em aplicativos VPP do iOS, contendo propriedades herdadas de ActionResult.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ebb4af4c9cd6b9f58a3e0ee341b7e43192094d29
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42798053"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="479b3-103">tipo de recurso iosVppAppRevokeLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="479b3-103">iosVppAppRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="479b3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="479b3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="479b3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="479b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="479b3-106">Define resultados para ações em aplicativos VPP do iOS, contendo propriedades herdadas de ActionResult.</span><span class="sxs-lookup"><span data-stu-id="479b3-106">Defines results for actions on iOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="479b3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="479b3-107">Properties</span></span>
|<span data-ttu-id="479b3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="479b3-108">Property</span></span>|<span data-ttu-id="479b3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="479b3-109">Type</span></span>|<span data-ttu-id="479b3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="479b3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="479b3-111">userId</span><span class="sxs-lookup"><span data-stu-id="479b3-111">userId</span></span>|<span data-ttu-id="479b3-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="479b3-112">String</span></span>|<span data-ttu-id="479b3-113">UserId associado à ação.</span><span class="sxs-lookup"><span data-stu-id="479b3-113">UserId associated with the action.</span></span>|
|<span data-ttu-id="479b3-114">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="479b3-114">managedDeviceId</span></span>|<span data-ttu-id="479b3-115">String</span><span class="sxs-lookup"><span data-stu-id="479b3-115">String</span></span>|<span data-ttu-id="479b3-116">DeviceID associado à ação.</span><span class="sxs-lookup"><span data-stu-id="479b3-116">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="479b3-117">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="479b3-117">totalLicensesCount</span></span>|<span data-ttu-id="479b3-118">Int32</span><span class="sxs-lookup"><span data-stu-id="479b3-118">Int32</span></span>|<span data-ttu-id="479b3-119">Uma contagem do número de licenças para as quais houve uma tentativa de revogação.</span><span class="sxs-lookup"><span data-stu-id="479b3-119">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="479b3-120">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="479b3-120">failedLicensesCount</span></span>|<span data-ttu-id="479b3-121">Int32</span><span class="sxs-lookup"><span data-stu-id="479b3-121">Int32</span></span>|<span data-ttu-id="479b3-122">Uma contagem do número de licenças para as quais houve falha na revogação.</span><span class="sxs-lookup"><span data-stu-id="479b3-122">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="479b3-123">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="479b3-123">actionFailureReason</span></span>|[<span data-ttu-id="479b3-124">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="479b3-124">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="479b3-125">O motivo da falha na ação de revogação de licenças.</span><span class="sxs-lookup"><span data-stu-id="479b3-125">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="479b3-126">Os valores possíveis são: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="479b3-126">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="479b3-127">actionName</span><span class="sxs-lookup"><span data-stu-id="479b3-127">actionName</span></span>|<span data-ttu-id="479b3-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="479b3-128">String</span></span>|<span data-ttu-id="479b3-129">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="479b3-129">Action name</span></span>|
|<span data-ttu-id="479b3-130">actionState</span><span class="sxs-lookup"><span data-stu-id="479b3-130">actionState</span></span>|[<span data-ttu-id="479b3-131">actionState</span><span class="sxs-lookup"><span data-stu-id="479b3-131">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="479b3-132">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="479b3-132">State of the action.</span></span> <span data-ttu-id="479b3-133">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="479b3-133">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="479b3-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="479b3-134">startDateTime</span></span>|<span data-ttu-id="479b3-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="479b3-135">DateTimeOffset</span></span>|<span data-ttu-id="479b3-136">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="479b3-136">Time the action was initiated</span></span>|
|<span data-ttu-id="479b3-137">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="479b3-137">lastUpdatedDateTime</span></span>|<span data-ttu-id="479b3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="479b3-138">DateTimeOffset</span></span>|<span data-ttu-id="479b3-139">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="479b3-139">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="479b3-140">Relações</span><span class="sxs-lookup"><span data-stu-id="479b3-140">Relationships</span></span>
<span data-ttu-id="479b3-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="479b3-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="479b3-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="479b3-142">JSON Representation</span></span>
<span data-ttu-id="479b3-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="479b3-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppRevokeLicensesActionResult",
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



