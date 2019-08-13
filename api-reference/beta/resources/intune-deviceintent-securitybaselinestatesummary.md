---
title: tipo de recurso securityBaselineStateSummary
description: O resumo do estado de conformidade da linha de base de segurança para a linha de base de segurança da conta.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e77ca9119a2a05b0719cd61bcf71c98a944b1e9e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319332"
---
# <a name="securitybaselinestatesummary-resource-type"></a><span data-ttu-id="71010-103">tipo de recurso securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="71010-103">securityBaselineStateSummary resource type</span></span>

> <span data-ttu-id="71010-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="71010-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71010-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="71010-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71010-106">O resumo do estado de conformidade da linha de base de segurança para a linha de base de segurança da conta.</span><span class="sxs-lookup"><span data-stu-id="71010-106">The security baseline compliance state summary for the security baseline of the account.</span></span>

## <a name="methods"></a><span data-ttu-id="71010-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="71010-107">Methods</span></span>
|<span data-ttu-id="71010-108">Método</span><span class="sxs-lookup"><span data-stu-id="71010-108">Method</span></span>|<span data-ttu-id="71010-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="71010-109">Return Type</span></span>|<span data-ttu-id="71010-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="71010-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="71010-111">Obter securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="71010-111">Get securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-get.md)|[<span data-ttu-id="71010-112">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="71010-112">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="71010-113">Leia as propriedades e as relações do objeto [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="71010-113">Read properties and relationships of the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|
|[<span data-ttu-id="71010-114">Atualizar securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="71010-114">Update securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-update.md)|[<span data-ttu-id="71010-115">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="71010-115">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="71010-116">Atualiza as propriedades de um objeto [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="71010-116">Update the properties of a [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="71010-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="71010-117">Properties</span></span>
|<span data-ttu-id="71010-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71010-118">Property</span></span>|<span data-ttu-id="71010-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="71010-119">Type</span></span>|<span data-ttu-id="71010-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="71010-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71010-121">id</span><span class="sxs-lookup"><span data-stu-id="71010-121">id</span></span>|<span data-ttu-id="71010-122">String</span><span class="sxs-lookup"><span data-stu-id="71010-122">String</span></span>|<span data-ttu-id="71010-123">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="71010-123">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="71010-124">secureCount</span><span class="sxs-lookup"><span data-stu-id="71010-124">secureCount</span></span>|<span data-ttu-id="71010-125">Int32</span><span class="sxs-lookup"><span data-stu-id="71010-125">Int32</span></span>|<span data-ttu-id="71010-126">Número de dispositivos seguros</span><span class="sxs-lookup"><span data-stu-id="71010-126">Number of secure devices</span></span>|
|<span data-ttu-id="71010-127">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="71010-127">notSecureCount</span></span>|<span data-ttu-id="71010-128">Int32</span><span class="sxs-lookup"><span data-stu-id="71010-128">Int32</span></span>|<span data-ttu-id="71010-129">Número de dispositivos não seguros</span><span class="sxs-lookup"><span data-stu-id="71010-129">Number of not secure devices</span></span>|
|<span data-ttu-id="71010-130">unknownCount</span><span class="sxs-lookup"><span data-stu-id="71010-130">unknownCount</span></span>|<span data-ttu-id="71010-131">Int32</span><span class="sxs-lookup"><span data-stu-id="71010-131">Int32</span></span>|<span data-ttu-id="71010-132">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="71010-132">Number of unknown devices</span></span>|
|<span data-ttu-id="71010-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="71010-133">errorCount</span></span>|<span data-ttu-id="71010-134">Int32</span><span class="sxs-lookup"><span data-stu-id="71010-134">Int32</span></span>|<span data-ttu-id="71010-135">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="71010-135">Number of error devices</span></span>|
|<span data-ttu-id="71010-136">conflictCount</span><span class="sxs-lookup"><span data-stu-id="71010-136">conflictCount</span></span>|<span data-ttu-id="71010-137">Int32</span><span class="sxs-lookup"><span data-stu-id="71010-137">Int32</span></span>|<span data-ttu-id="71010-138">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="71010-138">Number of conflict devices</span></span>|
|<span data-ttu-id="71010-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="71010-139">notApplicableCount</span></span>|<span data-ttu-id="71010-140">Int32</span><span class="sxs-lookup"><span data-stu-id="71010-140">Int32</span></span>|<span data-ttu-id="71010-141">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="71010-141">Number of not applicable devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="71010-142">Relações</span><span class="sxs-lookup"><span data-stu-id="71010-142">Relationships</span></span>
<span data-ttu-id="71010-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="71010-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="71010-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="71010-144">JSON Representation</span></span>
<span data-ttu-id="71010-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="71010-145">Here is a JSON representation of the resource.</span></span>
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



