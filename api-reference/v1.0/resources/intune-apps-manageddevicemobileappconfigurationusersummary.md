---
title: Tipo de recurso managedDeviceMobileAppConfigurationUserSummary
description: Contém propriedades, propriedades herdadas e ações para um resumo de status do usuário da configuração do aplicativo móvel de MDM.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 385e9ac51b10d97e425cf19acb10007402eeeeb4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934888"
---
# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="50580-103">Tipo de recurso managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="50580-103">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

> <span data-ttu-id="50580-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="50580-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="50580-105">Contém propriedades, propriedades herdadas e ações para um resumo de status do usuário da configuração do aplicativo móvel de MDM.</span><span class="sxs-lookup"><span data-stu-id="50580-105">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>
## <a name="methods"></a><span data-ttu-id="50580-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="50580-106">Methods</span></span>
|<span data-ttu-id="50580-107">Método</span><span class="sxs-lookup"><span data-stu-id="50580-107">Method</span></span>|<span data-ttu-id="50580-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="50580-108">Return Type</span></span>|<span data-ttu-id="50580-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="50580-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="50580-110">Obter managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="50580-110">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-get.md)|[<span data-ttu-id="50580-111">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="50580-111">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="50580-112">Ler propriedades e relações de objetos de [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="50580-112">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="50580-113">Atualizar managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="50580-113">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-update.md)|[<span data-ttu-id="50580-114">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="50580-114">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="50580-115">Atualizar as propriedades de um objeto de [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="50580-115">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="50580-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="50580-116">Properties</span></span>
|<span data-ttu-id="50580-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50580-117">Property</span></span>|<span data-ttu-id="50580-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="50580-118">Type</span></span>|<span data-ttu-id="50580-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="50580-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50580-120">id</span><span class="sxs-lookup"><span data-stu-id="50580-120">id</span></span>|<span data-ttu-id="50580-121">String</span><span class="sxs-lookup"><span data-stu-id="50580-121">String</span></span>|<span data-ttu-id="50580-122">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="50580-122">Key of the entity.</span></span>|
|<span data-ttu-id="50580-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="50580-123">pendingCount</span></span>|<span data-ttu-id="50580-124">Int32</span><span class="sxs-lookup"><span data-stu-id="50580-124">Int32</span></span>|<span data-ttu-id="50580-125">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="50580-125">Number of pending Users</span></span>|
|<span data-ttu-id="50580-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="50580-126">notApplicableCount</span></span>|<span data-ttu-id="50580-127">Int32</span><span class="sxs-lookup"><span data-stu-id="50580-127">Int32</span></span>|<span data-ttu-id="50580-128">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="50580-128">Number of not applicable users</span></span>|
|<span data-ttu-id="50580-129">successCount</span><span class="sxs-lookup"><span data-stu-id="50580-129">successCount</span></span>|<span data-ttu-id="50580-130">Int32</span><span class="sxs-lookup"><span data-stu-id="50580-130">Int32</span></span>|<span data-ttu-id="50580-131">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="50580-131">Number of succeeded Users</span></span>|
|<span data-ttu-id="50580-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="50580-132">errorCount</span></span>|<span data-ttu-id="50580-133">Int32</span><span class="sxs-lookup"><span data-stu-id="50580-133">Int32</span></span>|<span data-ttu-id="50580-134">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="50580-134">Number of error Users</span></span>|
|<span data-ttu-id="50580-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="50580-135">failedCount</span></span>|<span data-ttu-id="50580-136">Int32</span><span class="sxs-lookup"><span data-stu-id="50580-136">Int32</span></span>|<span data-ttu-id="50580-137">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="50580-137">Number of failed Users</span></span>|
|<span data-ttu-id="50580-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="50580-138">lastUpdateDateTime</span></span>|<span data-ttu-id="50580-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50580-139">DateTimeOffset</span></span>|<span data-ttu-id="50580-140">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="50580-140">Last update time</span></span>|
|<span data-ttu-id="50580-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="50580-141">configurationVersion</span></span>|<span data-ttu-id="50580-142">Int32</span><span class="sxs-lookup"><span data-stu-id="50580-142">Int32</span></span>|<span data-ttu-id="50580-143">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="50580-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="50580-144">Relações</span><span class="sxs-lookup"><span data-stu-id="50580-144">Relationships</span></span>
<span data-ttu-id="50580-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="50580-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="50580-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="50580-146">JSON Representation</span></span>
<span data-ttu-id="50580-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="50580-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationUserSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```



