---
title: Tipo de recurso managedDeviceMobileAppConfigurationUserSummary
description: Contém propriedades, propriedades herdadas e ações para um resumo de status do usuário da configuração do aplicativo móvel de MDM.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 608353667b4e9d8a16b699d3390cbb7e04eaf9a0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054669"
---
# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="f98bb-103">Tipo de recurso managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="f98bb-103">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

<span data-ttu-id="f98bb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f98bb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f98bb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f98bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f98bb-106">Contém propriedades, propriedades herdadas e ações para um resumo de status do usuário da configuração do aplicativo móvel de MDM.</span><span class="sxs-lookup"><span data-stu-id="f98bb-106">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>

## <a name="methods"></a><span data-ttu-id="f98bb-107">Methods</span><span class="sxs-lookup"><span data-stu-id="f98bb-107">Methods</span></span>
|<span data-ttu-id="f98bb-108">Método</span><span class="sxs-lookup"><span data-stu-id="f98bb-108">Method</span></span>|<span data-ttu-id="f98bb-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f98bb-109">Return Type</span></span>|<span data-ttu-id="f98bb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f98bb-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f98bb-111">Obter managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="f98bb-111">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-get.md)|[<span data-ttu-id="f98bb-112">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="f98bb-112">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="f98bb-113">Ler propriedades e relações de objetos de [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="f98bb-113">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="f98bb-114">Atualizar managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="f98bb-114">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-update.md)|[<span data-ttu-id="f98bb-115">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="f98bb-115">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="f98bb-116">Atualizar as propriedades de um objeto de [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="f98bb-116">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f98bb-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f98bb-117">Properties</span></span>
|<span data-ttu-id="f98bb-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f98bb-118">Property</span></span>|<span data-ttu-id="f98bb-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="f98bb-119">Type</span></span>|<span data-ttu-id="f98bb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f98bb-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f98bb-121">id</span><span class="sxs-lookup"><span data-stu-id="f98bb-121">id</span></span>|<span data-ttu-id="f98bb-122">String</span><span class="sxs-lookup"><span data-stu-id="f98bb-122">String</span></span>|<span data-ttu-id="f98bb-123">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f98bb-123">Key of the entity.</span></span>|
|<span data-ttu-id="f98bb-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="f98bb-124">pendingCount</span></span>|<span data-ttu-id="f98bb-125">Int32</span><span class="sxs-lookup"><span data-stu-id="f98bb-125">Int32</span></span>|<span data-ttu-id="f98bb-126">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="f98bb-126">Number of pending Users</span></span>|
|<span data-ttu-id="f98bb-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="f98bb-127">notApplicableCount</span></span>|<span data-ttu-id="f98bb-128">Int32</span><span class="sxs-lookup"><span data-stu-id="f98bb-128">Int32</span></span>|<span data-ttu-id="f98bb-129">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="f98bb-129">Number of not applicable users</span></span>|
|<span data-ttu-id="f98bb-130">successCount</span><span class="sxs-lookup"><span data-stu-id="f98bb-130">successCount</span></span>|<span data-ttu-id="f98bb-131">Int32</span><span class="sxs-lookup"><span data-stu-id="f98bb-131">Int32</span></span>|<span data-ttu-id="f98bb-132">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="f98bb-132">Number of succeeded Users</span></span>|
|<span data-ttu-id="f98bb-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="f98bb-133">errorCount</span></span>|<span data-ttu-id="f98bb-134">Int32</span><span class="sxs-lookup"><span data-stu-id="f98bb-134">Int32</span></span>|<span data-ttu-id="f98bb-135">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="f98bb-135">Number of error Users</span></span>|
|<span data-ttu-id="f98bb-136">failedCount</span><span class="sxs-lookup"><span data-stu-id="f98bb-136">failedCount</span></span>|<span data-ttu-id="f98bb-137">Int32</span><span class="sxs-lookup"><span data-stu-id="f98bb-137">Int32</span></span>|<span data-ttu-id="f98bb-138">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="f98bb-138">Number of failed Users</span></span>|
|<span data-ttu-id="f98bb-139">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="f98bb-139">lastUpdateDateTime</span></span>|<span data-ttu-id="f98bb-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f98bb-140">DateTimeOffset</span></span>|<span data-ttu-id="f98bb-141">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="f98bb-141">Last update time</span></span>|
|<span data-ttu-id="f98bb-142">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="f98bb-142">configurationVersion</span></span>|<span data-ttu-id="f98bb-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f98bb-143">Int32</span></span>|<span data-ttu-id="f98bb-144">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="f98bb-144">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="f98bb-145">Relações</span><span class="sxs-lookup"><span data-stu-id="f98bb-145">Relationships</span></span>
<span data-ttu-id="f98bb-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f98bb-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f98bb-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f98bb-147">JSON Representation</span></span>
<span data-ttu-id="f98bb-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f98bb-148">Here is a JSON representation of the resource.</span></span>
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









