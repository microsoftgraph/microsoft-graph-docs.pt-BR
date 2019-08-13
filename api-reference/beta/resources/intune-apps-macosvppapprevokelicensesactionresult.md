---
title: tipo de recurso macOsVppAppRevokeLicensesActionResult
description: Define os resultados de ações em aplicativos de conteúdo do MacOS, que contém as propriedades herdadas de ActionResult.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bb8a69ab5852aa3fee9ab8ffab757a87ef0235ba
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365892"
---
# <a name="macosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="28286-103">tipo de recurso macOsVppAppRevokeLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="28286-103">macOsVppAppRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="28286-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="28286-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28286-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="28286-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28286-106">Define os resultados de ações em aplicativos de conteúdo do MacOS, que contém as propriedades herdadas de ActionResult.</span><span class="sxs-lookup"><span data-stu-id="28286-106">Defines results for actions on MacOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="28286-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="28286-107">Properties</span></span>
|<span data-ttu-id="28286-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28286-108">Property</span></span>|<span data-ttu-id="28286-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="28286-109">Type</span></span>|<span data-ttu-id="28286-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="28286-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28286-111">userId</span><span class="sxs-lookup"><span data-stu-id="28286-111">userId</span></span>|<span data-ttu-id="28286-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="28286-112">String</span></span>|<span data-ttu-id="28286-113">UserId associado à ação.</span><span class="sxs-lookup"><span data-stu-id="28286-113">UserId associated with the action.</span></span>|
|<span data-ttu-id="28286-114">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="28286-114">managedDeviceId</span></span>|<span data-ttu-id="28286-115">String</span><span class="sxs-lookup"><span data-stu-id="28286-115">String</span></span>|<span data-ttu-id="28286-116">DeviceID associado à ação.</span><span class="sxs-lookup"><span data-stu-id="28286-116">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="28286-117">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="28286-117">totalLicensesCount</span></span>|<span data-ttu-id="28286-118">Int32</span><span class="sxs-lookup"><span data-stu-id="28286-118">Int32</span></span>|<span data-ttu-id="28286-119">Uma contagem do número de licenças para as quais houve uma tentativa de revogação.</span><span class="sxs-lookup"><span data-stu-id="28286-119">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="28286-120">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="28286-120">failedLicensesCount</span></span>|<span data-ttu-id="28286-121">Int32</span><span class="sxs-lookup"><span data-stu-id="28286-121">Int32</span></span>|<span data-ttu-id="28286-122">Uma contagem do número de licenças para as quais houve falha na revogação.</span><span class="sxs-lookup"><span data-stu-id="28286-122">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="28286-123">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="28286-123">actionFailureReason</span></span>|[<span data-ttu-id="28286-124">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="28286-124">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="28286-125">O motivo da falha na ação de revogação de licenças.</span><span class="sxs-lookup"><span data-stu-id="28286-125">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="28286-126">Os valores possíveis são: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="28286-126">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="28286-127">actionName</span><span class="sxs-lookup"><span data-stu-id="28286-127">actionName</span></span>|<span data-ttu-id="28286-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="28286-128">String</span></span>|<span data-ttu-id="28286-129">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="28286-129">Action name</span></span>|
|<span data-ttu-id="28286-130">actionState</span><span class="sxs-lookup"><span data-stu-id="28286-130">actionState</span></span>|[<span data-ttu-id="28286-131">actionState</span><span class="sxs-lookup"><span data-stu-id="28286-131">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="28286-132">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="28286-132">State of the action.</span></span> <span data-ttu-id="28286-133">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="28286-133">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="28286-134">startDateTime</span><span class="sxs-lookup"><span data-stu-id="28286-134">startDateTime</span></span>|<span data-ttu-id="28286-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28286-135">DateTimeOffset</span></span>|<span data-ttu-id="28286-136">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="28286-136">Time the action was initiated</span></span>|
|<span data-ttu-id="28286-137">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="28286-137">lastUpdatedDateTime</span></span>|<span data-ttu-id="28286-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28286-138">DateTimeOffset</span></span>|<span data-ttu-id="28286-139">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="28286-139">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="28286-140">Relações</span><span class="sxs-lookup"><span data-stu-id="28286-140">Relationships</span></span>
<span data-ttu-id="28286-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="28286-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="28286-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="28286-142">JSON Representation</span></span>
<span data-ttu-id="28286-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="28286-143">Here is a JSON representation of the resource.</span></span>
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



