---
title: Tipo de recurso managedDeviceMobileAppConfigurationUserSummary
description: Contém propriedades, propriedades herdadas e ações para um resumo de status do usuário da configuração do aplicativo móvel de MDM.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 42960156bd02f45117abb4974f0701ff6bc15568
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37368194"
---
# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="6b165-103">Tipo de recurso managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="6b165-103">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

> <span data-ttu-id="6b165-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6b165-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b165-105">Contém propriedades, propriedades herdadas e ações para um resumo de status do usuário da configuração do aplicativo móvel de MDM.</span><span class="sxs-lookup"><span data-stu-id="6b165-105">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>

## <a name="methods"></a><span data-ttu-id="6b165-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="6b165-106">Methods</span></span>
|<span data-ttu-id="6b165-107">Método</span><span class="sxs-lookup"><span data-stu-id="6b165-107">Method</span></span>|<span data-ttu-id="6b165-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6b165-108">Return Type</span></span>|<span data-ttu-id="6b165-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b165-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6b165-110">Obter managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="6b165-110">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-get.md)|[<span data-ttu-id="6b165-111">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="6b165-111">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="6b165-112">Ler propriedades e relações de objetos de [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="6b165-112">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="6b165-113">Atualizar managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="6b165-113">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-update.md)|[<span data-ttu-id="6b165-114">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="6b165-114">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="6b165-115">Atualizar as propriedades de um objeto de [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="6b165-115">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6b165-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6b165-116">Properties</span></span>
|<span data-ttu-id="6b165-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b165-117">Property</span></span>|<span data-ttu-id="6b165-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b165-118">Type</span></span>|<span data-ttu-id="6b165-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b165-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b165-120">id</span><span class="sxs-lookup"><span data-stu-id="6b165-120">id</span></span>|<span data-ttu-id="6b165-121">String</span><span class="sxs-lookup"><span data-stu-id="6b165-121">String</span></span>|<span data-ttu-id="6b165-122">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6b165-122">Key of the entity.</span></span>|
|<span data-ttu-id="6b165-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="6b165-123">pendingCount</span></span>|<span data-ttu-id="6b165-124">Int32</span><span class="sxs-lookup"><span data-stu-id="6b165-124">Int32</span></span>|<span data-ttu-id="6b165-125">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="6b165-125">Number of pending Users</span></span>|
|<span data-ttu-id="6b165-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="6b165-126">notApplicableCount</span></span>|<span data-ttu-id="6b165-127">Int32</span><span class="sxs-lookup"><span data-stu-id="6b165-127">Int32</span></span>|<span data-ttu-id="6b165-128">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="6b165-128">Number of not applicable users</span></span>|
|<span data-ttu-id="6b165-129">successCount</span><span class="sxs-lookup"><span data-stu-id="6b165-129">successCount</span></span>|<span data-ttu-id="6b165-130">Int32</span><span class="sxs-lookup"><span data-stu-id="6b165-130">Int32</span></span>|<span data-ttu-id="6b165-131">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="6b165-131">Number of succeeded Users</span></span>|
|<span data-ttu-id="6b165-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="6b165-132">errorCount</span></span>|<span data-ttu-id="6b165-133">Int32</span><span class="sxs-lookup"><span data-stu-id="6b165-133">Int32</span></span>|<span data-ttu-id="6b165-134">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="6b165-134">Number of error Users</span></span>|
|<span data-ttu-id="6b165-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="6b165-135">failedCount</span></span>|<span data-ttu-id="6b165-136">Int32</span><span class="sxs-lookup"><span data-stu-id="6b165-136">Int32</span></span>|<span data-ttu-id="6b165-137">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="6b165-137">Number of failed Users</span></span>|
|<span data-ttu-id="6b165-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="6b165-138">lastUpdateDateTime</span></span>|<span data-ttu-id="6b165-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b165-139">DateTimeOffset</span></span>|<span data-ttu-id="6b165-140">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="6b165-140">Last update time</span></span>|
|<span data-ttu-id="6b165-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="6b165-141">configurationVersion</span></span>|<span data-ttu-id="6b165-142">Int32</span><span class="sxs-lookup"><span data-stu-id="6b165-142">Int32</span></span>|<span data-ttu-id="6b165-143">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="6b165-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b165-144">Relações</span><span class="sxs-lookup"><span data-stu-id="6b165-144">Relationships</span></span>
<span data-ttu-id="6b165-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6b165-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b165-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6b165-146">JSON Representation</span></span>
<span data-ttu-id="6b165-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6b165-147">Here is a JSON representation of the resource.</span></span>
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




