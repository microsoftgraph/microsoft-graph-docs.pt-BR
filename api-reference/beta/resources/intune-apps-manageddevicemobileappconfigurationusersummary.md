---
title: Tipo de recurso managedDeviceMobileAppConfigurationUserSummary
description: Contém propriedades, propriedades herdadas e ações para um resumo de status do usuário da configuração do aplicativo móvel de MDM.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d0bbf101d6c4c27a18d46955beac765fae325854
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553992"
---
# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="30815-103">Tipo de recurso managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="30815-103">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

> <span data-ttu-id="30815-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="30815-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30815-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="30815-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30815-106">Contém propriedades, propriedades herdadas e ações para um resumo de status do usuário da configuração do aplicativo móvel de MDM.</span><span class="sxs-lookup"><span data-stu-id="30815-106">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>

## <a name="methods"></a><span data-ttu-id="30815-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="30815-107">Methods</span></span>
|<span data-ttu-id="30815-108">Método</span><span class="sxs-lookup"><span data-stu-id="30815-108">Method</span></span>|<span data-ttu-id="30815-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="30815-109">Return Type</span></span>|<span data-ttu-id="30815-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="30815-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="30815-111">Obter managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="30815-111">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-get.md)|[<span data-ttu-id="30815-112">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="30815-112">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="30815-113">Ler propriedades e relações de objetos de [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="30815-113">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="30815-114">Atualizar managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="30815-114">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-update.md)|[<span data-ttu-id="30815-115">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="30815-115">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="30815-116">Atualizar as propriedades de um objeto de [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="30815-116">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="30815-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="30815-117">Properties</span></span>
|<span data-ttu-id="30815-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="30815-118">Property</span></span>|<span data-ttu-id="30815-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="30815-119">Type</span></span>|<span data-ttu-id="30815-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="30815-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30815-121">id</span><span class="sxs-lookup"><span data-stu-id="30815-121">id</span></span>|<span data-ttu-id="30815-122">String</span><span class="sxs-lookup"><span data-stu-id="30815-122">String</span></span>|<span data-ttu-id="30815-123">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="30815-123">Key of the entity.</span></span>|
|<span data-ttu-id="30815-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="30815-124">pendingCount</span></span>|<span data-ttu-id="30815-125">Int32</span><span class="sxs-lookup"><span data-stu-id="30815-125">Int32</span></span>|<span data-ttu-id="30815-126">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="30815-126">Number of pending Users</span></span>|
|<span data-ttu-id="30815-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="30815-127">notApplicableCount</span></span>|<span data-ttu-id="30815-128">Int32</span><span class="sxs-lookup"><span data-stu-id="30815-128">Int32</span></span>|<span data-ttu-id="30815-129">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="30815-129">Number of not applicable users</span></span>|
|<span data-ttu-id="30815-130">successCount</span><span class="sxs-lookup"><span data-stu-id="30815-130">successCount</span></span>|<span data-ttu-id="30815-131">Int32</span><span class="sxs-lookup"><span data-stu-id="30815-131">Int32</span></span>|<span data-ttu-id="30815-132">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="30815-132">Number of succeeded Users</span></span>|
|<span data-ttu-id="30815-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="30815-133">errorCount</span></span>|<span data-ttu-id="30815-134">Int32</span><span class="sxs-lookup"><span data-stu-id="30815-134">Int32</span></span>|<span data-ttu-id="30815-135">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="30815-135">Number of error Users</span></span>|
|<span data-ttu-id="30815-136">failedCount</span><span class="sxs-lookup"><span data-stu-id="30815-136">failedCount</span></span>|<span data-ttu-id="30815-137">Int32</span><span class="sxs-lookup"><span data-stu-id="30815-137">Int32</span></span>|<span data-ttu-id="30815-138">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="30815-138">Number of failed Users</span></span>|
|<span data-ttu-id="30815-139">conflictCount</span><span class="sxs-lookup"><span data-stu-id="30815-139">conflictCount</span></span>|<span data-ttu-id="30815-140">Int32</span><span class="sxs-lookup"><span data-stu-id="30815-140">Int32</span></span>|<span data-ttu-id="30815-141">Número de usuários em conflito</span><span class="sxs-lookup"><span data-stu-id="30815-141">Number of users in conflict</span></span>|
|<span data-ttu-id="30815-142">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="30815-142">lastUpdateDateTime</span></span>|<span data-ttu-id="30815-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30815-143">DateTimeOffset</span></span>|<span data-ttu-id="30815-144">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="30815-144">Last update time</span></span>|
|<span data-ttu-id="30815-145">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="30815-145">configurationVersion</span></span>|<span data-ttu-id="30815-146">Int32</span><span class="sxs-lookup"><span data-stu-id="30815-146">Int32</span></span>|<span data-ttu-id="30815-147">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="30815-147">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="30815-148">Relações</span><span class="sxs-lookup"><span data-stu-id="30815-148">Relationships</span></span>
<span data-ttu-id="30815-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="30815-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="30815-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="30815-150">JSON Representation</span></span>
<span data-ttu-id="30815-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="30815-151">Here is a JSON representation of the resource.</span></span>
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





