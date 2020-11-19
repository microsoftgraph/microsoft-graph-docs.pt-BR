---
title: tipo de recurso vppTokenRevokeLicensesActionResult
description: O status da ação de revogação de licenças executada no token do Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 867d8c450ad199251a5a99b96b74eff01275845b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259554"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a><span data-ttu-id="0331f-103">tipo de recurso vppTokenRevokeLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="0331f-103">vppTokenRevokeLicensesActionResult resource type</span></span>

<span data-ttu-id="0331f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0331f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0331f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0331f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0331f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0331f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0331f-107">O status da ação de revogação de licenças executada no token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="0331f-107">The status of the revoke licenses action performed on the Apple Volume Purchase Program token.</span></span>


<span data-ttu-id="0331f-108">Herda de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0331f-108">Inherits from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0331f-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0331f-109">Properties</span></span>
|<span data-ttu-id="0331f-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0331f-110">Property</span></span>|<span data-ttu-id="0331f-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="0331f-111">Type</span></span>|<span data-ttu-id="0331f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="0331f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0331f-113">actionName</span><span class="sxs-lookup"><span data-stu-id="0331f-113">actionName</span></span>|<span data-ttu-id="0331f-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0331f-114">String</span></span>|<span data-ttu-id="0331f-115">Nome da ação herdado de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0331f-115">Action name Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="0331f-116">actionState</span><span class="sxs-lookup"><span data-stu-id="0331f-116">actionState</span></span>|[<span data-ttu-id="0331f-117">actionState</span><span class="sxs-lookup"><span data-stu-id="0331f-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="0331f-118">Estado da ação herdada de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="0331f-118">State of the action Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span></span> <span data-ttu-id="0331f-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="0331f-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="0331f-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0331f-120">startDateTime</span></span>|<span data-ttu-id="0331f-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0331f-121">DateTimeOffset</span></span>|<span data-ttu-id="0331f-122">Hora em que a ação foi iniciada herdada de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0331f-122">Time the action was initiated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="0331f-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="0331f-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="0331f-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0331f-124">DateTimeOffset</span></span>|<span data-ttu-id="0331f-125">Hora em que o estado da ação foi atualizado pela última vez de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0331f-125">Time the action state was last updated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="0331f-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="0331f-126">totalLicensesCount</span></span>|<span data-ttu-id="0331f-127">Int32</span><span class="sxs-lookup"><span data-stu-id="0331f-127">Int32</span></span>|<span data-ttu-id="0331f-128">Uma contagem do número de licenças que foram tentadas revogar.</span><span class="sxs-lookup"><span data-stu-id="0331f-128">A count of the number of licenses that were attempted to revoke.</span></span>|
|<span data-ttu-id="0331f-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="0331f-129">failedLicensesCount</span></span>|<span data-ttu-id="0331f-130">Int32</span><span class="sxs-lookup"><span data-stu-id="0331f-130">Int32</span></span>|<span data-ttu-id="0331f-131">Uma contagem do número de licenças que falharam ao revogar.</span><span class="sxs-lookup"><span data-stu-id="0331f-131">A count of the number of licenses that failed to revoke.</span></span>|
|<span data-ttu-id="0331f-132">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="0331f-132">actionFailureReason</span></span>|[<span data-ttu-id="0331f-133">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="0331f-133">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="0331f-134">O motivo da falha na ação de revogação de licenças.</span><span class="sxs-lookup"><span data-stu-id="0331f-134">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="0331f-135">Os valores possíveis são: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="0331f-135">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0331f-136">Relações</span><span class="sxs-lookup"><span data-stu-id="0331f-136">Relationships</span></span>
<span data-ttu-id="0331f-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0331f-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0331f-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0331f-138">JSON Representation</span></span>
<span data-ttu-id="0331f-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0331f-139">Here is a JSON representation of the resource.</span></span>
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




