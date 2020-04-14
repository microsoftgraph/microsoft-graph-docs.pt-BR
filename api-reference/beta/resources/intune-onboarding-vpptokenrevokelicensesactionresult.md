---
title: tipo de recurso vppTokenRevokeLicensesActionResult
description: O status da ação de revogação de licenças executada no token do Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e4033342cfb1b08563b53a00ea1314209cc1db49
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446827"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a><span data-ttu-id="4610b-103">tipo de recurso vppTokenRevokeLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="4610b-103">vppTokenRevokeLicensesActionResult resource type</span></span>

<span data-ttu-id="4610b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4610b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4610b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4610b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4610b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4610b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4610b-107">O status da ação de revogação de licenças executada no token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="4610b-107">The status of the revoke licenses action performed on the Apple Volume Purchase Program token.</span></span>


<span data-ttu-id="4610b-108">Herda de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4610b-108">Inherits from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4610b-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4610b-109">Properties</span></span>
|<span data-ttu-id="4610b-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4610b-110">Property</span></span>|<span data-ttu-id="4610b-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="4610b-111">Type</span></span>|<span data-ttu-id="4610b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4610b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4610b-113">actionName</span><span class="sxs-lookup"><span data-stu-id="4610b-113">actionName</span></span>|<span data-ttu-id="4610b-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4610b-114">String</span></span>|<span data-ttu-id="4610b-115">Nome da ação herdado de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4610b-115">Action name Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="4610b-116">actionState</span><span class="sxs-lookup"><span data-stu-id="4610b-116">actionState</span></span>|[<span data-ttu-id="4610b-117">actionState</span><span class="sxs-lookup"><span data-stu-id="4610b-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="4610b-118">Estado da ação herdada de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="4610b-118">State of the action Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span></span> <span data-ttu-id="4610b-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="4610b-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="4610b-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4610b-120">startDateTime</span></span>|<span data-ttu-id="4610b-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4610b-121">DateTimeOffset</span></span>|<span data-ttu-id="4610b-122">Hora em que a ação foi iniciada herdada de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4610b-122">Time the action was initiated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="4610b-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="4610b-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="4610b-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4610b-124">DateTimeOffset</span></span>|<span data-ttu-id="4610b-125">Hora em que o estado da ação foi atualizado pela última vez de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4610b-125">Time the action state was last updated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="4610b-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="4610b-126">totalLicensesCount</span></span>|<span data-ttu-id="4610b-127">Int32</span><span class="sxs-lookup"><span data-stu-id="4610b-127">Int32</span></span>|<span data-ttu-id="4610b-128">Uma contagem do número de licenças que foram tentadas revogar.</span><span class="sxs-lookup"><span data-stu-id="4610b-128">A count of the number of licenses that were attempted to revoke.</span></span>|
|<span data-ttu-id="4610b-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="4610b-129">failedLicensesCount</span></span>|<span data-ttu-id="4610b-130">Int32</span><span class="sxs-lookup"><span data-stu-id="4610b-130">Int32</span></span>|<span data-ttu-id="4610b-131">Uma contagem do número de licenças que falharam ao revogar.</span><span class="sxs-lookup"><span data-stu-id="4610b-131">A count of the number of licenses that failed to revoke.</span></span>|
|<span data-ttu-id="4610b-132">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="4610b-132">actionFailureReason</span></span>|[<span data-ttu-id="4610b-133">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="4610b-133">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="4610b-134">O motivo da falha na ação de revogação de licenças.</span><span class="sxs-lookup"><span data-stu-id="4610b-134">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="4610b-135">Os valores possíveis são: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="4610b-135">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4610b-136">Relações</span><span class="sxs-lookup"><span data-stu-id="4610b-136">Relationships</span></span>
<span data-ttu-id="4610b-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4610b-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4610b-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4610b-138">JSON Representation</span></span>
<span data-ttu-id="4610b-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4610b-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenRevokeLicensesActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024,
  "actionFailureReason": "String"
}
```



