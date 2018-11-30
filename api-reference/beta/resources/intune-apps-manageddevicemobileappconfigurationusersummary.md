---
title: Tipo de recurso managedDeviceMobileAppConfigurationUserSummary
description: Contém propriedades, propriedades herdadas e ações para um resumo de status do usuário da configuração do aplicativo móvel de MDM.
ms.openlocfilehash: b27f4c24dc4b89238ec4e555d9507f36795ebc9b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036043"
---
# <a name="manageddevicemobileappconfigurationusersummary-resource-type"></a><span data-ttu-id="68033-103">Tipo de recurso managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="68033-103">managedDeviceMobileAppConfigurationUserSummary resource type</span></span>

> <span data-ttu-id="68033-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="68033-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="68033-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="68033-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="68033-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="68033-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68033-107">Contém propriedades, propriedades herdadas e ações para um resumo de status do usuário da configuração do aplicativo móvel de MDM.</span><span class="sxs-lookup"><span data-stu-id="68033-107">Contains properties, inherited properties and actions for an MDM mobile app configuration user status summary.</span></span>
## <a name="methods"></a><span data-ttu-id="68033-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="68033-108">Methods</span></span>
|<span data-ttu-id="68033-109">Método</span><span class="sxs-lookup"><span data-stu-id="68033-109">Method</span></span>|<span data-ttu-id="68033-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="68033-110">Return Type</span></span>|<span data-ttu-id="68033-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="68033-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="68033-112">Obter managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="68033-112">Get managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-get.md)|[<span data-ttu-id="68033-113">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="68033-113">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="68033-114">Ler propriedades e relações de objetos de [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="68033-114">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|
|[<span data-ttu-id="68033-115">Atualizar managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="68033-115">Update managedDeviceMobileAppConfigurationUserSummary</span></span>](../api/intune-apps-manageddevicemobileappconfigurationusersummary-update.md)|[<span data-ttu-id="68033-116">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="68033-116">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="68033-117">Atualizar as propriedades de um objeto de [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="68033-117">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="68033-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="68033-118">Properties</span></span>
|<span data-ttu-id="68033-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68033-119">Property</span></span>|<span data-ttu-id="68033-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="68033-120">Type</span></span>|<span data-ttu-id="68033-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="68033-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68033-122">id</span><span class="sxs-lookup"><span data-stu-id="68033-122">id</span></span>|<span data-ttu-id="68033-123">String</span><span class="sxs-lookup"><span data-stu-id="68033-123">String</span></span>|<span data-ttu-id="68033-124">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="68033-124">Key of the entity.</span></span>|
|<span data-ttu-id="68033-125">pendingCount</span><span class="sxs-lookup"><span data-stu-id="68033-125">pendingCount</span></span>|<span data-ttu-id="68033-126">Int32</span><span class="sxs-lookup"><span data-stu-id="68033-126">Int32</span></span>|<span data-ttu-id="68033-127">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="68033-127">Number of pending Users</span></span>|
|<span data-ttu-id="68033-128">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="68033-128">notApplicableCount</span></span>|<span data-ttu-id="68033-129">Int32</span><span class="sxs-lookup"><span data-stu-id="68033-129">Int32</span></span>|<span data-ttu-id="68033-130">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="68033-130">Number of not applicable users</span></span>|
|<span data-ttu-id="68033-131">successCount</span><span class="sxs-lookup"><span data-stu-id="68033-131">successCount</span></span>|<span data-ttu-id="68033-132">Int32</span><span class="sxs-lookup"><span data-stu-id="68033-132">Int32</span></span>|<span data-ttu-id="68033-133">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="68033-133">Number of succeeded Users</span></span>|
|<span data-ttu-id="68033-134">errorCount</span><span class="sxs-lookup"><span data-stu-id="68033-134">errorCount</span></span>|<span data-ttu-id="68033-135">Int32</span><span class="sxs-lookup"><span data-stu-id="68033-135">Int32</span></span>|<span data-ttu-id="68033-136">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="68033-136">Number of error Users</span></span>|
|<span data-ttu-id="68033-137">failedCount</span><span class="sxs-lookup"><span data-stu-id="68033-137">failedCount</span></span>|<span data-ttu-id="68033-138">Int32</span><span class="sxs-lookup"><span data-stu-id="68033-138">Int32</span></span>|<span data-ttu-id="68033-139">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="68033-139">Number of failed Users</span></span>|
|<span data-ttu-id="68033-140">conflictCount</span><span class="sxs-lookup"><span data-stu-id="68033-140">conflictCount</span></span>|<span data-ttu-id="68033-141">Int32</span><span class="sxs-lookup"><span data-stu-id="68033-141">Int32</span></span>|<span data-ttu-id="68033-142">Número de usuários em conflito</span><span class="sxs-lookup"><span data-stu-id="68033-142">Number of users in conflict</span></span>|
|<span data-ttu-id="68033-143">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="68033-143">lastUpdateDateTime</span></span>|<span data-ttu-id="68033-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68033-144">DateTimeOffset</span></span>|<span data-ttu-id="68033-145">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="68033-145">Last update time</span></span>|
|<span data-ttu-id="68033-146">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="68033-146">configurationVersion</span></span>|<span data-ttu-id="68033-147">Int32</span><span class="sxs-lookup"><span data-stu-id="68033-147">Int32</span></span>|<span data-ttu-id="68033-148">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="68033-148">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="68033-149">Relações</span><span class="sxs-lookup"><span data-stu-id="68033-149">Relationships</span></span>
<span data-ttu-id="68033-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="68033-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="68033-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="68033-151">JSON Representation</span></span>
<span data-ttu-id="68033-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="68033-152">Here is a JSON representation of the resource.</span></span>
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





