---
title: tipo de recurso securityBaselineStateSummary
description: O resumo do estado de conformidade da linha de base de segurança para a linha de base de segurança da conta.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d5d4fc9c256ca498e1a9e14136397847cf5c1953
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43419669"
---
# <a name="securitybaselinestatesummary-resource-type"></a><span data-ttu-id="c946c-103">tipo de recurso securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="c946c-103">securityBaselineStateSummary resource type</span></span>

<span data-ttu-id="c946c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c946c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c946c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c946c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c946c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c946c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c946c-107">O resumo do estado de conformidade da linha de base de segurança para a linha de base de segurança da conta.</span><span class="sxs-lookup"><span data-stu-id="c946c-107">The security baseline compliance state summary for the security baseline of the account.</span></span>

## <a name="methods"></a><span data-ttu-id="c946c-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="c946c-108">Methods</span></span>
|<span data-ttu-id="c946c-109">Método</span><span class="sxs-lookup"><span data-stu-id="c946c-109">Method</span></span>|<span data-ttu-id="c946c-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c946c-110">Return Type</span></span>|<span data-ttu-id="c946c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c946c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c946c-112">Obter securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="c946c-112">Get securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-get.md)|[<span data-ttu-id="c946c-113">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="c946c-113">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="c946c-114">Leia as propriedades e as relações do objeto [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="c946c-114">Read properties and relationships of the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|
|[<span data-ttu-id="c946c-115">Atualizar securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="c946c-115">Update securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-update.md)|[<span data-ttu-id="c946c-116">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="c946c-116">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="c946c-117">Atualiza as propriedades de um objeto [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="c946c-117">Update the properties of a [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c946c-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c946c-118">Properties</span></span>
|<span data-ttu-id="c946c-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c946c-119">Property</span></span>|<span data-ttu-id="c946c-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="c946c-120">Type</span></span>|<span data-ttu-id="c946c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c946c-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c946c-122">id</span><span class="sxs-lookup"><span data-stu-id="c946c-122">id</span></span>|<span data-ttu-id="c946c-123">String</span><span class="sxs-lookup"><span data-stu-id="c946c-123">String</span></span>|<span data-ttu-id="c946c-124">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="c946c-124">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="c946c-125">secureCount</span><span class="sxs-lookup"><span data-stu-id="c946c-125">secureCount</span></span>|<span data-ttu-id="c946c-126">Int32</span><span class="sxs-lookup"><span data-stu-id="c946c-126">Int32</span></span>|<span data-ttu-id="c946c-127">Número de dispositivos seguros</span><span class="sxs-lookup"><span data-stu-id="c946c-127">Number of secure devices</span></span>|
|<span data-ttu-id="c946c-128">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="c946c-128">notSecureCount</span></span>|<span data-ttu-id="c946c-129">Int32</span><span class="sxs-lookup"><span data-stu-id="c946c-129">Int32</span></span>|<span data-ttu-id="c946c-130">Número de dispositivos não seguros</span><span class="sxs-lookup"><span data-stu-id="c946c-130">Number of not secure devices</span></span>|
|<span data-ttu-id="c946c-131">unknownCount</span><span class="sxs-lookup"><span data-stu-id="c946c-131">unknownCount</span></span>|<span data-ttu-id="c946c-132">Int32</span><span class="sxs-lookup"><span data-stu-id="c946c-132">Int32</span></span>|<span data-ttu-id="c946c-133">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="c946c-133">Number of unknown devices</span></span>|
|<span data-ttu-id="c946c-134">errorCount</span><span class="sxs-lookup"><span data-stu-id="c946c-134">errorCount</span></span>|<span data-ttu-id="c946c-135">Int32</span><span class="sxs-lookup"><span data-stu-id="c946c-135">Int32</span></span>|<span data-ttu-id="c946c-136">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="c946c-136">Number of error devices</span></span>|
|<span data-ttu-id="c946c-137">conflictCount</span><span class="sxs-lookup"><span data-stu-id="c946c-137">conflictCount</span></span>|<span data-ttu-id="c946c-138">Int32</span><span class="sxs-lookup"><span data-stu-id="c946c-138">Int32</span></span>|<span data-ttu-id="c946c-139">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="c946c-139">Number of conflict devices</span></span>|
|<span data-ttu-id="c946c-140">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="c946c-140">notApplicableCount</span></span>|<span data-ttu-id="c946c-141">Int32</span><span class="sxs-lookup"><span data-stu-id="c946c-141">Int32</span></span>|<span data-ttu-id="c946c-142">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="c946c-142">Number of not applicable devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="c946c-143">Relações</span><span class="sxs-lookup"><span data-stu-id="c946c-143">Relationships</span></span>
<span data-ttu-id="c946c-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c946c-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c946c-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c946c-145">JSON Representation</span></span>
<span data-ttu-id="c946c-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c946c-146">Here is a JSON representation of the resource.</span></span>
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



