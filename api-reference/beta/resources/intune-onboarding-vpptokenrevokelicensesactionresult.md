---
title: tipo de recurso de vppTokenRevokeLicensesActionResult
description: O status da ação licenças revoke executada no token do programa de compra de Volume do Apple.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 75c75c6b8bcdc06ede0f71b19956155becc4d478
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418222"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a><span data-ttu-id="11bcb-103">tipo de recurso de vppTokenRevokeLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="11bcb-103">vppTokenRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="11bcb-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="11bcb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="11bcb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="11bcb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="11bcb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="11bcb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11bcb-107">O status da ação licenças revoke executada no token do programa de compra de Volume do Apple.</span><span class="sxs-lookup"><span data-stu-id="11bcb-107">The status of the revoke licenses action performed on the Apple Volume Purchase Program token.</span></span>


<span data-ttu-id="11bcb-108">Herda de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="11bcb-108">Inherits from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="11bcb-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11bcb-109">Properties</span></span>
|<span data-ttu-id="11bcb-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11bcb-110">Property</span></span>|<span data-ttu-id="11bcb-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="11bcb-111">Type</span></span>|<span data-ttu-id="11bcb-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="11bcb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11bcb-113">actionName</span><span class="sxs-lookup"><span data-stu-id="11bcb-113">actionName</span></span>|<span data-ttu-id="11bcb-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="11bcb-114">String</span></span>|<span data-ttu-id="11bcb-115">Nome da ação Inherited de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="11bcb-115">Action name Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="11bcb-116">actionState</span><span class="sxs-lookup"><span data-stu-id="11bcb-116">actionState</span></span>|[<span data-ttu-id="11bcb-117">actionState</span><span class="sxs-lookup"><span data-stu-id="11bcb-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="11bcb-118">Estado da ação Inherited de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="11bcb-118">State of the action Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span></span> <span data-ttu-id="11bcb-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="11bcb-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="11bcb-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="11bcb-120">startDateTime</span></span>|<span data-ttu-id="11bcb-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11bcb-121">DateTimeOffset</span></span>|<span data-ttu-id="11bcb-122">Hora a ação foi iniciada herdado de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="11bcb-122">Time the action was initiated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="11bcb-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="11bcb-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="11bcb-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11bcb-124">DateTimeOffset</span></span>|<span data-ttu-id="11bcb-125">Tempo que o estado de ação foi o último atualizado Inherited de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="11bcb-125">Time the action state was last updated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="11bcb-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="11bcb-126">totalLicensesCount</span></span>|<span data-ttu-id="11bcb-127">Int32</span><span class="sxs-lookup"><span data-stu-id="11bcb-127">Int32</span></span>|<span data-ttu-id="11bcb-128">Uma contagem do número de licenças que foram tentados a serem revogados.</span><span class="sxs-lookup"><span data-stu-id="11bcb-128">A count of the number of licenses that were attempted to revoke.</span></span>|
|<span data-ttu-id="11bcb-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="11bcb-129">failedLicensesCount</span></span>|<span data-ttu-id="11bcb-130">Int32</span><span class="sxs-lookup"><span data-stu-id="11bcb-130">Int32</span></span>|<span data-ttu-id="11bcb-131">Uma contagem do número de licenças que falharam a serem revogados.</span><span class="sxs-lookup"><span data-stu-id="11bcb-131">A count of the number of licenses that failed to revoke.</span></span>|
|<span data-ttu-id="11bcb-132">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="11bcb-132">actionFailureReason</span></span>|[<span data-ttu-id="11bcb-133">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="11bcb-133">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="11bcb-134">O motivo da falha de ação de licenças revoke.</span><span class="sxs-lookup"><span data-stu-id="11bcb-134">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="11bcb-135">Os valores possíveis são: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="11bcb-135">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11bcb-136">Relações</span><span class="sxs-lookup"><span data-stu-id="11bcb-136">Relationships</span></span>
<span data-ttu-id="11bcb-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="11bcb-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="11bcb-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11bcb-138">JSON Representation</span></span>
<span data-ttu-id="11bcb-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="11bcb-139">Here is a JSON representation of the resource.</span></span>
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




