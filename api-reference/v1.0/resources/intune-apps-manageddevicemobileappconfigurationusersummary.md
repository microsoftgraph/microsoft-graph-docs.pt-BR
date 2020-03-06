---
title: Tipo de recurso managedDeviceMobileAppConfigurationUserSummary
description: Contém propriedades, propriedades herdadas e ações para um resumo de status do usuário da configuração do aplicativo móvel de MDM.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4db930c4c36fd0f3e6d26347f17dbb739e19e188
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531171"
---
# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="b7485-103">Tipo de recurso managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="b7485-103">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

<span data-ttu-id="b7485-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7485-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b7485-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b7485-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7485-106">Contém propriedades, propriedades herdadas e ações para um resumo de status do usuário da configuração do aplicativo móvel de MDM.</span><span class="sxs-lookup"><span data-stu-id="b7485-106">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>

## <a name="methods"></a><span data-ttu-id="b7485-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="b7485-107">Methods</span></span>
|<span data-ttu-id="b7485-108">Método</span><span class="sxs-lookup"><span data-stu-id="b7485-108">Method</span></span>|<span data-ttu-id="b7485-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b7485-109">Return Type</span></span>|<span data-ttu-id="b7485-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7485-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b7485-111">Obter managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="b7485-111">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-get.md)|[<span data-ttu-id="b7485-112">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="b7485-112">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="b7485-113">Ler propriedades e relações de objetos de [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="b7485-113">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="b7485-114">Atualizar managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="b7485-114">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-update.md)|[<span data-ttu-id="b7485-115">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="b7485-115">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="b7485-116">Atualizar as propriedades de um objeto de [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="b7485-116">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b7485-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b7485-117">Properties</span></span>
|<span data-ttu-id="b7485-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7485-118">Property</span></span>|<span data-ttu-id="b7485-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7485-119">Type</span></span>|<span data-ttu-id="b7485-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7485-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7485-121">id</span><span class="sxs-lookup"><span data-stu-id="b7485-121">id</span></span>|<span data-ttu-id="b7485-122">String</span><span class="sxs-lookup"><span data-stu-id="b7485-122">String</span></span>|<span data-ttu-id="b7485-123">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b7485-123">Key of the entity.</span></span>|
|<span data-ttu-id="b7485-124">pendingCount</span><span class="sxs-lookup"><span data-stu-id="b7485-124">pendingCount</span></span>|<span data-ttu-id="b7485-125">Int32</span><span class="sxs-lookup"><span data-stu-id="b7485-125">Int32</span></span>|<span data-ttu-id="b7485-126">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="b7485-126">Number of pending Users</span></span>|
|<span data-ttu-id="b7485-127">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="b7485-127">notApplicableCount</span></span>|<span data-ttu-id="b7485-128">Int32</span><span class="sxs-lookup"><span data-stu-id="b7485-128">Int32</span></span>|<span data-ttu-id="b7485-129">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="b7485-129">Number of not applicable users</span></span>|
|<span data-ttu-id="b7485-130">successCount</span><span class="sxs-lookup"><span data-stu-id="b7485-130">successCount</span></span>|<span data-ttu-id="b7485-131">Int32</span><span class="sxs-lookup"><span data-stu-id="b7485-131">Int32</span></span>|<span data-ttu-id="b7485-132">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="b7485-132">Number of succeeded Users</span></span>|
|<span data-ttu-id="b7485-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="b7485-133">errorCount</span></span>|<span data-ttu-id="b7485-134">Int32</span><span class="sxs-lookup"><span data-stu-id="b7485-134">Int32</span></span>|<span data-ttu-id="b7485-135">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="b7485-135">Number of error Users</span></span>|
|<span data-ttu-id="b7485-136">failedCount</span><span class="sxs-lookup"><span data-stu-id="b7485-136">failedCount</span></span>|<span data-ttu-id="b7485-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b7485-137">Int32</span></span>|<span data-ttu-id="b7485-138">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="b7485-138">Number of failed Users</span></span>|
|<span data-ttu-id="b7485-139">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="b7485-139">lastUpdateDateTime</span></span>|<span data-ttu-id="b7485-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7485-140">DateTimeOffset</span></span>|<span data-ttu-id="b7485-141">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="b7485-141">Last update time</span></span>|
|<span data-ttu-id="b7485-142">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="b7485-142">configurationVersion</span></span>|<span data-ttu-id="b7485-143">Int32</span><span class="sxs-lookup"><span data-stu-id="b7485-143">Int32</span></span>|<span data-ttu-id="b7485-144">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="b7485-144">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7485-145">Relações</span><span class="sxs-lookup"><span data-stu-id="b7485-145">Relationships</span></span>
<span data-ttu-id="b7485-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b7485-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7485-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b7485-147">JSON Representation</span></span>
<span data-ttu-id="b7485-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b7485-148">Here is a JSON representation of the resource.</span></span>
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




