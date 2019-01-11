---
title: tipo de recurso de vppTokenRevokeLicensesActionResult
description: O status da ação licenças revoke executada no token do programa de compra de Volume do Apple.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d7df9472be177bb52eba22ebf54f24e75c9a3539
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866490"
---
# <a name="vpptokenrevokelicensesactionresult-resource-type"></a><span data-ttu-id="125fa-103">tipo de recurso de vppTokenRevokeLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="125fa-103">vppTokenRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="125fa-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="125fa-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="125fa-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="125fa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="125fa-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="125fa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="125fa-107">O status da ação licenças revoke executada no token do programa de compra de Volume do Apple.</span><span class="sxs-lookup"><span data-stu-id="125fa-107">The status of the revoke licenses action performed on the Apple Volume Purchase Program token.</span></span>

<span data-ttu-id="125fa-108">Herda de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="125fa-108">Inherits from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="125fa-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="125fa-109">Properties</span></span>
|<span data-ttu-id="125fa-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="125fa-110">Property</span></span>|<span data-ttu-id="125fa-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="125fa-111">Type</span></span>|<span data-ttu-id="125fa-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="125fa-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="125fa-113">actionName</span><span class="sxs-lookup"><span data-stu-id="125fa-113">actionName</span></span>|<span data-ttu-id="125fa-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="125fa-114">String</span></span>|<span data-ttu-id="125fa-115">Nome da ação Inherited de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="125fa-115">Action name Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="125fa-116">actionState</span><span class="sxs-lookup"><span data-stu-id="125fa-116">actionState</span></span>|[<span data-ttu-id="125fa-117">actionState</span><span class="sxs-lookup"><span data-stu-id="125fa-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="125fa-118">Estado da ação Inherited de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="125fa-118">State of the action Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md).</span></span> <span data-ttu-id="125fa-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="125fa-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="125fa-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="125fa-120">startDateTime</span></span>|<span data-ttu-id="125fa-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="125fa-121">DateTimeOffset</span></span>|<span data-ttu-id="125fa-122">Hora a ação foi iniciada herdado de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="125fa-122">Time the action was initiated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="125fa-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="125fa-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="125fa-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="125fa-124">DateTimeOffset</span></span>|<span data-ttu-id="125fa-125">Tempo que o estado de ação foi o último atualizado Inherited de [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="125fa-125">Time the action state was last updated Inherited from [vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md)</span></span>|
|<span data-ttu-id="125fa-126">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="125fa-126">totalLicensesCount</span></span>|<span data-ttu-id="125fa-127">Int32</span><span class="sxs-lookup"><span data-stu-id="125fa-127">Int32</span></span>|<span data-ttu-id="125fa-128">Uma contagem do número de licenças que foram tentados a serem revogados.</span><span class="sxs-lookup"><span data-stu-id="125fa-128">A count of the number of licenses that were attempted to revoke.</span></span>|
|<span data-ttu-id="125fa-129">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="125fa-129">failedLicensesCount</span></span>|<span data-ttu-id="125fa-130">Int32</span><span class="sxs-lookup"><span data-stu-id="125fa-130">Int32</span></span>|<span data-ttu-id="125fa-131">Uma contagem do número de licenças que falharam a serem revogados.</span><span class="sxs-lookup"><span data-stu-id="125fa-131">A count of the number of licenses that failed to revoke.</span></span>|
|<span data-ttu-id="125fa-132">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="125fa-132">actionFailureReason</span></span>|[<span data-ttu-id="125fa-133">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="125fa-133">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="125fa-134">O motivo da falha de ação de licenças revoke.</span><span class="sxs-lookup"><span data-stu-id="125fa-134">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="125fa-135">Os valores possíveis são: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="125fa-135">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="125fa-136">Relações</span><span class="sxs-lookup"><span data-stu-id="125fa-136">Relationships</span></span>
<span data-ttu-id="125fa-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="125fa-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="125fa-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="125fa-138">JSON Representation</span></span>
<span data-ttu-id="125fa-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="125fa-139">Here is a JSON representation of the resource.</span></span>
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





