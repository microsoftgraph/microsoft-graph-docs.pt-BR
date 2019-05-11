---
title: tipo de recurso iosVppAppRevokeLicensesActionResult
description: Define resultados para ações em aplicativos VPP do iOS, contendo propriedades herdadas de ActionResult.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6e28e21baa4dc0461d9b54f206810a969a153c15
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950239"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="06fc8-103">tipo de recurso iosVppAppRevokeLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="06fc8-103">iosVppAppRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="06fc8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="06fc8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06fc8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="06fc8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06fc8-106">Define resultados para ações em aplicativos VPP do iOS, contendo propriedades herdadas de ActionResult.</span><span class="sxs-lookup"><span data-stu-id="06fc8-106">Defines results for actions on iOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="06fc8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="06fc8-107">Properties</span></span>
|<span data-ttu-id="06fc8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06fc8-108">Property</span></span>|<span data-ttu-id="06fc8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="06fc8-109">Type</span></span>|<span data-ttu-id="06fc8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="06fc8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06fc8-111">userId</span><span class="sxs-lookup"><span data-stu-id="06fc8-111">userId</span></span>|<span data-ttu-id="06fc8-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06fc8-112">String</span></span>|<span data-ttu-id="06fc8-113">UserId associado à ação.</span><span class="sxs-lookup"><span data-stu-id="06fc8-113">UserId associated with the action.</span></span>|
|<span data-ttu-id="06fc8-114">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="06fc8-114">managedDeviceId</span></span>|<span data-ttu-id="06fc8-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06fc8-115">String</span></span>|<span data-ttu-id="06fc8-116">DeviceID associado à ação.</span><span class="sxs-lookup"><span data-stu-id="06fc8-116">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="06fc8-117">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="06fc8-117">totalLicensesCount</span></span>|<span data-ttu-id="06fc8-118">Int32</span><span class="sxs-lookup"><span data-stu-id="06fc8-118">Int32</span></span>|<span data-ttu-id="06fc8-119">Uma contagem do número de licenças para as quais houve uma tentativa de revogação.</span><span class="sxs-lookup"><span data-stu-id="06fc8-119">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="06fc8-120">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="06fc8-120">failedLicensesCount</span></span>|<span data-ttu-id="06fc8-121">Int32</span><span class="sxs-lookup"><span data-stu-id="06fc8-121">Int32</span></span>|<span data-ttu-id="06fc8-122">Uma contagem do número de licenças para as quais houve falha na revogação.</span><span class="sxs-lookup"><span data-stu-id="06fc8-122">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="06fc8-123">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="06fc8-123">actionFailureReason</span></span>|[<span data-ttu-id="06fc8-124">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="06fc8-124">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="06fc8-125">O motivo da falha na ação de revogação de licenças.</span><span class="sxs-lookup"><span data-stu-id="06fc8-125">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="06fc8-126">Os valores possíveis são: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="06fc8-126">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="06fc8-127">actionName</span><span class="sxs-lookup"><span data-stu-id="06fc8-127">actionName</span></span>|<span data-ttu-id="06fc8-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06fc8-128">String</span></span>|<span data-ttu-id="06fc8-129">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="06fc8-129">Action name</span></span>|
|<span data-ttu-id="06fc8-130">actionState</span><span class="sxs-lookup"><span data-stu-id="06fc8-130">actionState</span></span>|[<span data-ttu-id="06fc8-131">actionState</span><span class="sxs-lookup"><span data-stu-id="06fc8-131">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="06fc8-132">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="06fc8-132">State of the action.</span></span> <span data-ttu-id="06fc8-133">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="06fc8-133">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="06fc8-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="06fc8-134">startDateTime</span></span>|<span data-ttu-id="06fc8-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06fc8-135">DateTimeOffset</span></span>|<span data-ttu-id="06fc8-136">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="06fc8-136">Time the action was initiated</span></span>|
|<span data-ttu-id="06fc8-137">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="06fc8-137">lastUpdatedDateTime</span></span>|<span data-ttu-id="06fc8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06fc8-138">DateTimeOffset</span></span>|<span data-ttu-id="06fc8-139">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="06fc8-139">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="06fc8-140">Relações</span><span class="sxs-lookup"><span data-stu-id="06fc8-140">Relationships</span></span>
<span data-ttu-id="06fc8-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="06fc8-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="06fc8-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="06fc8-142">JSON Representation</span></span>
<span data-ttu-id="06fc8-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="06fc8-143">Here is a JSON representation of the resource.</span></span>
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




