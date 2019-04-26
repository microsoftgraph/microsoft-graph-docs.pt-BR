---
title: tipo de recurso securityBaselineStateSummary
description: O resumo do estado de conformidade da linha de base de segurança para a linha de base de segurança da conta.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8133fb325b0c2abdacf38e034aedc6523b13623c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562220"
---
# <a name="securitybaselinestatesummary-resource-type"></a><span data-ttu-id="1bfe3-103">tipo de recurso securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="1bfe3-103">securityBaselineStateSummary resource type</span></span>

> <span data-ttu-id="1bfe3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1bfe3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bfe3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1bfe3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bfe3-106">O resumo do estado de conformidade da linha de base de segurança para a linha de base de segurança da conta.</span><span class="sxs-lookup"><span data-stu-id="1bfe3-106">The security baseline compliance state summary for the security baseline of the account.</span></span>

## <a name="methods"></a><span data-ttu-id="1bfe3-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="1bfe3-107">Methods</span></span>
|<span data-ttu-id="1bfe3-108">Método</span><span class="sxs-lookup"><span data-stu-id="1bfe3-108">Method</span></span>|<span data-ttu-id="1bfe3-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1bfe3-109">Return Type</span></span>|<span data-ttu-id="1bfe3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bfe3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1bfe3-111">Obter securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="1bfe3-111">Get securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-get.md)|[<span data-ttu-id="1bfe3-112">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="1bfe3-112">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="1bfe3-113">Leia as propriedades e as relações do objeto [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="1bfe3-113">Read properties and relationships of the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|
|[<span data-ttu-id="1bfe3-114">Atualizar securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="1bfe3-114">Update securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-update.md)|[<span data-ttu-id="1bfe3-115">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="1bfe3-115">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="1bfe3-116">Atualiza as propriedades de um objeto [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="1bfe3-116">Update the properties of a [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1bfe3-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1bfe3-117">Properties</span></span>
|<span data-ttu-id="1bfe3-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1bfe3-118">Property</span></span>|<span data-ttu-id="1bfe3-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="1bfe3-119">Type</span></span>|<span data-ttu-id="1bfe3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bfe3-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bfe3-121">id</span><span class="sxs-lookup"><span data-stu-id="1bfe3-121">id</span></span>|<span data-ttu-id="1bfe3-122">String</span><span class="sxs-lookup"><span data-stu-id="1bfe3-122">String</span></span>|<span data-ttu-id="1bfe3-123">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="1bfe3-123">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="1bfe3-124">secureCount</span><span class="sxs-lookup"><span data-stu-id="1bfe3-124">secureCount</span></span>|<span data-ttu-id="1bfe3-125">Int32</span><span class="sxs-lookup"><span data-stu-id="1bfe3-125">Int32</span></span>|<span data-ttu-id="1bfe3-126">Número de dispositivos seguros</span><span class="sxs-lookup"><span data-stu-id="1bfe3-126">Number of secure devices</span></span>|
|<span data-ttu-id="1bfe3-127">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="1bfe3-127">notSecureCount</span></span>|<span data-ttu-id="1bfe3-128">Int32</span><span class="sxs-lookup"><span data-stu-id="1bfe3-128">Int32</span></span>|<span data-ttu-id="1bfe3-129">Número de dispositivos não seguros</span><span class="sxs-lookup"><span data-stu-id="1bfe3-129">Number of not secure devices</span></span>|
|<span data-ttu-id="1bfe3-130">unknownCount</span><span class="sxs-lookup"><span data-stu-id="1bfe3-130">unknownCount</span></span>|<span data-ttu-id="1bfe3-131">Int32</span><span class="sxs-lookup"><span data-stu-id="1bfe3-131">Int32</span></span>|<span data-ttu-id="1bfe3-132">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="1bfe3-132">Number of unknown devices</span></span>|
|<span data-ttu-id="1bfe3-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="1bfe3-133">errorCount</span></span>|<span data-ttu-id="1bfe3-134">Int32</span><span class="sxs-lookup"><span data-stu-id="1bfe3-134">Int32</span></span>|<span data-ttu-id="1bfe3-135">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="1bfe3-135">Number of error devices</span></span>|
|<span data-ttu-id="1bfe3-136">conflictCount</span><span class="sxs-lookup"><span data-stu-id="1bfe3-136">conflictCount</span></span>|<span data-ttu-id="1bfe3-137">Int32</span><span class="sxs-lookup"><span data-stu-id="1bfe3-137">Int32</span></span>|<span data-ttu-id="1bfe3-138">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="1bfe3-138">Number of conflict devices</span></span>|
|<span data-ttu-id="1bfe3-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="1bfe3-139">notApplicableCount</span></span>|<span data-ttu-id="1bfe3-140">Int32</span><span class="sxs-lookup"><span data-stu-id="1bfe3-140">Int32</span></span>|<span data-ttu-id="1bfe3-141">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="1bfe3-141">Number of not applicable devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="1bfe3-142">Relações</span><span class="sxs-lookup"><span data-stu-id="1bfe3-142">Relationships</span></span>
<span data-ttu-id="1bfe3-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1bfe3-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1bfe3-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1bfe3-144">JSON Representation</span></span>
<span data-ttu-id="1bfe3-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1bfe3-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineStateSummary",
  "id": "String (identifier)",
  "secureCount": 1024,
  "notSecureCount": 1024,
  "unknownCount": 1024,
  "errorCount": 1024,
  "conflictCount": 1024,
  "notApplicableCount": 1024
}
```





