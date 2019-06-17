---
title: Tipo de recurso managedDeviceMobileAppConfigurationUserSummary
description: Contém propriedades, propriedades herdadas e ações para um resumo de status do usuário da configuração do aplicativo móvel de MDM.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7793b81ba9bedb8fba6a07beb40ccd4ca3d87a28
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964392"
---
# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="52318-103">Tipo de recurso managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="52318-103">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

> <span data-ttu-id="52318-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="52318-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52318-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="52318-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52318-106">Contém propriedades, propriedades herdadas e ações para um resumo de status do usuário da configuração do aplicativo móvel de MDM.</span><span class="sxs-lookup"><span data-stu-id="52318-106">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>

## <a name="methods"></a><span data-ttu-id="52318-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="52318-107">Methods</span></span>
|<span data-ttu-id="52318-108">Método</span><span class="sxs-lookup"><span data-stu-id="52318-108">Method</span></span>|<span data-ttu-id="52318-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="52318-109">Return Type</span></span>|<span data-ttu-id="52318-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="52318-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="52318-111">Obter managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="52318-111">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-get.md)|[<span data-ttu-id="52318-112">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="52318-112">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="52318-113">Ler propriedades e relações de objetos de [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="52318-113">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="52318-114">Atualizar managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="52318-114">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-update.md)|[<span data-ttu-id="52318-115">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="52318-115">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="52318-116">Atualizar as propriedades de um objeto de [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="52318-116">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="52318-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52318-117">Properties</span></span>
|<span data-ttu-id="52318-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52318-118">Property</span></span>|<span data-ttu-id="52318-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="52318-119">Type</span></span>|<span data-ttu-id="52318-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="52318-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52318-121">id</span><span class="sxs-lookup"><span data-stu-id="52318-121">id</span></span>|<span data-ttu-id="52318-122">String</span><span class="sxs-lookup"><span data-stu-id="52318-122">String</span></span>|<span data-ttu-id="52318-123">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="52318-123">Key of the entity.</span></span>|
|<span data-ttu-id="52318-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="52318-124">pendingCount</span></span>|<span data-ttu-id="52318-125">Int32</span><span class="sxs-lookup"><span data-stu-id="52318-125">Int32</span></span>|<span data-ttu-id="52318-126">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="52318-126">Number of pending Users</span></span>|
|<span data-ttu-id="52318-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="52318-127">notApplicableCount</span></span>|<span data-ttu-id="52318-128">Int32</span><span class="sxs-lookup"><span data-stu-id="52318-128">Int32</span></span>|<span data-ttu-id="52318-129">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="52318-129">Number of not applicable users</span></span>|
|<span data-ttu-id="52318-130">successCount</span><span class="sxs-lookup"><span data-stu-id="52318-130">successCount</span></span>|<span data-ttu-id="52318-131">Int32</span><span class="sxs-lookup"><span data-stu-id="52318-131">Int32</span></span>|<span data-ttu-id="52318-132">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="52318-132">Number of succeeded Users</span></span>|
|<span data-ttu-id="52318-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="52318-133">errorCount</span></span>|<span data-ttu-id="52318-134">Int32</span><span class="sxs-lookup"><span data-stu-id="52318-134">Int32</span></span>|<span data-ttu-id="52318-135">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="52318-135">Number of error Users</span></span>|
|<span data-ttu-id="52318-136">failedCount</span><span class="sxs-lookup"><span data-stu-id="52318-136">failedCount</span></span>|<span data-ttu-id="52318-137">Int32</span><span class="sxs-lookup"><span data-stu-id="52318-137">Int32</span></span>|<span data-ttu-id="52318-138">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="52318-138">Number of failed Users</span></span>|
|<span data-ttu-id="52318-139">conflictCount</span><span class="sxs-lookup"><span data-stu-id="52318-139">conflictCount</span></span>|<span data-ttu-id="52318-140">Int32</span><span class="sxs-lookup"><span data-stu-id="52318-140">Int32</span></span>|<span data-ttu-id="52318-141">Número de usuários em conflito</span><span class="sxs-lookup"><span data-stu-id="52318-141">Number of users in conflict</span></span>|
|<span data-ttu-id="52318-142">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="52318-142">lastUpdateDateTime</span></span>|<span data-ttu-id="52318-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52318-143">DateTimeOffset</span></span>|<span data-ttu-id="52318-144">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="52318-144">Last update time</span></span>|
|<span data-ttu-id="52318-145">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="52318-145">configurationVersion</span></span>|<span data-ttu-id="52318-146">Int32</span><span class="sxs-lookup"><span data-stu-id="52318-146">Int32</span></span>|<span data-ttu-id="52318-147">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="52318-147">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="52318-148">Relações</span><span class="sxs-lookup"><span data-stu-id="52318-148">Relationships</span></span>
<span data-ttu-id="52318-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="52318-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="52318-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52318-150">JSON Representation</span></span>
<span data-ttu-id="52318-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="52318-151">Here is a JSON representation of the resource.</span></span>
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
  "conflictCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```





