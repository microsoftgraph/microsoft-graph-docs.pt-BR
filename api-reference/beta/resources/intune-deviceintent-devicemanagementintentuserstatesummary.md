---
title: tipo de recurso deviceManagementIntentUserStateSummary
description: Entidade que representa o resumo de estado do usuário para uma intenção
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fea6f40af4223bc14f7f1e419107c8b44b95f10e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49275633"
---
# <a name="devicemanagementintentuserstatesummary-resource-type"></a><span data-ttu-id="0e240-103">tipo de recurso deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="0e240-103">deviceManagementIntentUserStateSummary resource type</span></span>

<span data-ttu-id="0e240-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e240-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0e240-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0e240-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e240-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0e240-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e240-107">Entidade que representa o resumo de estado do usuário para uma intenção</span><span class="sxs-lookup"><span data-stu-id="0e240-107">Entity that represents user state summary for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="0e240-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="0e240-108">Methods</span></span>
|<span data-ttu-id="0e240-109">Método</span><span class="sxs-lookup"><span data-stu-id="0e240-109">Method</span></span>|<span data-ttu-id="0e240-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0e240-110">Return Type</span></span>|<span data-ttu-id="0e240-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e240-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0e240-112">Obter deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="0e240-112">Get deviceManagementIntentUserStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentuserstatesummary-get.md)|[<span data-ttu-id="0e240-113">deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="0e240-113">deviceManagementIntentUserStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|<span data-ttu-id="0e240-114">Leia as propriedades e as relações do objeto [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="0e240-114">Read properties and relationships of the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>|
|[<span data-ttu-id="0e240-115">Atualizar deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="0e240-115">Update deviceManagementIntentUserStateSummary</span></span>](../api/intune-deviceintent-devicemanagementintentuserstatesummary-update.md)|[<span data-ttu-id="0e240-116">deviceManagementIntentUserStateSummary</span><span class="sxs-lookup"><span data-stu-id="0e240-116">deviceManagementIntentUserStateSummary</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|<span data-ttu-id="0e240-117">Atualiza as propriedades de um objeto [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="0e240-117">Update the properties of a [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0e240-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0e240-118">Properties</span></span>
|<span data-ttu-id="0e240-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e240-119">Property</span></span>|<span data-ttu-id="0e240-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e240-120">Type</span></span>|<span data-ttu-id="0e240-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e240-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e240-122">id</span><span class="sxs-lookup"><span data-stu-id="0e240-122">id</span></span>|<span data-ttu-id="0e240-123">String</span><span class="sxs-lookup"><span data-stu-id="0e240-123">String</span></span>|<span data-ttu-id="0e240-124">A ID</span><span class="sxs-lookup"><span data-stu-id="0e240-124">The ID</span></span>|
|<span data-ttu-id="0e240-125">conflictCount</span><span class="sxs-lookup"><span data-stu-id="0e240-125">conflictCount</span></span>|<span data-ttu-id="0e240-126">Int32</span><span class="sxs-lookup"><span data-stu-id="0e240-126">Int32</span></span>|<span data-ttu-id="0e240-127">Número de usuários em conflito</span><span class="sxs-lookup"><span data-stu-id="0e240-127">Number of users in conflict</span></span>|
|<span data-ttu-id="0e240-128">errorCount</span><span class="sxs-lookup"><span data-stu-id="0e240-128">errorCount</span></span>|<span data-ttu-id="0e240-129">Int32</span><span class="sxs-lookup"><span data-stu-id="0e240-129">Int32</span></span>|<span data-ttu-id="0e240-130">Número de usuários de erro</span><span class="sxs-lookup"><span data-stu-id="0e240-130">Number of error users</span></span>|
|<span data-ttu-id="0e240-131">failedCount</span><span class="sxs-lookup"><span data-stu-id="0e240-131">failedCount</span></span>|<span data-ttu-id="0e240-132">Int32</span><span class="sxs-lookup"><span data-stu-id="0e240-132">Int32</span></span>|<span data-ttu-id="0e240-133">Número de usuários com falha</span><span class="sxs-lookup"><span data-stu-id="0e240-133">Number of failed users</span></span>|
|<span data-ttu-id="0e240-134">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="0e240-134">notApplicableCount</span></span>|<span data-ttu-id="0e240-135">Int32</span><span class="sxs-lookup"><span data-stu-id="0e240-135">Int32</span></span>|<span data-ttu-id="0e240-136">Número de usuários não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="0e240-136">Number of not applicable users</span></span>|
|<span data-ttu-id="0e240-137">successCount</span><span class="sxs-lookup"><span data-stu-id="0e240-137">successCount</span></span>|<span data-ttu-id="0e240-138">Int32</span><span class="sxs-lookup"><span data-stu-id="0e240-138">Int32</span></span>|<span data-ttu-id="0e240-139">Número de usuários com êxito</span><span class="sxs-lookup"><span data-stu-id="0e240-139">Number of succeeded users</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e240-140">Relações</span><span class="sxs-lookup"><span data-stu-id="0e240-140">Relationships</span></span>
<span data-ttu-id="0e240-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0e240-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e240-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0e240-142">JSON Representation</span></span>
<span data-ttu-id="0e240-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0e240-143">Here is a JSON representation of the resource.</span></span>
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




