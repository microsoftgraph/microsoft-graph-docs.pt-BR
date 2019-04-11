---
title: tipo de recurso deviceManagementIntentUserStateSummary
description: Entidade que representa o resumo de estado do usuário para uma intenção
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 538d1e5da36a1d90aac95641175eb0cebeeb69c3
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31790008"
---
# <a name="devicemanagementintentuserstatesummary-resource-type"></a><span data-ttu-id="7dede-103">tipo de recurso deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="7dede-103">deviceManagementIntentUserStateSummary resource type</span></span>

> <span data-ttu-id="7dede-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7dede-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7dede-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7dede-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7dede-106">Entidade que representa o resumo de estado do usuário para uma intenção</span><span class="sxs-lookup"><span data-stu-id="7dede-106">Entity that represents user state summary for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="7dede-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="7dede-107">Methods</span></span>
|<span data-ttu-id="7dede-108">Método</span><span class="sxs-lookup"><span data-stu-id="7dede-108">Method</span></span>|<span data-ttu-id="7dede-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7dede-109">Return Type</span></span>|<span data-ttu-id="7dede-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7dede-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7dede-111">Obter deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="7dede-111">Get deviceManagementIntentUserStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentuserstatesummary-get.md)|[<span data-ttu-id="7dede-112">deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="7dede-112">deviceManagementIntentUserStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|<span data-ttu-id="7dede-113">Leia as propriedades e as relações do objeto [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="7dede-113">Read properties and relationships of the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>|
|[<span data-ttu-id="7dede-114">Atualizar deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="7dede-114">Update deviceManagementIntentUserStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentuserstatesummary-update.md)|[<span data-ttu-id="7dede-115">deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="7dede-115">deviceManagementIntentUserStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|<span data-ttu-id="7dede-116">Atualiza as propriedades de um objeto [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="7dede-116">Update the properties of a [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7dede-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7dede-117">Properties</span></span>
|<span data-ttu-id="7dede-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7dede-118">Property</span></span>|<span data-ttu-id="7dede-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="7dede-119">Type</span></span>|<span data-ttu-id="7dede-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7dede-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7dede-121">id</span><span class="sxs-lookup"><span data-stu-id="7dede-121">id</span></span>|<span data-ttu-id="7dede-122">String</span><span class="sxs-lookup"><span data-stu-id="7dede-122">String</span></span>|<span data-ttu-id="7dede-123">A ID</span><span class="sxs-lookup"><span data-stu-id="7dede-123">The ID</span></span>|
|<span data-ttu-id="7dede-124">conflictCount</span><span class="sxs-lookup"><span data-stu-id="7dede-124">conflictCount</span></span>|<span data-ttu-id="7dede-125">Int32</span><span class="sxs-lookup"><span data-stu-id="7dede-125">Int32</span></span>|<span data-ttu-id="7dede-126">Número de usuários em conflito</span><span class="sxs-lookup"><span data-stu-id="7dede-126">Number of users in conflict</span></span>|
|<span data-ttu-id="7dede-127">errorCount</span><span class="sxs-lookup"><span data-stu-id="7dede-127">errorCount</span></span>|<span data-ttu-id="7dede-128">Int32</span><span class="sxs-lookup"><span data-stu-id="7dede-128">Int32</span></span>|<span data-ttu-id="7dede-129">Número de usuários de erro</span><span class="sxs-lookup"><span data-stu-id="7dede-129">Number of error users</span></span>|
|<span data-ttu-id="7dede-130">failedCount</span><span class="sxs-lookup"><span data-stu-id="7dede-130">failedCount</span></span>|<span data-ttu-id="7dede-131">Int32</span><span class="sxs-lookup"><span data-stu-id="7dede-131">Int32</span></span>|<span data-ttu-id="7dede-132">Número de usuários com falha</span><span class="sxs-lookup"><span data-stu-id="7dede-132">Number of failed users</span></span>|
|<span data-ttu-id="7dede-133">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="7dede-133">notApplicableCount</span></span>|<span data-ttu-id="7dede-134">Int32</span><span class="sxs-lookup"><span data-stu-id="7dede-134">Int32</span></span>|<span data-ttu-id="7dede-135">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="7dede-135">Number of not applicable users</span></span>|
|<span data-ttu-id="7dede-136">successCount</span><span class="sxs-lookup"><span data-stu-id="7dede-136">successCount</span></span>|<span data-ttu-id="7dede-137">Int32</span><span class="sxs-lookup"><span data-stu-id="7dede-137">Int32</span></span>|<span data-ttu-id="7dede-138">Número de usuários com êxito</span><span class="sxs-lookup"><span data-stu-id="7dede-138">Number of succeeded users</span></span>|

## <a name="relationships"></a><span data-ttu-id="7dede-139">Relações</span><span class="sxs-lookup"><span data-stu-id="7dede-139">Relationships</span></span>
<span data-ttu-id="7dede-140">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="7dede-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7dede-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7dede-141">JSON Representation</span></span>
<span data-ttu-id="7dede-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7dede-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentUserStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserStateSummary",
  "id": "String (identifier)",
  "conflictCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024
}
```





