---
title: Tipo de recurso deviceComplianceUserOverview
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: fd11bb0949e9279b826cfc12e4c89a9f6b34ff53
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305261"
---
# <a name="devicecomplianceuseroverview-resource-type"></a><span data-ttu-id="29281-103">Tipo de recurso deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="29281-103">deviceComplianceUserOverview resource type</span></span>

> <span data-ttu-id="29281-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="29281-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29281-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="29281-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="29281-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="29281-106">Methods</span></span>
|<span data-ttu-id="29281-107">Método</span><span class="sxs-lookup"><span data-stu-id="29281-107">Method</span></span>|<span data-ttu-id="29281-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="29281-108">Return Type</span></span>|<span data-ttu-id="29281-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="29281-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="29281-110">Obter deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="29281-110">Get deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-get.md)|[<span data-ttu-id="29281-111">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="29281-111">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="29281-112">Ler propriedades e relações de objetos de [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="29281-112">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|
|[<span data-ttu-id="29281-113">Atualizar deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="29281-113">Update deviceComplianceUserOverview</span></span>](../api/intune-deviceconfig-devicecomplianceuseroverview-update.md)|[<span data-ttu-id="29281-114">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="29281-114">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="29281-115">Atualizar as propriedades de um objeto de [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="29281-115">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="29281-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="29281-116">Properties</span></span>
|<span data-ttu-id="29281-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29281-117">Property</span></span>|<span data-ttu-id="29281-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="29281-118">Type</span></span>|<span data-ttu-id="29281-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="29281-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29281-120">id</span><span class="sxs-lookup"><span data-stu-id="29281-120">id</span></span>|<span data-ttu-id="29281-121">String</span><span class="sxs-lookup"><span data-stu-id="29281-121">String</span></span>|<span data-ttu-id="29281-122">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="29281-122">Key of the entity.</span></span>|
|<span data-ttu-id="29281-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="29281-123">pendingCount</span></span>|<span data-ttu-id="29281-124">Int32</span><span class="sxs-lookup"><span data-stu-id="29281-124">Int32</span></span>|<span data-ttu-id="29281-125">Número de usuários pendentes</span><span class="sxs-lookup"><span data-stu-id="29281-125">Number of pending Users</span></span>|
|<span data-ttu-id="29281-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="29281-126">notApplicableCount</span></span>|<span data-ttu-id="29281-127">Int32</span><span class="sxs-lookup"><span data-stu-id="29281-127">Int32</span></span>|<span data-ttu-id="29281-128">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="29281-128">Number of not applicable users</span></span>|
|<span data-ttu-id="29281-129">successCount</span><span class="sxs-lookup"><span data-stu-id="29281-129">successCount</span></span>|<span data-ttu-id="29281-130">Int32</span><span class="sxs-lookup"><span data-stu-id="29281-130">Int32</span></span>|<span data-ttu-id="29281-131">Número de usuários bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="29281-131">Number of succeeded Users</span></span>|
|<span data-ttu-id="29281-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="29281-132">errorCount</span></span>|<span data-ttu-id="29281-133">Int32</span><span class="sxs-lookup"><span data-stu-id="29281-133">Int32</span></span>|<span data-ttu-id="29281-134">Número de usuários com erro</span><span class="sxs-lookup"><span data-stu-id="29281-134">Number of error Users</span></span>|
|<span data-ttu-id="29281-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="29281-135">failedCount</span></span>|<span data-ttu-id="29281-136">Int32</span><span class="sxs-lookup"><span data-stu-id="29281-136">Int32</span></span>|<span data-ttu-id="29281-137">Número de usuários com falhas</span><span class="sxs-lookup"><span data-stu-id="29281-137">Number of failed Users</span></span>|
|<span data-ttu-id="29281-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="29281-138">lastUpdateDateTime</span></span>|<span data-ttu-id="29281-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29281-139">DateTimeOffset</span></span>|<span data-ttu-id="29281-140">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="29281-140">Last update time</span></span>|
|<span data-ttu-id="29281-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="29281-141">configurationVersion</span></span>|<span data-ttu-id="29281-142">Int32</span><span class="sxs-lookup"><span data-stu-id="29281-142">Int32</span></span>|<span data-ttu-id="29281-143">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="29281-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="29281-144">Relações</span><span class="sxs-lookup"><span data-stu-id="29281-144">Relationships</span></span>
<span data-ttu-id="29281-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="29281-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="29281-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="29281-146">JSON Representation</span></span>
<span data-ttu-id="29281-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="29281-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceUserOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
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



