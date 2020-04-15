---
title: Tipo de recurso managedDeviceMobileAppConfigurationUserSummary
description: Contém propriedades, propriedades herdadas e ações para um resumo de status do usuário da configuração do aplicativo móvel de MDM.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 99311c3fca0d1b1ecbe701057c9172d723ae8f05
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43474174"
---
# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="63dab-103">Tipo de recurso managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="63dab-103">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

<span data-ttu-id="63dab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63dab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63dab-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="63dab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63dab-106">Contém propriedades, propriedades herdadas e ações para um resumo de status do usuário da configuração do aplicativo móvel de MDM.</span><span class="sxs-lookup"><span data-stu-id="63dab-106">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>

## <a name="methods"></a><span data-ttu-id="63dab-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="63dab-107">Methods</span></span>
|<span data-ttu-id="63dab-108">Método</span><span class="sxs-lookup"><span data-stu-id="63dab-108">Method</span></span>|<span data-ttu-id="63dab-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="63dab-109">Return Type</span></span>|<span data-ttu-id="63dab-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="63dab-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="63dab-111">Obter managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="63dab-111">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-get.md)|[<span data-ttu-id="63dab-112">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="63dab-112">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="63dab-113">Ler propriedades e relações de objetos de [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="63dab-113">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="63dab-114">Atualizar managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="63dab-114">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-update.md)|[<span data-ttu-id="63dab-115">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="63dab-115">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="63dab-116">Atualizar as propriedades de um objeto de [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="63dab-116">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="63dab-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="63dab-117">Properties</span></span>
|<span data-ttu-id="63dab-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63dab-118">Property</span></span>|<span data-ttu-id="63dab-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="63dab-119">Type</span></span>|<span data-ttu-id="63dab-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="63dab-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63dab-121">id</span><span class="sxs-lookup"><span data-stu-id="63dab-121">id</span></span>|<span data-ttu-id="63dab-122">String</span><span class="sxs-lookup"><span data-stu-id="63dab-122">String</span></span>|<span data-ttu-id="63dab-123">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="63dab-123">Key of the entity.</span></span>|
|<span data-ttu-id="63dab-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="63dab-124">pendingCount</span></span>|<span data-ttu-id="63dab-125">Int32</span><span class="sxs-lookup"><span data-stu-id="63dab-125">Int32</span></span>|<span data-ttu-id="63dab-126">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="63dab-126">Number of pending Users</span></span>|
|<span data-ttu-id="63dab-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="63dab-127">notApplicableCount</span></span>|<span data-ttu-id="63dab-128">Int32</span><span class="sxs-lookup"><span data-stu-id="63dab-128">Int32</span></span>|<span data-ttu-id="63dab-129">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="63dab-129">Number of not applicable users</span></span>|
|<span data-ttu-id="63dab-130">successCount</span><span class="sxs-lookup"><span data-stu-id="63dab-130">successCount</span></span>|<span data-ttu-id="63dab-131">Int32</span><span class="sxs-lookup"><span data-stu-id="63dab-131">Int32</span></span>|<span data-ttu-id="63dab-132">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="63dab-132">Number of succeeded Users</span></span>|
|<span data-ttu-id="63dab-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="63dab-133">errorCount</span></span>|<span data-ttu-id="63dab-134">Int32</span><span class="sxs-lookup"><span data-stu-id="63dab-134">Int32</span></span>|<span data-ttu-id="63dab-135">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="63dab-135">Number of error Users</span></span>|
|<span data-ttu-id="63dab-136">failedCount</span><span class="sxs-lookup"><span data-stu-id="63dab-136">failedCount</span></span>|<span data-ttu-id="63dab-137">Int32</span><span class="sxs-lookup"><span data-stu-id="63dab-137">Int32</span></span>|<span data-ttu-id="63dab-138">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="63dab-138">Number of failed Users</span></span>|
|<span data-ttu-id="63dab-139">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="63dab-139">lastUpdateDateTime</span></span>|<span data-ttu-id="63dab-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63dab-140">DateTimeOffset</span></span>|<span data-ttu-id="63dab-141">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="63dab-141">Last update time</span></span>|
|<span data-ttu-id="63dab-142">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="63dab-142">configurationVersion</span></span>|<span data-ttu-id="63dab-143">Int32</span><span class="sxs-lookup"><span data-stu-id="63dab-143">Int32</span></span>|<span data-ttu-id="63dab-144">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="63dab-144">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="63dab-145">Relações</span><span class="sxs-lookup"><span data-stu-id="63dab-145">Relationships</span></span>
<span data-ttu-id="63dab-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="63dab-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="63dab-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="63dab-147">JSON Representation</span></span>
<span data-ttu-id="63dab-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="63dab-148">Here is a JSON representation of the resource.</span></span>
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







