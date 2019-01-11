---
title: tipo de recurso de iosVppAppRevokeLicensesActionResult
description: Define os resultados para ações em iOS Vpp Apps, contém as propriedades herdadas para ActionResult.
localization_priority: Normal
ms.openlocfilehash: 8ed57465e263245cfc18ca22899c2142d949855d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842081"
---
# <a name="iosvppapprevokelicensesactionresult-resource-type"></a><span data-ttu-id="1a1e9-103">tipo de recurso de iosVppAppRevokeLicensesActionResult</span><span class="sxs-lookup"><span data-stu-id="1a1e9-103">iosVppAppRevokeLicensesActionResult resource type</span></span>

> <span data-ttu-id="1a1e9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1a1e9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a1e9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1a1e9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1a1e9-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1a1e9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1a1e9-107">Define os resultados para ações em iOS Vpp Apps, contém as propriedades herdadas para ActionResult.</span><span class="sxs-lookup"><span data-stu-id="1a1e9-107">Defines results for actions on iOS Vpp Apps, contains inherited properties for ActionResult.</span></span>
## <a name="properties"></a><span data-ttu-id="1a1e9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1a1e9-108">Properties</span></span>
|<span data-ttu-id="1a1e9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a1e9-109">Property</span></span>|<span data-ttu-id="1a1e9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a1e9-110">Type</span></span>|<span data-ttu-id="1a1e9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a1e9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a1e9-112">userId</span><span class="sxs-lookup"><span data-stu-id="1a1e9-112">userId</span></span>|<span data-ttu-id="1a1e9-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a1e9-113">String</span></span>|<span data-ttu-id="1a1e9-114">ID de usuário associado à ação.</span><span class="sxs-lookup"><span data-stu-id="1a1e9-114">UserId associated with the action.</span></span>|
|<span data-ttu-id="1a1e9-115">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="1a1e9-115">managedDeviceId</span></span>|<span data-ttu-id="1a1e9-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a1e9-116">String</span></span>|<span data-ttu-id="1a1e9-117">DeviceId associado à ação.</span><span class="sxs-lookup"><span data-stu-id="1a1e9-117">DeviceId associated with the action.</span></span>|
|<span data-ttu-id="1a1e9-118">totalLicensesCount</span><span class="sxs-lookup"><span data-stu-id="1a1e9-118">totalLicensesCount</span></span>|<span data-ttu-id="1a1e9-119">Int32</span><span class="sxs-lookup"><span data-stu-id="1a1e9-119">Int32</span></span>|<span data-ttu-id="1a1e9-120">Uma contagem do número de licenças para o qual revoke foi tentada.</span><span class="sxs-lookup"><span data-stu-id="1a1e9-120">A count of the number of licenses for which revoke was attempted.</span></span>|
|<span data-ttu-id="1a1e9-121">failedLicensesCount</span><span class="sxs-lookup"><span data-stu-id="1a1e9-121">failedLicensesCount</span></span>|<span data-ttu-id="1a1e9-122">Int32</span><span class="sxs-lookup"><span data-stu-id="1a1e9-122">Int32</span></span>|<span data-ttu-id="1a1e9-123">Uma contagem do número de licenças para o qual revoke falhou.</span><span class="sxs-lookup"><span data-stu-id="1a1e9-123">A count of the number of licenses for which revoke failed.</span></span>|
|<span data-ttu-id="1a1e9-124">actionFailureReason</span><span class="sxs-lookup"><span data-stu-id="1a1e9-124">actionFailureReason</span></span>|[<span data-ttu-id="1a1e9-125">vppTokenActionFailureReason</span><span class="sxs-lookup"><span data-stu-id="1a1e9-125">vppTokenActionFailureReason</span></span>](../resources/intune-shared-vpptokenactionfailurereason.md)|<span data-ttu-id="1a1e9-126">O motivo da falha de ação de licenças revoke.</span><span class="sxs-lookup"><span data-stu-id="1a1e9-126">The reason for the revoke licenses action failure.</span></span> <span data-ttu-id="1a1e9-127">Os valores possíveis são: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span><span class="sxs-lookup"><span data-stu-id="1a1e9-127">Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.</span></span>|
|<span data-ttu-id="1a1e9-128">actionName</span><span class="sxs-lookup"><span data-stu-id="1a1e9-128">actionName</span></span>|<span data-ttu-id="1a1e9-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a1e9-129">String</span></span>|<span data-ttu-id="1a1e9-130">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="1a1e9-130">Action name</span></span>|
|<span data-ttu-id="1a1e9-131">actionState</span><span class="sxs-lookup"><span data-stu-id="1a1e9-131">actionState</span></span>|[<span data-ttu-id="1a1e9-132">actionState</span><span class="sxs-lookup"><span data-stu-id="1a1e9-132">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="1a1e9-133">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="1a1e9-133">State of the action.</span></span> <span data-ttu-id="1a1e9-134">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="1a1e9-134">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="1a1e9-135">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1a1e9-135">startDateTime</span></span>|<span data-ttu-id="1a1e9-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a1e9-136">DateTimeOffset</span></span>|<span data-ttu-id="1a1e9-137">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="1a1e9-137">Time the action was initiated</span></span>|
|<span data-ttu-id="1a1e9-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a1e9-138">lastUpdatedDateTime</span></span>|<span data-ttu-id="1a1e9-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a1e9-139">DateTimeOffset</span></span>|<span data-ttu-id="1a1e9-140">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="1a1e9-140">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a1e9-141">Relações</span><span class="sxs-lookup"><span data-stu-id="1a1e9-141">Relationships</span></span>
<span data-ttu-id="1a1e9-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1a1e9-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1a1e9-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1a1e9-143">JSON Representation</span></span>
<span data-ttu-id="1a1e9-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1a1e9-144">Here is a JSON representation of the resource.</span></span>
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





