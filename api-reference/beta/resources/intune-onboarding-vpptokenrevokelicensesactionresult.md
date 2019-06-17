---
title: tipo de recurso vppTokenRevokeLicensesActionResult
description: O status da ação de revogação de licenças executada no token do Apple Volume Purchase Program.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e33a47d6fd4f40939d26a7faf41c209fe6e63651
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958582"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a><span data-ttu-id="4784c-103">tipo de recurso vppTokenRevokeLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="4784c-103">vppTokenRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="4784c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4784c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4784c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4784c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4784c-106">O status da ação de revogação de licenças executada no token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="4784c-106">The status of the revoke licenses action performed on the Apple Volume Purchase Program token.</span></span>


<span data-ttu-id="4784c-107">Herda de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4784c-107">Inherits from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4784c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4784c-108">Properties</span></span>
|<span data-ttu-id="4784c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4784c-109">Property</span></span>|<span data-ttu-id="4784c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4784c-110">Type</span></span>|<span data-ttu-id="4784c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4784c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4784c-112">actionName</span><span class="sxs-lookup"><span data-stu-id="4784c-112">actionName</span></span>|<span data-ttu-id="4784c-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4784c-113">String</span></span>|<span data-ttu-id="4784c-114">Nome da ação herdado de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4784c-114">Action name Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="4784c-115">actionState</span><span class="sxs-lookup"><span data-stu-id="4784c-115">actionState</span></span>|[<span data-ttu-id="4784c-116">actionState</span><span class="sxs-lookup"><span data-stu-id="4784c-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="4784c-117">Estado da ação herdada de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="4784c-117">State of the action Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span></span> <span data-ttu-id="4784c-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="4784c-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="4784c-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4784c-119">startDateTime</span></span>|<span data-ttu-id="4784c-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4784c-120">DateTimeOffset</span></span>|<span data-ttu-id="4784c-121">Hora em que a ação foi iniciada herdada de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4784c-121">Time the action was initiated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="4784c-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="4784c-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="4784c-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4784c-123">DateTimeOffset</span></span>|<span data-ttu-id="4784c-124">Hora em que o estado da ação foi atualizado pela última vez de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4784c-124">Time the action state was last updated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="4784c-125">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="4784c-125">totalLicensesCount</span></span>|<span data-ttu-id="4784c-126">Int32</span><span class="sxs-lookup"><span data-stu-id="4784c-126">Int32</span></span>|<span data-ttu-id="4784c-127">Uma contagem do número de licenças que foram tentadas revogar.</span><span class="sxs-lookup"><span data-stu-id="4784c-127">A count of the number of licenses that were attempted to revoke.</span></span>|
|<span data-ttu-id="4784c-128">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="4784c-128">failedLicensesCount</span></span>|<span data-ttu-id="4784c-129">Int32</span><span class="sxs-lookup"><span data-stu-id="4784c-129">Int32</span></span>|<span data-ttu-id="4784c-130">Uma contagem do número de licenças que falharam ao revogar.</span><span class="sxs-lookup"><span data-stu-id="4784c-130">A count of the number of licenses that failed to revoke.</span></span>|
|<span data-ttu-id="4784c-131">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="4784c-131">actionFailureReason</span></span>|[<span data-ttu-id="4784c-132">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="4784c-132">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="4784c-133">O motivo da falha na ação de revogação de licenças.</span><span class="sxs-lookup"><span data-stu-id="4784c-133">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="4784c-134">Os valores possíveis são: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="4784c-134">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4784c-135">Relações</span><span class="sxs-lookup"><span data-stu-id="4784c-135">Relationships</span></span>
<span data-ttu-id="4784c-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4784c-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4784c-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4784c-137">JSON Representation</span></span>
<span data-ttu-id="4784c-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4784c-138">Here is a JSON representation of the resource.</span></span>
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





