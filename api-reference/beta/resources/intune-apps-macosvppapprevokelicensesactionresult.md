---
title: tipo de recurso de macOsVppAppRevokeLicensesActionResult
description: Define os resultados para ações nos aplicativos de Vpp MacOS, contém as propriedades herdadas para ActionResult.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f90bd55476bbbb48ab3a4904886a67b217ab67b7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29428986"
---
# <a name="macosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="a72c6-103">tipo de recurso de macOsVppAppRevokeLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="a72c6-103">macOsVppAppRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="a72c6-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="a72c6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a72c6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a72c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a72c6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="a72c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a72c6-107">Define os resultados para ações nos aplicativos de Vpp MacOS, contém as propriedades herdadas para ActionResult.</span><span class="sxs-lookup"><span data-stu-id="a72c6-107">Defines results for actions on MacOS Vpp Apps, contains inherited properties for ActionResult.</span></span>

## <a name="properties"></a><span data-ttu-id="a72c6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a72c6-108">Properties</span></span>
|<span data-ttu-id="a72c6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a72c6-109">Property</span></span>|<span data-ttu-id="a72c6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a72c6-110">Type</span></span>|<span data-ttu-id="a72c6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a72c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a72c6-112">userId</span><span class="sxs-lookup"><span data-stu-id="a72c6-112">userId</span></span>|<span data-ttu-id="a72c6-113">String</span><span class="sxs-lookup"><span data-stu-id="a72c6-113">String</span></span>|<span data-ttu-id="a72c6-114">ID de usuário associado à ação.</span><span class="sxs-lookup"><span data-stu-id="a72c6-114">UserId associated with the action.</span></span>|
|<span data-ttu-id="a72c6-115">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="a72c6-115">managedDeviceId</span></span>|<span data-ttu-id="a72c6-116">String</span><span class="sxs-lookup"><span data-stu-id="a72c6-116">String</span></span>|<span data-ttu-id="a72c6-117">DeviceId associado à ação.</span><span class="sxs-lookup"><span data-stu-id="a72c6-117">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="a72c6-118">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="a72c6-118">totalLicensesCount</span></span>|<span data-ttu-id="a72c6-119">Int32</span><span class="sxs-lookup"><span data-stu-id="a72c6-119">Int32</span></span>|<span data-ttu-id="a72c6-120">Uma contagem do número de licenças para o qual revoke foi tentada.</span><span class="sxs-lookup"><span data-stu-id="a72c6-120">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="a72c6-121">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="a72c6-121">failedLicensesCount</span></span>|<span data-ttu-id="a72c6-122">Int32</span><span class="sxs-lookup"><span data-stu-id="a72c6-122">Int32</span></span>|<span data-ttu-id="a72c6-123">Uma contagem do número de licenças para o qual revoke falhou.</span><span class="sxs-lookup"><span data-stu-id="a72c6-123">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="a72c6-124">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="a72c6-124">actionFailureReason</span></span>|[<span data-ttu-id="a72c6-125">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="a72c6-125">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="a72c6-126">O motivo da falha de ação de licenças revoke.</span><span class="sxs-lookup"><span data-stu-id="a72c6-126">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="a72c6-127">Os valores possíveis são: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="a72c6-127">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="a72c6-128">actionName</span><span class="sxs-lookup"><span data-stu-id="a72c6-128">actionName</span></span>|<span data-ttu-id="a72c6-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a72c6-129">String</span></span>|<span data-ttu-id="a72c6-130">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="a72c6-130">Action name</span></span>|
|<span data-ttu-id="a72c6-131">actionState</span><span class="sxs-lookup"><span data-stu-id="a72c6-131">actionState</span></span>|[<span data-ttu-id="a72c6-132">actionState</span><span class="sxs-lookup"><span data-stu-id="a72c6-132">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="a72c6-133">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="a72c6-133">State of the action.</span></span> <span data-ttu-id="a72c6-134">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="a72c6-134">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="a72c6-135">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a72c6-135">startDateTime</span></span>|<span data-ttu-id="a72c6-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a72c6-136">DateTimeOffset</span></span>|<span data-ttu-id="a72c6-137">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="a72c6-137">Time the action was initiated</span></span>|
|<span data-ttu-id="a72c6-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="a72c6-138">lastUpdatedDateTime</span></span>|<span data-ttu-id="a72c6-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a72c6-139">DateTimeOffset</span></span>|<span data-ttu-id="a72c6-140">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="a72c6-140">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="a72c6-141">Relações</span><span class="sxs-lookup"><span data-stu-id="a72c6-141">Relationships</span></span>
<span data-ttu-id="a72c6-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a72c6-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a72c6-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a72c6-143">JSON Representation</span></span>
<span data-ttu-id="a72c6-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a72c6-144">Here is a JSON representation of the resource.</span></span>
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




