---
title: Tipo de recurso managedDeviceMobileAppConfigurationUserSummary
description: Contém propriedades, propriedades herdadas e ações para um resumo de status do usuário da configuração do aplicativo móvel de MDM.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 34f6d8254e743f4a294d2351c291631d2ae65a51
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399868"
---
# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="067ef-103">Tipo de recurso managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="067ef-103">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

> <span data-ttu-id="067ef-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="067ef-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="067ef-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="067ef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="067ef-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="067ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="067ef-107">Contém propriedades, propriedades herdadas e ações para um resumo de status do usuário da configuração do aplicativo móvel de MDM.</span><span class="sxs-lookup"><span data-stu-id="067ef-107">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>

## <a name="methods"></a><span data-ttu-id="067ef-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="067ef-108">Methods</span></span>
|<span data-ttu-id="067ef-109">Método</span><span class="sxs-lookup"><span data-stu-id="067ef-109">Method</span></span>|<span data-ttu-id="067ef-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="067ef-110">Return Type</span></span>|<span data-ttu-id="067ef-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="067ef-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="067ef-112">Obter managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="067ef-112">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-get.md)|[<span data-ttu-id="067ef-113">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="067ef-113">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="067ef-114">Ler propriedades e relações de objetos de [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="067ef-114">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="067ef-115">Atualizar managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="067ef-115">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-update.md)|[<span data-ttu-id="067ef-116">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="067ef-116">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="067ef-117">Atualizar as propriedades de um objeto de [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="067ef-117">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="067ef-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="067ef-118">Properties</span></span>
|<span data-ttu-id="067ef-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="067ef-119">Property</span></span>|<span data-ttu-id="067ef-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="067ef-120">Type</span></span>|<span data-ttu-id="067ef-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="067ef-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="067ef-122">id</span><span class="sxs-lookup"><span data-stu-id="067ef-122">id</span></span>|<span data-ttu-id="067ef-123">String</span><span class="sxs-lookup"><span data-stu-id="067ef-123">String</span></span>|<span data-ttu-id="067ef-124">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="067ef-124">Key of the entity.</span></span>|
|<span data-ttu-id="067ef-125">pendingCount</span><span class="sxs-lookup"><span data-stu-id="067ef-125">pendingCount</span></span>|<span data-ttu-id="067ef-126">Int32</span><span class="sxs-lookup"><span data-stu-id="067ef-126">Int32</span></span>|<span data-ttu-id="067ef-127">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="067ef-127">Number of pending Users</span></span>|
|<span data-ttu-id="067ef-128">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="067ef-128">notApplicableCount</span></span>|<span data-ttu-id="067ef-129">Int32</span><span class="sxs-lookup"><span data-stu-id="067ef-129">Int32</span></span>|<span data-ttu-id="067ef-130">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="067ef-130">Number of not applicable users</span></span>|
|<span data-ttu-id="067ef-131">successCount</span><span class="sxs-lookup"><span data-stu-id="067ef-131">successCount</span></span>|<span data-ttu-id="067ef-132">Int32</span><span class="sxs-lookup"><span data-stu-id="067ef-132">Int32</span></span>|<span data-ttu-id="067ef-133">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="067ef-133">Number of succeeded Users</span></span>|
|<span data-ttu-id="067ef-134">errorCount</span><span class="sxs-lookup"><span data-stu-id="067ef-134">errorCount</span></span>|<span data-ttu-id="067ef-135">Int32</span><span class="sxs-lookup"><span data-stu-id="067ef-135">Int32</span></span>|<span data-ttu-id="067ef-136">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="067ef-136">Number of error Users</span></span>|
|<span data-ttu-id="067ef-137">failedCount</span><span class="sxs-lookup"><span data-stu-id="067ef-137">failedCount</span></span>|<span data-ttu-id="067ef-138">Int32</span><span class="sxs-lookup"><span data-stu-id="067ef-138">Int32</span></span>|<span data-ttu-id="067ef-139">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="067ef-139">Number of failed Users</span></span>|
|<span data-ttu-id="067ef-140">conflictCount</span><span class="sxs-lookup"><span data-stu-id="067ef-140">conflictCount</span></span>|<span data-ttu-id="067ef-141">Int32</span><span class="sxs-lookup"><span data-stu-id="067ef-141">Int32</span></span>|<span data-ttu-id="067ef-142">Número de usuários em conflito</span><span class="sxs-lookup"><span data-stu-id="067ef-142">Number of users in conflict</span></span>|
|<span data-ttu-id="067ef-143">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="067ef-143">lastUpdateDateTime</span></span>|<span data-ttu-id="067ef-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="067ef-144">DateTimeOffset</span></span>|<span data-ttu-id="067ef-145">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="067ef-145">Last update time</span></span>|
|<span data-ttu-id="067ef-146">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="067ef-146">configurationVersion</span></span>|<span data-ttu-id="067ef-147">Int32</span><span class="sxs-lookup"><span data-stu-id="067ef-147">Int32</span></span>|<span data-ttu-id="067ef-148">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="067ef-148">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="067ef-149">Relações</span><span class="sxs-lookup"><span data-stu-id="067ef-149">Relationships</span></span>
<span data-ttu-id="067ef-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="067ef-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="067ef-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="067ef-151">JSON Representation</span></span>
<span data-ttu-id="067ef-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="067ef-152">Here is a JSON representation of the resource.</span></span>
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




