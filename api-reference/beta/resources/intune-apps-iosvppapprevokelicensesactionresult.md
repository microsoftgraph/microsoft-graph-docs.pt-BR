---
title: tipo de recurso iosVppAppRevokeLicensesActionResult
description: Define resultados para ações em aplicativos VPP do iOS, contendo propriedades herdadas de ActionResult.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fbc7ea19fb2a644b889ac1a6a00f5a3fba503f93
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42493220"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="1453a-103">tipo de recurso iosVppAppRevokeLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="1453a-103">iosVppAppRevokeLicensesActionResult resource type</span></span>

<span data-ttu-id="1453a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1453a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1453a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1453a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1453a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1453a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1453a-107">Define resultados para ações em aplicativos VPP do iOS, contendo propriedades herdadas de ActionResult.</span><span class="sxs-lookup"><span data-stu-id="1453a-107">Defines results for actions on iOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="1453a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1453a-108">Properties</span></span>
|<span data-ttu-id="1453a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1453a-109">Property</span></span>|<span data-ttu-id="1453a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1453a-110">Type</span></span>|<span data-ttu-id="1453a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1453a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1453a-112">userId</span><span class="sxs-lookup"><span data-stu-id="1453a-112">userId</span></span>|<span data-ttu-id="1453a-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1453a-113">String</span></span>|<span data-ttu-id="1453a-114">UserId associado à ação.</span><span class="sxs-lookup"><span data-stu-id="1453a-114">UserId associated with the action.</span></span>|
|<span data-ttu-id="1453a-115">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="1453a-115">managedDeviceId</span></span>|<span data-ttu-id="1453a-116">String</span><span class="sxs-lookup"><span data-stu-id="1453a-116">String</span></span>|<span data-ttu-id="1453a-117">DeviceID associado à ação.</span><span class="sxs-lookup"><span data-stu-id="1453a-117">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="1453a-118">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="1453a-118">totalLicensesCount</span></span>|<span data-ttu-id="1453a-119">Int32</span><span class="sxs-lookup"><span data-stu-id="1453a-119">Int32</span></span>|<span data-ttu-id="1453a-120">Uma contagem do número de licenças para as quais houve uma tentativa de revogação.</span><span class="sxs-lookup"><span data-stu-id="1453a-120">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="1453a-121">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="1453a-121">failedLicensesCount</span></span>|<span data-ttu-id="1453a-122">Int32</span><span class="sxs-lookup"><span data-stu-id="1453a-122">Int32</span></span>|<span data-ttu-id="1453a-123">Uma contagem do número de licenças para as quais houve falha na revogação.</span><span class="sxs-lookup"><span data-stu-id="1453a-123">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="1453a-124">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="1453a-124">actionFailureReason</span></span>|[<span data-ttu-id="1453a-125">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="1453a-125">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="1453a-126">O motivo da falha na ação de revogação de licenças.</span><span class="sxs-lookup"><span data-stu-id="1453a-126">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="1453a-127">Os valores possíveis são: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="1453a-127">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="1453a-128">actionName</span><span class="sxs-lookup"><span data-stu-id="1453a-128">actionName</span></span>|<span data-ttu-id="1453a-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1453a-129">String</span></span>|<span data-ttu-id="1453a-130">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="1453a-130">Action name</span></span>|
|<span data-ttu-id="1453a-131">actionState</span><span class="sxs-lookup"><span data-stu-id="1453a-131">actionState</span></span>|[<span data-ttu-id="1453a-132">actionState</span><span class="sxs-lookup"><span data-stu-id="1453a-132">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="1453a-133">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="1453a-133">State of the action.</span></span> <span data-ttu-id="1453a-134">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="1453a-134">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="1453a-135">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1453a-135">startDateTime</span></span>|<span data-ttu-id="1453a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1453a-136">DateTimeOffset</span></span>|<span data-ttu-id="1453a-137">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="1453a-137">Time the action was initiated</span></span>|
|<span data-ttu-id="1453a-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1453a-138">lastUpdatedDateTime</span></span>|<span data-ttu-id="1453a-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1453a-139">DateTimeOffset</span></span>|<span data-ttu-id="1453a-140">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="1453a-140">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="1453a-141">Relações</span><span class="sxs-lookup"><span data-stu-id="1453a-141">Relationships</span></span>
<span data-ttu-id="1453a-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1453a-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1453a-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1453a-143">JSON Representation</span></span>
<span data-ttu-id="1453a-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1453a-144">Here is a JSON representation of the resource.</span></span>
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



